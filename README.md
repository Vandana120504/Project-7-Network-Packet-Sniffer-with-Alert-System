# Project-7-Network-Packet-Sniffer-with-Alert-System


A Python-based real-time packet sniffer with anomaly detection and traffic visualization, built for ethical network monitoring and intrusion detection.

# Features
- Captures live TCP/UDP/IP packets using **Scapy**
- Logs packet details (timestamp, source/destination IP, protocol, length) to **SQLite**
- Detects suspicious activity like **port scanning** and **DoS/flooding attempts**
- Visualizes top IP addresses based on traffic volume using **Matplotlib**
- Runs on **Kali Linux** with a CLI-based interface and optional graphing script

## Tools & Libraries Used
- Python 3
- [Scapy]
- SQLite3 (built-in)
- [Matplotlib]

## Project Structure
packet_sniffer_project/
├── sniffer.py         # Main packet sniffer and anomaly detector
├── graph.py           # Traffic visualizer for top source IPs
└── packets.db         # SQLite database storing packet logs

## How to Run
### 1. Install dependencies (Kali Linux):
sudo apt update
sudo apt install python3-scapy python3-matplotlib sqlite3

### 2. Run the sniffer:
sudo python3 sniffer.py

### 3. Visualize traffic:
python3 graph.py

## Example Output
Captured: 192.168.1.5 -> 192.168.1.1 [TCP] (60 bytes)
[!] Potential Port Scan Detected on Port 80
[!] Possible DDoS or flooding from 192.168.1.5

## Future Improvements
- Add email alerts on detection
- GUI for real-time live traffic monitoring
- Export packet logs to CSV
- GeoIP lookup for source IPs

![IMG-20250613-WA0013](https://github.com/user-attachments/assets/73a65d5e-56ae-4a0c-a470-b83879ea47bb)
![IMG-20250613-WA0011](https://github.com/user-attachments/assets/57c489bf-24dc-4c3d-9d31-e074d62ad537)
![IMG-20250613-WA0009](https://github.com/user-attachments/assets/ff9ff9b6-a0e9-40c1-a5c4-434a6bcb964f)
![IMG-20250613-WA0015](https://github.com/user-attachments/assets/ae348e3b-f19f-4163-b37e-bb043e23780c)
![IMG-20250613-WA0012](https://github.com/user-attachments/assets/6f4afcd7-af55-4e08-b676-3b8e7887fc65)



Created by [Vandana S] for Internship Phase Project – Cybersecurity (June 2025)
