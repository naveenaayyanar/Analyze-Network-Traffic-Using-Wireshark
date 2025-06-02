 Analyze-Network-Traffic-Using-Wireshark
 🛡️ Network Traffic Analysis – Task 5 (Cyber Security Internship)

 🎯 Objective
Capture and analyze live network traffic using Wireshark to identify key network protocols and understand packet-level communication.



 🧰 Tools Used
- Wireshark (Network packet analyzer)
- Kali Linux Terminal (For traffic generation via ping, browser)



 🔄 Steps Performed

1. Launched Wireshark and selected the active network interface.
2. Started packet capture.
3. Generated traffic:
   - Opened websites (e.g., Mozilla, Google).
   - Used `ping` command to test ICMP packets.
4. Stopped capture after ~1 minute and saved the file as `network_capture.pcap`.
5. Filtered traffic using protocol filters:
   - `dns`, `tcp`, `icmp`, `http`
6. Analyzed packets and recorded observations.
7. Captured screenshots of protocol details.
8. Created this summary report.



 📡 Protocols Identified & Observations

 1. DNS (Domain Name System)
- Translates domain names to IP addresses.
- DNS A and AAAA queries seen to domains like `contile.services.mozilla.com`.

 2. TCP (Transmission Control Protocol)
- Connection-oriented communication.
- Three-way handshake (SYN, SYN-ACK, ACK) observed.
- Secure connections to servers over port 443 (TLS).

 3. ICMP (Internet Control Message Protocol)
- Used for diagnostics (ping).
- `ping www.google.com` showed successful replies (~55ms).
- Ping to `104.19.230.21` failed with "port unreachable" — likely filtered.

 4. HTTP/OCSP (Online Certificate Status Protocol)
- OCSP used to verify SSL certificate status during HTTPS sessions.
- Responses from servers like `23.53.120.229` were logged.



 📁 Files Included
- `network_capture.pcap` – Wireshark capture file
- `dns.jpg` – DNS traffic screenshot
- `tcp.jpg` – TCP packet screenshot
- `icmp.jpg` – ICMP traffic screenshot
- `http.jpg` – HTTP/OCSP request screenshot
- `ping server.jpg` – Terminal output of `ping` command
- `Steps to do` – Before analysis what are the steps



 📘 Key Learnings
- Understood how to capture live traffic with Wireshark.
- Learned to isolate and analyze specific protocols.
- Gained practical exposure to TCP/IP behavior and diagnostics.
- Observed real-world DNS, HTTPS, and ping traffic patterns.

