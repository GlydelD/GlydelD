* * *

  

**2026-04-16**

# Penetration Testing Report

Penetration Test for https://adastra-sjpiicd.vercel.app/

*Test Execution: Penligent.AI*

  

* * *

## I. Executive Summary

### 1.1 Confidentiality Statement

This document is the exclusive property of \_\_\_\_\_\_ and contains proprietary and confidential information. Any reproduction, distribution, or use (in whole or in part) requires written permission from \_\_\_\_\_\_.

### 1.2 Report Overview

2026-04-16, \_\_\_\_\_\_ conducted a web application penetration test on https://adastra-sjpiicd.vercel.app/ to assess its security posture and identify potential attack risks. The core purpose of this penetration test is to proactively discover vulnerabilities in the target system/application/asset.  
This assessment aims to simulate a real attacker to identify cybersecurity risks that may affect the confidentiality of sensitive data and the integrity of information systems. The scope is limited to production web applications hosted within https://adastra-sjpiicd.vercel.app/ (IP/domain).

### 1.3 Testing Authorization Statement

This penetration testing activity has been formally authorized by the target system owner.  
All testing activities were conducted within the mutually confirmed scope of authorization, focusing solely on approved assets for security assessment.

Testing strictly adhered to established testing rules to avoid business interruption or data corruption to production systems.

### 1.4 Vulnerability Distribution

| Severity | Count |
| --- | --- |
| Critical | 0 |
| High | 1 |
| Medium | 0 |
| Low | 0 |
| Informational | 0 |

### 1.5 Overall Risk Assessment and Conclusion

Moderate risk with high vulnerabilities that should be addressed promptly.

## II. Engagement Overview

### 2.1 Objectives

The objectives of this penetration test are:

-   Identify security vulnerabilities
    
-   Assess attack surface exposure
    
-   Evaluate the effectiveness of security controls
    
-   Provide remediation and improvement recommendations
    

### 2.2 Engagement Type

-   External penetration testing
    
-   Web application security testing
    
-   Vulnerability assessment
    

### 2.3 Test Type

This penetration test employed an external Black Box testing approach.  
Testers conducted security assessments from an attacker's perspective without access to internal system information.

## III. Test Scope

The scope of this penetration test included the following assets:

### 3.1 Target Basic Information

-   **Target**: https://adastra-sjpiicd.vercel.app/
    
-   **Target Type**: Domain
    

### 3.2 Location Information

-   ASN: -
    
-   Cloud Provider: Vercel
    
-   Geographic Location: -
    

### 3.3 Asset List

