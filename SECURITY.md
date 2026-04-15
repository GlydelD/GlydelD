#Security Vulnerability Report – Unauthorized Storage Enumeration and Object Access (Supabase)
#Summary

An authorization misconfiguration in Supabase Storage allows unauthenticated or low-privileged users (anon role) to list and download objects from a restricted storage bucket, potentially enabling unauthorized access to stored files.

#Affected Component
Service: Supabase Storage API

#Endpoint:

POST /storage/v1/object/list/{bucket}
GET  /storage/v1/object/{bucket}/{file}
Bucket: Signature
Path Affected: signatures/
#Vulnerability Type
Broken Access Control (OWASP A01:2021)
Insecure Direct Object Reference (IDOR)
Improper Storage Access Control
#Technical Details

Using a valid Supabase anon JWT token, it is possible to:

Enumerate files in the storage bucket
POST /storage/v1/object/list/Signature
Download objects without authentication enforcement
GET /storage/v1/object/Signature/{filename}

The following request headers were sufficient:

apikey: <anon-key>
Authorization: Bearer <anon-key>
#Proof of Concept

Example request successfully returns file listings:

Downloading: 2010-0277_ETING_9883b12f-d0ac-46d2-bc3b-9a73dc418e41.webp
Downloading: 2013-1187_CASTILLANO_d364edcd-5ad6-41a2-8881-12f5fbb72842.webp
Downloading: 2014-1324_SABULAAN_4e97cee9-3a21-44ee-9e9d-694fa0b2bf1e.webp

This confirms:

File enumeration is enabled
Direct object access is permitted via anon role
#Impact

If the affected bucket contains sensitive or user-related data (e.g. signatures, IDs, documents), this vulnerability can lead to:

Unauthorized data exposure
Mass file scraping / bulk download
Privacy violation (PII leakage if present)
Data harvesting for external abuse

Even if data is not currently sensitive, the misconfiguration introduces a scalable data exposure risk.

#Severity Assessment
Severity: High (potentially Critical depending on stored data)
CVSS Estimate: 7.5 – 9.1 (High to Critical range)
#Root Cause

Likely misconfiguration in Supabase Storage policies:

Overly permissive SELECT policy on storage.objects
Bucket allowing public listing or anon access
Missing row-level security (RLS) restrictions for object access
#Recommended Fix
Restrict object listing
Disable public listing unless explicitly required

Enforce RLS policies

Allow only authenticated users or owners:
USING (auth.role() = 'authenticated')
Make bucket private
Ensure Signature bucket is not publicly accessible
Add ownership validation
Restrict access based on user ID or metadata path ownership
Avoid exposing anon key in high-privilege contexts
#Notes
The issue is reproducible using only the Supabase anon key
No authentication bypass or token manipulation was required
Exploitation allows full enumeration of stored objects under the specified prefix
#Environment
Supabase Storage API
Vercel-hosted frontend observed: https://adastra-sjpiicd.vercel.app/
Testing performed using curl + jq
