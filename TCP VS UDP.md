# TCP VS UDP

Both **TCP (Transmission Control Protocol)** and **UDP (User Datagram Protocol)** are transport layer protocols in networking, but they are used in different scenarios based on reliability, speed, and use cases.

---
## **TCP (Transmission Control Protocol)**

🔹 **Where We Use TCP:**

- **Web Browsing (HTTP/HTTPS)** – Ensures full page loading without missing data.
- **File Transfers (FTP, SFTP, SCP)** – Requires reliability and data integrity.
- **Emails (SMTP, IMAP, POP3)** – Ensures complete delivery.
- **Remote Login (SSH, Telnet)** – Needs reliable data exchange.
- **Database Communication (MySQL, PostgreSQL, etc.)** – Prevents data corruption.

🔹 **Why We Use TCP:**  
✅ **Reliable:** Ensures all data packets arrive.  
✅ **Error Checking & Correction:** Resends lost packets.  
✅ **Ordered Delivery:** Maintains correct sequence.  
✅ **Connection-Oriented:** Establishes a connection before data transfer.  
🚫 **Slower:** Due to acknowledgment and retransmission overhead.

📌 **Example: TCP Socket (C Code)**

```c
sockfd = socket(AF_INET, SOCK_STREAM, 0);  // TCP uses SOCK_STREAM
```

---
## **2️⃣ UDP (User Datagram Protocol)**

🔹 **Where We Use UDP:**

- **Live Streaming (YouTube, Twitch, Netflix, etc.)** – Prioritizes speed over reliability.
- **Online Gaming (PUBG, CS:GO, etc.)** – Fast data exchange without waiting for acknowledgments.
- **VoIP Calls (Skype, Zoom, WhatsApp Calls, etc.)** – Latency-sensitive applications.
- **DNS Requests (Domain Name System)** – Fast response required without establishing a connection.
- **DHCP (Dynamic Host Configuration Protocol)** – Sends data without waiting for confirmation.

🔹 **Why We Use UDP:**  
✅ **Faster:** No connection setup or acknowledgment.  
✅ **Lightweight:** Less overhead compared to TCP.  
✅ **Efficient for real-time applications.**  
🚫 **Unreliable:** No guarantee of delivery.  
🚫 **No Ordering:** Packets may arrive out of sequence.

📌 **Example: UDP Socket (C Code)**

```c
sockfd = socket(AF_INET, SOCK_DGRAM, 0);  // UDP uses SOCK_DGRAM
```

---

### **⚖️ TCP vs UDP Summary Table**

|Feature|TCP (Reliable)|UDP (Fast)|
|---|---|---|
|Connection|Connection-oriented|Connectionless|
|Speed|Slower (due to reliability)|Faster (no overhead)|
|Reliability|High (error checking, retransmission)|Low (no acknowledgment)|
|Ordering|Yes (data arrives in order)|No (packets can arrive in any order)|
|Use Case|Web browsing, file transfer, emails, SSH|Streaming, gaming, VoIP, DNS|