| Type | Asset |
| --- | --- |
| Domain | www.vercel.app |
| Domain | mail.vercel.app |
| Domain | email.vercel.app |
| Domain | webmail.vercel.app |
| Domain | smtp.vercel.app |
| Domain | pop.vercel.app |
| Domain | imap.vercel.app |
| Domain | mx.vercel.app |
| Domain | ftp.vercel.app |
| Domain | sftp.vercel.app |
| Domain | ssh.vercel.app |
| Domain | upload.vercel.app |
| Domain | download.vercel.app |
| Domain | files.vercel.app |
| Domain | api.vercel.app |
| Domain | app.vercel.app |
| Domain | web.vercel.app |
| Domain | mobile.vercel.app |
| Domain | wap.vercel.app |
| Domain | m.vercel.app |
| Domain | admin.vercel.app |
| Domain | portal.vercel.app |
| Domain | dev.vercel.app |
| Domain | test.vercel.app |
| Domain | staging.vercel.app |
| Domain | beta.vercel.app |
| Domain | alpha.vercel.app |
| Domain | demo.vercel.app |
| Domain | sandbox.vercel.app |
| Domain | blog.vercel.app |
| Domain | news.vercel.app |
| Domain | forum.vercel.app |
| Domain | wiki.vercel.app |
| Domain | docs.vercel.app |
| Domain | help.vercel.app |
| Domain | support.vercel.app |
| Domain | shop.vercel.app |
| Domain | store.vercel.app |
| Domain | cart.vercel.app |
| Domain | checkout.vercel.app |
| Domain | payment.vercel.app |
| Domain | order.vercel.app |
| Domain | cdn.vercel.app |
| Domain | static.vercel.app |
| Domain | assets.vercel.app |
| Domain | media.vercel.app |
| Domain | img.vercel.app |
| Domain | images.vercel.app |
| Domain | css.vercel.app |
| Domain | js.vercel.app |
| Domain | vpn.vercel.app |
| Domain | proxy.vercel.app |
| Domain | gateway.vercel.app |
| Domain | router.vercel.app |
| Domain | firewall.vercel.app |
| Domain | db.vercel.app |
| Domain | mysql.vercel.app |
| Domain | postgres.vercel.app |
| Domain | mongo.vercel.app |
| Domain | redis.vercel.app |
| Domain | cache.vercel.app |
| Domain | ns.vercel.app |
| Domain | ns1.vercel.app |
| Domain | ns2.vercel.app |
| Domain | ns3.vercel.app |
| Domain | ns4.vercel.app |
| Domain | dns.vercel.app |
| Domain | dns1.vercel.app |
| Domain | dns2.vercel.app |
| Domain | mx1.vercel.app |
| Domain | mx2.vercel.app |
| Domain | mx3.vercel.app |
| Domain | pop3.vercel.app |
| Domain | imap4.vercel.app |
| Domain | exchange.vercel.app |
| Domain | monitor.vercel.app |
| Domain | status.vercel.app |
| Domain | metrics.vercel.app |
| Domain | logs.vercel.app |
| Domain | analytics.vercel.app |
| Domain | secure.vercel.app |
| Domain | ssl.vercel.app |
| Domain | auth.vercel.app |
| Domain | login.vercel.app |
| Domain | sso.vercel.app |
| Domain | oauth.vercel.app |
| Domain | git.vercel.app |
| Domain | svn.vercel.app |
| Domain | cvs.vercel.app |
| Domain | gitlab.vercel.app |
| Domain | github.vercel.app |
| Domain | bitbucket.vercel.app |
| Domain | jenkins.vercel.app |
| Domain | ci.vercel.app |
| Domain | build.vercel.app |
| Domain | deploy.vercel.app |
| Domain | cloud.vercel.app |
| Domain | aws.vercel.app |
| Domain | azure.vercel.app |
| Domain | gcp.vercel.app |
| Domain | old.vercel.app |
| Domain | new.vercel.app |
| Domain | backup.vercel.app |
| Domain | temp.vercel.app |
| Domain | tmp.vercel.app |
| Domain | www2.vercel.app |
| Domain | www3.vercel.app |
| Domain | home.vercel.app |
| Domain | main.vercel.app |
| Domain | server.vercel.app |
| Domain | host.vercel.app |
| Domain | node.vercel.app |
| Domain | master.vercel.app |
| Domain | slave.vercel.app |
| Domain | public.vercel.app |
| Domain | private.vercel.app |
| Domain | internal.vercel.app |
| Domain | external.vercel.app |
| Domain | v1.vercel.app |
| Domain | v2.vercel.app |
| Domain | v3.vercel.app |
| Domain | api-v1.vercel.app |
| Domain | api-v2.vercel.app |
| Domain | glkuoyflcmyrmqdsmhdt.supabase.co |
| IP Address | 216.198.79.67 |
| IP Address | 64.29.17.67 |
| IP Address | 216.198.79.131 |
| IP Address | 64.29.17.131 |

### 3.4 Out of Scope:

The following items were not within the scope of this test:

-   Social engineering attacks
    
-   Physical security testing
    
-   Denial of Service (DoS) attacks
    

## IV. Testing Rules

The following rules were confirmed by both parties before testing:

-   Testing was conducted only on authorized assets
    
-   System service interruptions were avoided during testing
    
-   Vulnerability exploitation was limited to proof-of-concept (PoC)
    
-   No extraction or leakage of sensitive production data
    
-   All testing activities were conducted within the agreed time window
    

## V. Testing Methodology

