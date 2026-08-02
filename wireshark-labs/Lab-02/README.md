# 🧪 Lab 02 - DNS Traffic Analysis with Wireshark

## 📌 Objective

Analyze DNS traffic using Wireshark to understand how a client resolves a domain name into an IPv4 address.

---

## 🛠️ Tools Used

- Wireshark
- DNS Protocol
- PCAPNG Capture File

---

## 🔍 Display Filter

```text
dns
```

---

## 📸 Evidence

### DNS Traffic

> Display filter showing only DNS packets.

*(Insert screenshot: dns-filter.png)*

### DNS Query and Response

> DNS query requesting the IPv4 address of `dns.google` and the corresponding response from the DNS server.

*(Insert screenshot: dns-query-response.png)*

---

## 📊 Packet Analysis

### Client Information

| Item | Value |
|------|-------|
| Client IP | 192.168.0.13 |
| DNS Server | 8.8.4.4 |
| Protocol | DNS |

---

### DNS Query

The client sends a DNS query requesting the IPv4 address of the domain:

- **Domain:** `dns.google`
- **Record Type:** A
- **Class:** IN

This query asks the DNS server to resolve the hostname into an IPv4 address.

---

### DNS Response

The DNS server replies with the following IPv4 addresses:

- **8.8.4.4**
- **8.8.8.8**

These addresses allow the client to establish communication with the requested host.

---

## 📚 What I Learned

- How DNS resolves hostnames into IPv4 addresses.
- How to filter DNS traffic in Wireshark.
- How to identify DNS queries and responses.
- How to interpret DNS packet fields.
- How to identify the client and DNS server involved in the communication.

---

## ✅ Conclusion

This lab demonstrated the complete DNS name resolution process. Using Wireshark, it was possible to observe how a client requests the IPv4 address of a domain and how the DNS server responds with the corresponding IP addresses.

Understanding DNS traffic is a fundamental networking skill and an essential step toward network troubleshooting and cybersecurity analysis.
