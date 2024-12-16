# Wireshark Network Analysis

## Objective

The objective of this project was to utilize Wireshark as a powerful network protocol analyzer to capture, filter, and analyze network traffic. The goal was to enhance the understanding of how data travels through a network, recognize patterns, detect anomalies, and identify potential security threats.

### Skills Learned

- Proficiency in using Wireshark for capturing live network traffic.
- Ability to apply filtering techniques to isolate relevant packets for analysis.
- Understanding of various network protocols and their normal behavior.
- Skills in identifying malicious traffic and potential indicators of compromise (IoCs).
- Enhanced analytical skills for interpreting packet data and deriving meaningful insights.

### Tools Used

- Wireshark: A leading network protocol analyzer for capturing and inspecting packets in real-time.
- Tcpdump: A command-line packet analyzer for capturing traffic for later analysis with Wireshark.
- Network Protocols: Familiarity with protocols such as TCP, UDP, HTTP, and DNS for comprehensive traffic analysis.

## Steps

### 1. Capture Network Traffic
- Start Wireshark and select the appropriate network interface to capture traffic.
  - Launched Wireshark and selected the appropriate network interface (e.g., Wi-Fi or Ethernet) to start capturing packets. Clicked on the interface and then clicked the "Start Capturing Packets" button.

- Findings: After capturing packets for a designated time, I observed traffic consisting of various protocols such as TCP, UDP, ARP, and ICMP. This initial capture set the stage for further analysis.

---

### 2. Apply Filters
- Use filters to focus on specific protocols or IP addresses.
  1. Filter for HTTP Traffic:
     ```bash
     http
  2. Filter for DNS Queries:
     ```bash
     dns

---

### 3. Analyze Captured Packets
- Inspect individual packets to understand the details, including source and destination addresses, protocols used, and payload data.
   - Follow TCP Stream: Right-click on a TCP packet and select "Follow" > "TCP Stream" to view the entire conversation between two hosts.

- Findings: While analyzing an HTTP stream, I discovered a successful login attempt with credentials exposed in plain text. This highlighted a significant security risk.

---

### 4. Identify Anomalies
- Look for unusual patterns or spikes in traffic that may indicate suspicious activity or potential cybersecurity threats.
   - Protocol Hierarchy Statistics: Accessed via Statistics > Protocol Hierarchy to visualize the distribution of protocols present in the capture.

- Findings: During the analysis, I noticed an unexpected spike in UDP traffic at certain times, suggesting possible unauthorized broadcasts or DDoS activity targeting specific services.

---

### 5. Document Findings
- Record observations and findings from the analysis to create a comprehensive report detailing any identified security concerns or anomalies. This included:
   - A summary of detected security threats (e.g., exposure of sensitive information).
   - Recommendations for mitigating risks such as enforcing HTTPS for web applications and implementing intrusion detection systems.


## Conclusion

This project not only provided practical experience with network analysis tools but also reinforced critical cybersecurity concepts essential for identifying and mitigating threats in real-world environments.
