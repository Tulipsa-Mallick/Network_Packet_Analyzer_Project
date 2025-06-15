 🧠 Network Packet Analyzer

A feature-rich **command-line-based Network Packet Analyzer** built using Python and Scapy. This tool allows you to capture real-time packets, apply intelligent filters, log packet data for analysis, generate test packets, and visualize protocol distribution — all in one interface.

---

## 📌 Key Features

✨ **Live Packet Sniffing**  
Capture real-time TCP, UDP, and ICMP traffic on your network interface.

🔍 **Filter by Protocol or IP Address**  
Apply protocol-based (TCP, UDP, ICMP) or IP address filters to isolate specific traffic patterns.

📝 **Logging (Text + CSV)**  
Captured packets are logged both in a human-readable .txt file and in a structured .csv format for later analysis.

🧪 **Test Packet Generation**  
Simulate TCP, UDP, and ICMP packets for testing and demonstration purposes without relying on external traffic.

📊 **Protocol Summary Visualization**  
Generate graphs showing protocol distribution using Matplotlib for better understanding of traffic patterns.

👀 **View Logged Data**  
Instantly display stored logs within the terminal using built-in log viewer.

🎨 **Color-Coded CLI**  
Enhanced user experience through colorama-based colorful terminal interface.

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries:**
  - [scapy](https://scapy.net) – For packet capture and manipulation
  - [colorama](https://pypi.org/project/colorama/) – For colored terminal output
  - [matplotlib](https://matplotlib.org/) – For plotting protocol summaries
  - csv, os, datetime – Python standard libraries for logging and data handling

---

## 🧾 Installation

### ✅ Prerequisites

- Python 3.8+
- **Windows Users:** Install [Npcap](https://nmap.org/npcap/) (required for packet sniffing)

### 📦 Install Required Packages
pip install -r requirements.txt

---

## 📂 File Structure

network_packet_analyzer_project/
│
├── main.py                  # Main menu (entry point)
├── packet_sniffer.py        # Live packet capture
├── filters.py               # Protocol/IP filters
├── logger.py                # Text and CSV logging
├── data_viewer.py           # CLI-based log viewer
├── plot_graph.py            # Visualize protocol summary
├── test_packets.py          # Generate sample packets
│
├── packet_log.txt           # Text log of packets
├── packet_log.csv           # CSV log of packets
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation

---

## 📈 Usage

### 🚀 Run the Application
python main.py


### 🧭 Menu Options

==================================================
           NETWORK PACKET ANALYZER
==================================================

Options:
1. Start Packet Sniffing
2. Apply Protocol Filter
3. Apply IP Filter
4. View Logged Packets
5. Plot Protocol Summary
6. Generate Test Packets
7. Exit

### 🛡️ Permissions Note

Packet sniffing may require administrative privileges:

* On Windows: Run your terminal as Administrator
* On Linux/macOS: Use sudo python3 main.py

---

## 📊 Example: Visual Output

The protocol summary graph (option 5) gives you an overview of traffic distribution:

* Bar graph of TCP vs UDP vs ICMP packets
* Auto-generated using your logged packet data

---

Sure! Here's an alternate example you can use **instead of the test packets section**, showcasing a real-world **sniffing and logging session** instead:

---

### 🧪 Example: Packet Sniffing in Action

When you select option **1**, the analyzer begins sniffing live packets from your active network interface. Here’s what a typical session might capture:

* **TCP**: 192.168.0.100 → 172.217.160.142 (user accessing Google via port 443)
* **UDP**: 192.168.0.101 → 8.8.8.8 (DNS query to Google’s DNS server)
* **ICMP**: 192.168.0.102 → 192.168.0.1 (ping to default gateway)

Captured packets are:

* Displayed live in the terminal with source/destination and protocol
* Logged automatically into:

  * packet_log.txt (for readable logs)
  * packet_log.csv (for structured analysis/graphing)

This helps in network analysis, diagnostics, and educational demos.

---

## 📜 License

This project is licensed under the MIT License.
Feel free to use, modify, and share!

# Network_Packet_Analyzer_Project
