# 📊 Network Protocol Analysis Report

## 🎯 Capture Details
- **Tool Used:** Wireshark 4.2.0
- **Capture Duration:** 1 minute
- **Network Interface:** Wi-Fi/Ethernet
- **Total Packets Captured:** 150+
- **Capture File:** `network_capture.pcap`

## 🔍 Protocols Identified

### 1. DNS (Domain Name System)
**Purpose:** Translates domain names to IP addresses
**Observed Behavior:** 
- DNS queries for websites like google.com, github.com
- DNS responses with IP addresses
- Uses UDP protocol on port 53

### 2. TCP (Transmission Control Protocol)
**Purpose:** Reliable, connection-oriented data transmission
**Observed Behavior:**
- TCP three-way handshake (SYN → SYN-ACK → ACK)
- Sequence number tracking
- Flow control mechanisms
- Connection termination (FIN packets)

### 3. HTTP (Hypertext Transfer Protocol)
**Purpose:** Unencrypted web communication
**Observed Behavior:**
- HTTP GET requests for web pages
- HTTP 200 OK responses
- Clear text headers and data

### 4. TLS (Transport Layer Security)
**Purpose:** Encrypted web communication
**Observed Behavior:**
- TLS handshake process
- Encrypted application data
- Used by HTTPS websites

## 🛠️ Wireshark Filters Used
- `dns` - Show only DNS packets
- `tcp` - Show only TCP packets  
- `http` - Show only HTTP packets
- `tls` - Show only TLS packets
- `tcp.port == 80` - Show HTTP traffic
- `tcp.port == 443` - Show HTTPS traffic

## 📈 Key Observations
1. **Most traffic is encrypted** (TLS) for security
2. **DNS is one of the most common protocols** in background traffic
3. **TCP handshake occurs** before any data transfer
4. **HTTP is becoming less common** due to HTTPS adoption
   
