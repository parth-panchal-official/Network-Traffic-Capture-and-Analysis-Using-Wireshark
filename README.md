# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live packets, filter them, and identify protocols.

## Tools
- [Wireshark](https://www.wireshark.org/download.html)

## Steps
1. **Install Wireshark**  
   - Linux: `sudo apt install wireshark`
   - Windows/Mac: Download from official site.
2. **Start Capture**  
   - Open Wireshark → Select active interface → Click Start.
3. **Generate Traffic**  
   - Visit websites or run: `ping google.com`
4. **Stop Capture** after ~1 min.
5. **Filter & Identify Protocols**  
   - Use filters: `http`, `dns`, `tcp`
6. **Save Capture**  
   - File → Save As → `task5_capture.pcap`
7. **Report**  
   - List protocols, packet counts, and findings.

## Outcome
Understand packet capture, protocol filtering, and traffic analysis.

---

### 2. Start Capturing Packets

1. Launch Wireshark.
2. Select your **active network interface** (e.g., Ethernet, Wi-Fi).
3. Click **Start Capturing** (the blue shark fin icon).

---

### 3. Generate Network Traffic

* Open a browser and visit any website.
* OR run:

  ```bash
  ping google.com
  ```
* This will generate HTTP, DNS, and TCP packets.

---

### 4. Stop Capturing

* After about **1 minute**, click the **red stop button**.

---

### 5. Filter Captured Packets

* Use Wireshark filters to view specific protocols:

  * HTTP: `http`
  * DNS: `dns`
  * TCP: `tcp`

---

### 6. Identify Protocols

* Identify at least **three different protocols** from your capture.
* Example:

  * HTTP
  * DNS
  * TCP

---

### 7. Export the Capture

* Go to **File → Save As**
* Save the file as:

  ```
  task5_capture.pcap
  ```

---

### 8. Write the Report

Create a short report summarizing:

* **Protocols captured**
* **Packet count per protocol**
* **Any interesting findings**

Example report:

```
Captured Protocols:
- HTTP: 120 packets
- DNS: 30 packets
- TCP: 250 packets

Findings:
- HTTP requests to example.com
- DNS queries to 8.8.8.8
```

---

## Outcome

Hands-on experience in:

* Packet analysis
* Protocol identification
* Network traffic monitoring

---

## Example Commands for Linux Users

Start pinging to generate traffic:

bash
ping -c 5 google.com

Run Wireshark with root privileges (if needed):

'bash'
sudo wireshark
