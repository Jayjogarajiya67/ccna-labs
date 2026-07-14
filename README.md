# 📘 CCNA Labs

Hands-on CCNA labs covering networking fundamentals, routing, switching, VLANs, NAT, ACLs, and troubleshooting — built for **CCNA 200-301 exam practice** using Cisco Packet Tracer.

---

## 🚀 Overview

This repository is a structured collection of **Cisco Packet Tracer (.pkt)** labs, each targeting one core CCNA topic. The goal is to move beyond theory and get real practice configuring, verifying, and troubleshooting Cisco devices in a simulated environment — the same skill set tested in the CCNA 200-301 exam.

Each lab is self-contained: open the `.pkt` file, and you'll find a pre-built topology (routers, switches, PCs) ready for configuration. Where available, a matching write-up in `labs-summaries/` explains the objective, the commands used, and how to verify the result.

---

## 🛠️ Prerequisites

| Requirement | Details |
|---|---|
| Software | Cisco **Packet Tracer v8.x** or higher (free via Cisco Networking Academy / Skills for All) |
| Knowledge | Basic networking fundamentals (IP addressing, subnetting, OSI model) |
| CLI | Familiarity with Cisco IOS CLI (enable mode, config mode, `show` commands) |
| Optional | A CCNA 200-301 study guide or Cisco's official exam topics list for cross-reference |

---

## 📂 Repository Structure

```
ccna-labs/
├── imgs/                          # Diagrams & screenshots
├── labs-summaries/                # Short notes & explanations per lab
├── AccessControlList(Extend).pkt
├── AccessControlList(Standard).pkt
├── BackupRouter'sConfigrations.pkt
├── CiscoDiscoveryProtocol(CDP).pkt
├── Dynamic-Host-Configuration-Protocol(DHCP)...pkt
├── FrameRelayProtocol(WAN).pkt
├── IPv6Routing(RIP).pkt
├── Inter-VIAN-Routing(RouterOnAStick).pkt
├── Overload-NAT.pkt
├── RecoverRouter'sPassword.pkt
├── RouterCommands.pkt
├── Routing(EIGRP-Protocol).pkt
├── Routing(OSPF-Protocol).pkt
├── Routing(RIP-Protocol).pkt
├── SecureSwitchFromMacFlooding(Sticky).pkt
├── SecureSwitchFromMacFlooding(Static).pkt
├── SecureSwitchFromMacFlooding.pkt
├── Static-NAT.pkt
├── StaticRoute.pkt
├── SwitchCommands.pkt
├── Telnet&DNS.pkt
├── Traditional-Inter-VLAN-Routing.pkt
├── VLAN-1.pkt
├── VLAN-2(With Trunk).pkt
├── VTP-Protocol.pkt
├── Wireless-Network.pkt
├── point-to-point(WAN-Protocol).pkt
├── LICENSE
└── README.md
```

---

## 🧪 Lab Topics — Detailed Breakdown

### 🔀 Routing
| Lab | What it covers |
|---|---|
| `Routing(RIP-Protocol).pkt` | Configuring RIP (v1/v2) between multiple routers, verifying routing tables |
| `Routing(EIGRP-Protocol).pkt` | EIGRP configuration, autonomous system numbers, neighbor verification |
| `Routing(OSPF-Protocol).pkt` | Single/multi-area OSPF, router IDs, `show ip ospf neighbor` verification |
| `IPv6Routing(RIP).pkt` | RIPng basics for IPv6 networks |
| `StaticRoute.pkt` | Manually configured static routes, default routes |

### 🔁 Switching & VLANs
| Lab | What it covers |
|---|---|
| `VLAN-1.pkt` | Creating and assigning VLANs to switch ports |
| `VLAN-2(With Trunk).pkt` | Trunk links between switches, tagging with 802.1Q |
| `Traditional-Inter-VLAN-Routing.pkt` | Inter-VLAN routing using multiple router interfaces |
| `Inter-VIAN-Routing(RouterOnAStick).pkt` | Router-on-a-stick using sub-interfaces on a single physical link |
| `VTP-Protocol.pkt` | VLAN Trunking Protocol — server/client/transparent modes |
| `SecureSwitchFromMacFlooding.pkt` / `(Static).pkt` / `(Sticky).pkt` | Port security configurations to prevent MAC flooding attacks, comparing static vs. sticky MAC learning |

