# Cybersecurity SOC Investigations | Wireshark Labs

## Project Overview

This repository documents my hands-on cybersecurity investigations using Wireshark as part of the NetworkWalks SOC Analyst training programme.

The project focuses on analysing network traffic, identifying suspicious behaviour, investigating security incidents, and understanding how attackers exploit network vulnerabilities.

These investigations were completed in a simulated training environment.

## Tools and Skills

- Wireshark
- Network traffic analysis
- TCP/IP protocol analysis
- Packet filtering
- SOC investigation techniques
- Incident detection and analysis
- HTTP, FTP, DNS, SIP and RTP analysis

## Lab Investigations

### Lab 3: Identifying a Port Scan

**Objective:** Identify an attacker scanning a server for open ports.

**Findings:**
- Attacker IP: 192.168.10.66
- Target IP: 192.168.10.20
- Ports scanned: 40
- Open ports: 22, 80, 443
- Closed ports: 37
- Attack identified: TCP port scan

**Skills gained:** TCP flag analysis, SYN packets, SYN-ACK responses and identifying reconnaissance activity.

### Lab 4: Investigating Plaintext Chat Traffic

**Objective:** Investigate an unencrypted office chat conversation.

**Findings:**
- Chat protocol: TCP
- Server port: 5000
- Client IP: 192.168.10.45
- TCP stream: 5
- Conversation size: 413 bytes

**Security risk:** Sensitive information exchanged through plaintext communication can be intercepted and read.

### Lab 5: Finding Hidden Information in HTTP Traffic

**Objective:** Examine HTTP responses for information that is not visible in a browser.

**Findings:**
- A hidden note was discovered in `/staff.html`.
- The information was stored inside an HTML comment.
- HTTP response: 200 OK

**Security risk:** HTML comments can accidentally expose sensitive internal information.

### Lab 6: Investigating Exposed Login Credentials

**Objective:** Analyse a login submitted through an unencrypted web application.

**Findings:**
- Protocol: HTTP
- Request method: POST
- Login endpoint: `/login`
- Form encoding: application/x-www-form-urlencoded

**Security risk:** HTTP can expose usernames and passwords in plaintext.

**Recommendation:** Use HTTPS to encrypt web traffic.

### Lab 7: Detecting an FTP Brute-Force Attack

**Objective:** Investigate repeated failed FTP login attempts.

**Findings:**
- Attacker IP: 192.168.10.66
- Target FTP server: 192.168.10.20
- Targeted username: admin
- Failed login response: 530
- Successful login response: 230

**Security risk:** Repeated password attempts may allow attackers to gain unauthorised access.

**Recommendation:** Apply account lockout policies, rate limiting and secure authentication.

### Lab 8: Investigating VoIP Traffic

**Objective:** Analyse a voice call captured in network traffic.

**Findings:**
- SIP was used to establish the call.
- RTP carried the voice traffic.
- The caller's extension was 101.
- The call audio could be reconstructed from the capture.

**Security risk:** Unencrypted voice traffic may be intercepted.

**Recommendation:** Protect voice communication using SRTP.

## Key Takeaways

Through these investigations, I developed practical experience in:

1. Identifying suspicious network behaviour.
2. Analysing packets and TCP flags.
3. Following TCP streams to reconstruct communications.
4. Investigating exposed credentials.
5. Recognising brute-force attacks.
6. Understanding the importance of encryption.
7. Documenting security findings and recommending mitigations.

## Disclaimer

All investigations were conducted using simulated network traffic in an authorised cybersecurity training environment. IP addresses and findings belong to the training scenarios.

## Training

NetworkWalks - SOC Analyst Wireshark Labs