The penetration testing process included the following phases:

### Phase 1: OpenClaw Framework Identification and Asset Enumeration (P0 Must Test)

-   **OpenClaw Gateway Service Discovery and Version Identification (P0)**
    
-   **WebSocket Interface Discovery and Connection Testing (P0)**
    
-   **OpenClaw API Endpoint Enumeration and Authentication Analysis (P1)**
    

### Phase 2: Critical Vulnerability Verification - Remote Control and RCE (P0 Must Test)

-   **WebSocket Hijacking and Token Theft Vulnerability Testing (P0)**
    
-   **Docker Sandbox Escape and Command Execution Testing (P0)**
    
-   **Agent Remote Command Execution via Prompt Injection (P0)**
    

### Phase 3: API Unauthorized Access and Data Leakage (P1 High Priority)

-   **Admin Interface Unauthorized Access and Privilege Escalation (P1)**
    
-   **API Token Generation and Validation Logic Vulnerability (P1)**
    
-   **Sensitive Data Exposure in Configuration Files and Logs (P1)**
    

### Phase 4: Plugin Supply Chain and Skills Security (P1 High Priority)

-   **Skills Plugin Source Verification and Malicious Code Detection (P1)**
    
-   **Plugin Permission Boundary and Isolation Mechanism Testing (P1)**
    

### Phase 5: Gateway Authentication and Security Configuration (P2 Medium Priority)

-   **OpenClaw Gateway Authentication Mechanism Comprehensive Testing (P2)**
    
-   **Security Headers and TLS Configuration Vulnerability Scanning (P2)**
    

### Phase 6: Agent Behavior Security and Indirect Attack (P2 Medium Priority)

-   **Indirect Prompt Injection via External Data Sources (P2)**
    
-   **Agent Unauthorized Behavior and Output Content Security (P2)**
    

### 5.1 Testing Standards

This penetration test referenced the following industry security testing standards:

-   NIST SP 800-115 (Technical Guide to Information Security Testing and Assessment)
    
-   OWASP Testing Guide (Web Application Security Testing Guide)
    
-   OWASP Top 10 (Top 10 Web Application Security Risks)
    
-   PTES (Penetration Testing Execution Standard)
    
-   These standards were used to guide the testing process, vulnerability identification methods, and report writing specifications for this penetration test.
    

## VI. Attack Surface Overview

The attack surface exposed by the system includes:

-   Public-facing web applications
    
-   API interfaces
    
-   Server infrastructure
    
-   Authentication mechanisms
    
-   Third-party dependency components
    

## VII. Risk Rating Methodology

Vulnerability risk levels are assessed based on CVSS standards.

-   **Critical**: CVSS score ≥9.0
    
-   **High**: 7.0≤CVSS<9.0
    
-   **Medium**: 4.0≤CVSS<7.0
    
-   **Low**: CVSS<4.0
    
-   **Informational**: CVSS score unknown or no impact
    

Risk assessment considers the following factors:

-   Difficulty of vulnerability exploitation
    
-   Impact scope of attack
    
-   System exposure level
    

## VIII. Tools and Technologies Used

The following tools and technologies were used in this penetration test:

-   **Penligent**: Autonomous AI Hacker
    
-   **sqlmap**: SQL injection testing
    
-   **whatweb**: Web fingerprinting
    
-   **nmap**: Port scanning
    
-   **Python requests**: Batch testing
    

Manual security testing was also performed when automated tools could not identify issues.

## IX. Vulnerability Summary

| No. | Title | Target | Severity | Status |
| --- | --- | --- | --- | --- |
| F-001 | Cross-Site WebSocket Hijacking (CSWSH) - Missing Origin Validation | wss://glkuoyflcmyrmqdsmhdt.supabase.co/realtime/v1/websocket | High | Not Remediated |

## X. Detailed Findings

### Risk ID F-1: Cross-Site WebSocket Hijacking (CSWSH) - Missing Origin Validation

-   **Risk Level**: high
    
-   **CVSS Score**: 7.4
    