### 🌐 WAN Protocols
| Lab | What it covers |
|---|---|
| `FrameRelayProtocol(WAN).pkt` | Frame Relay configuration between routers over a simulated WAN cloud |
| `point-to-point(WAN-Protocol).pkt` | PPP encapsulation, authentication (PAP/CHAP) |

### 🧰 Network Services
| Lab | What it covers |
|---|---|
| `Dynamic-Host-Configuration-Protocol(DHCP)...pkt` | DHCP server configuration on a router, address pools, exclusions |
| `Static-NAT.pkt` | One-to-one static NAT translation |
| `Overload-NAT.pkt` | NAT overload (PAT) — many private IPs sharing one public IP |
| `Telnet&DNS.pkt` | Remote access via Telnet, basic DNS setup |

### 🔐 Security & Access Control
| Lab | What it covers |
|---|---|
| `AccessControlList(Standard).pkt` | Standard ACLs — filtering by source IP |
| `AccessControlList(Extend).pkt` | Extended ACLs — filtering by source/destination IP, protocol, and port |

### 🛠️ Device Management & Troubleshooting
| Lab | What it covers |
|---|---|
| `RouterCommands.pkt` | Core IOS commands for router configuration and verification |
| `SwitchCommands.pkt` | Core IOS commands for switch configuration and verification |
| `CiscoDiscoveryProtocol(CDP).pkt` | Using CDP to discover directly connected Cisco devices |
| `BackupRouter'sConfigrations.pkt` | Backing up and restoring router configs (TFTP/copy commands) |
| `RecoverRouter'sPassword.pkt` | Password recovery procedure via ROMMON |

### 📡 Wireless
| Lab | What it covers |
|---|---|
| `Wireless-Network.pkt` | Basic wireless router/AP setup, SSID, security (WPA2), client connectivity |

---

## 🎯 Mapping to CCNA 200-301 Exam Domains

| Exam Domain | Related Labs |
|---|---|
| 1.0 Network Fundamentals | VLAN-1, VLAN-2, Wireless-Network |
| 2.0 Network Access | VLAN-2(Trunk), VTP-Protocol, SecureSwitchFromMacFlooding(*) |
| 3.0 IP Connectivity | StaticRoute, Routing(RIP/EIGRP/OSPF), IPv6Routing(RIP), Inter-VLAN Routing labs |
| 4.0 IP Services | DHCP, Static-NAT, Overload-NAT, Telnet&DNS |
| 5.0 Security Fundamentals | AccessControlList(Standard/Extend), Port Security labs |
| 6.0 Automation & Programmability | *(not covered — CLI-focused labs only)* |

---

## 📖 How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/JayJogariya67/ccna-labs.git
   ```
2. **Open a lab:** Launch Cisco Packet Tracer and open the desired `.pkt` file.
3. **Read the summary (if available):** Check `labs-summaries/` for the objective and expected outcome before diving in.
4. **Configure from scratch:** Try building the configuration yourself first — use the pre-built topology as the target, not the answer key.
5. **Verify:** Use `show` commands (`show ip route`, `show vlan brief`, `show ip interface brief`, etc.) to confirm your configuration matches expectations.
6. **Troubleshoot:** Intentionally break something (wrong VLAN, bad ACL, mistyped route) and practice diagnosing it — this mirrors real exam troubleshooting scenarios.

---

## 🤝 Contributing

Contributions are welcome — new labs, corrected configs, or better documentation all help.

1. Fork the repository
2. Create a branch: `git checkout -b add-new-lab`
3. Commit your changes with a clear message
4. Open a Pull Request describing what the lab covers

---

## 📜 License

Licensed under the **MIT License** — see [LICENSE](./LICENSE) for full terms.

---

## 👤 Author

**Jay Jogaraiya**
Cybersecurity Student · CCNA Learner

If this repo helped you study, consider giving it a ⭐ — it helps others find it too.
