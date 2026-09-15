# VLANIF Inter-VLAN Communication Lab

## 📌 Overview
This lab focuses on enabling communication between different VLANs using **VLANIF interfaces** on Huawei network devices. It demonstrates how Layer 3 VLAN interfaces can be used to provide routing between separate, isolated VLAN networks.

---

## 🎯 Objectives
*   Create and configure multiple VLANs.
*   Configure VLANIF interfaces.
*   Assign IP addresses to VLANIF interfaces.
*   Enable communication between different VLANs.
*   Verify inter-VLAN connectivity.

---

## 🛠️ Tools
*   **Huawei eNSP** (Enterprise Network Simulation Platform)
*   **Huawei Switches** (S5700 or equivalent L3 Switches)
*   **Huawei VRP CLI** (Versatile Routing Platform)

---

## 💡 Skills Practiced
*   VLAN configuration
*   VLANIF configuration
*   Inter-VLAN routing
*   IPv4 addressing
*   Layer 3 switching
*   Connectivity testing
*   Troubleshooting

---

## 📐 Topology & Configuration (Suggested Reference)

| Device | Interface | VLAN | IP Address | Subnet Mask |
| :--- | :--- | :--- | :--- | :--- |
| **Switch-L3** | VLANIF 10 | VLAN 10 | *e.g., 192.168.10.1* | 255.255.255.0 |
| **Switch-L3** | VLANIF 20 | VLAN 20 | *e.g., 192.168.20.1* | 255.255.255.0 |
| **PC-1** | Ethernet 0/0/1 | VLAN 10 | *e.g., 192.168.10.10* | 255.255.255.0 |
| **PC-2** | Ethernet 0/0/2 | VLAN 20 | *e.g., 192.168.20.10* | 255.255.255.0 |

---

## 🔍 Verification & Troubleshooting
Connectivity between the configured VLANs was verified using network ping tests and Huawei CLI verification commands.

### Key Verification Commands
```shell
# Check the status and IP configuration of VLANIF interfaces
display ip interface brief

# View the active routing table to verify inter-VLAN routes
display ip routing-table

# View VLAN assignment and interface status
display vlan
```

---

## 📂 Evidence
The screenshots and project files included in this repository folder demonstrate the following:
1. Network topology architecture.
2. Device running configurations (VLAN & VLANIF).
3. Successful end-to-end `ping` connectivity verification.

---

## 🔑 Key Takeaway
This lab provided practical experience implementing inter-VLAN communication using VLANIF interfaces. It highlights the importance and efficiency of Layer 3 switching over traditional router-on-a-stick methodologies in enterprise networks.
