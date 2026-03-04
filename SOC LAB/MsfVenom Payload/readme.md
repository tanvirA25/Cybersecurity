
# SOC Lab: Windows 11 + Kali Reverse Shell (msfvenom)

## Lab Objective
- Build a small SOC-style home lab on an M1 Mac
- Use Kali to generate a Windows malware payload with **msfvenom**
- Get a **Meterpreter** reverse shell on a Windows 11 VM
- Observe/prepare to observe activity with tools like Sysmon/Splunk later

---

## Lab Environment

**Host**
- macOS on Apple Silicon (M1)
- VMware Fusion

**Virtual Machines**
- Kali Linux (attacker)
- Windows 11 ARM (victim / SOC endpoint)

**Networking**
- Custom / host-only vmnet for lab traffic (no internet)
- Optional NAT adapter on Kali for updates

---

## Network Design & Isolation

- Kali and Windows on the **same host‑only vmnet**  
- Example lab subnet:
  - Kali: `192.168.51.129`
  - Windows: `192.168.51.128`
- Isolation controls:
  - No bridged adapter on Windows
  - No shared folders, drag‑and‑drop, or clipboard host‑integration
  - macOS protected by its own firewall and up‑to‑date hypervisor

---

## Connectivity Validation

**On Kali**
```bash
ip a                     # confirm IP, e.g. 192.168.51.129
ping 192.168.51.128      # ping Windows
nmap -sA 192.168.51.128 -Pn