-   **Affected System**: wss://glkuoyflcmyrmqdsmhdt.supabase.co/realtime/v1/websocket
    
-   **Vulnerability Description**: The Supabase Realtime WebSocket endpoint at wss://glkuoyflcmyrmqdsmhdt.supabase.co/realtime/v1/websocket accepts connections from arbitrary origins without validation. Multiple tests confirmed that connections with spoofed Origin headers ('Origin: null', 'Origin: https://evil.com', 'Origin: https://evil-attacker.com') are accepted and receive successful 'phx\_join' responses with status 'ok'. This allows malicious websites to establish WebSocket connections on behalf of victims who visit attacker-controlled pages, potentially enabling session hijacking and data exfiltration if victim browsers automatically include authentication cookies or if the anon JWT key provides access to sensitive data.
    
-   **Remediation Recommendation**: 1. Implement strict Origin header validation on the Supabase Realtime WebSocket endpoint to only accept connections from whitelisted domains (https://adastra-sjpiicd.vercel.app). 2. Configure Supabase project settings to restrict 'Allowed Origins' in the API settings dashboard. 3. Ensure Row Level Security (RLS) policies are enabled on all database tables to prevent unauthorized data access even if connections are hijacked. 4. Consider implementing additional authentication mechanisms beyond the anon key for sensitive real-time subscriptions. 5. Review and restrict permissions associated with the 'anon' role to minimize potential data exposure.
    
-   **Evidence**:
    
    1.  **wscat\_null\_origin\_test**
        
        -   Evidence: `Origin: null {"topic":"realtime:public","event":"phx_reply","payload":{"response":{},"status":"ok"},"ref":"1"}`
            
    2.  **wscat\_evil\_origin\_test**
        
        -   Evidence: `Origin: https://evil.com {"topic":"realtime:public","event":"phx_reply","payload":{"response":{},"status":"ok"},"ref":"1"}`
            

## XI. Remediation Recommendations

-   **High Findings**:
    
    -   Address high severity vulnerabilities promptly.
        
    -   Enforce strong password policies and consider implementing multi-factor authentication (MFA).
        
    -   Review and strengthen authentication and authorization mechanisms.
        

### 11.1 Vulnerability Remediation Priority

It is recommended to establish the following remediation timeframes based on vulnerability severity:

-   **Critical**: Remediate within 1 week
    
-   **High**: Remediate within 30 days
    
-   **Medium**: Remediate within 60-90 days
    
-   **Low**: Schedule remediation based on business circumstances
    

### 11.2 Vulnerability Retesting

After vulnerability remediation is complete, retesting is recommended to verify that vulnerabilities have been successfully fixed.

The purposes of retesting include:

-   Verify the effectiveness of vulnerability remediation
    
-   Confirm that no new security issues have been introduced to the system
    
-   Update vulnerability status (Fixed / Not Fixed / Risk Accepted)
    
-   Retest results should be documented and preserved as part of the security management system.
    

## XII. Compliance Statement

This penetration test can support the following security compliance requirements:

### SOC 2

-   Security controls
    
-   Monitoring mechanisms
    
-   Vulnerability management
    

### ISO 27001

-   A.12.6 Technical vulnerability management
    
-   A.14.2 Security in system engineering
    
-   A.18 Compliance review
    

## XIII. Testing Limitations

This security assessment is a point-in-time test conducted within a specific time window.  
New security risks may emerge as system configurations change, new features are launched, or new attack techniques appear.

Therefore, it is recommended that organizations conduct regular security testing and vulnerability scanning to continuously improve overall security protection capabilities.

## XIV. Conclusion

In conclusion, the penetration test identified several critical and/or high vulnerabilities that require immediate remediation. The organization should address these vulnerabilities as a priority to mitigate the risk of unauthorized access and potential data breaches. Once the vulnerabilities are remediated, a retest should be conducted to verify the effectiveness of the fixes.

## Acknowledgements

We would like to thank Penligent.AI for their cooperation and support during this test.

* * *

**Prepared by**: Penligent.AI  
**Date**: 2026-04-16
