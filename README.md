<div align="center">

```
██████╗ ███████╗███╗   ██╗████████╗███████╗███████╗████████╗
██╔══██╗██╔════╝████╗  ██║╚══██╔══╝██╔════╝██╔════╝╚══██╔══╝
██████╔╝█████╗  ██╔██╗ ██║   ██║   █████╗  ███████╗   ██║   
██╔═══╝ ██╔══╝  ██║╚██╗██║   ██║   ██╔══╝  ╚════██║   ██║   
██║     ███████╗██║ ╚████║   ██║   ███████╗███████║   ██║   
╚═╝     ╚══════╝╚═╝  ╚═══╝   ╚═╝   ╚══════╝╚══════╝   ╚═╝   
```

# Nvsncis · Security Researcher

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=00FF41&width=600&lines=Breaking+apps+before+attackers+do.;Android+%7C+Web+%7C+Network+Security.;Authorized+engagements+only.)](https://git.io/typing-svg)

![Profile Views](https://komarev.com/ghpvc/?username=0xpentest&color=00ff41&style=flat-square)
![Status](https://img.shields.io/badge/Status-Available%20for%20contracts-00ff41?style=flat-square)
![Location](https://img.shields.io/badge/Location-Bishkek%2C%20KG-blue?style=flat-square)

</div>

-----

## `whoami`

```bash
$ cat /etc/profile.d/researcher.sh

NAME="Security Researcher"
FOCUS="Android · Web APIs · Network Infrastructure"
METHOD="Hands-on exploitation + reverse engineering"
RULE="Contract first. Always."
STATUS="Open to pentest engagements"
```

> I break Android apps, web APIs, and networks by exploiting real-world misconfigurations.  
> My work combines **reverse engineering** with **dynamic analysis** to uncover practically exploitable vulnerabilities.  
> **Authorized engagements only.**

-----

## `cat focus_areas.txt`

<table>
<tr>
<td width="33%">

### 📱 Android Security

```
✓ APK reverse engineering
  └─ Smali / Java decompilation
  └─ Native .so library analysis

✓ Runtime bypass techniques
  └─ SSL Pinning bypass
  └─ Root detection bypass
  └─ Integrity / anti-tamper bypass

✓ Data exposure analysis
  └─ Insecure local storage
  └─ Sensitive data in logs/memory
```

</td>
<td width="33%">

### 🌐 Web & API Security

```
✓ Injection attacks
  └─ SQLi: Union / Blind / Time-based
  └─ XSS: Stored / Reflected / DOM

✓ Access control flaws
  └─ IDOR / BOLA
  └─ Business logic exploitation
  └─ Broken authentication

✓ API-specific testing
  └─ REST / GraphQL endpoints
  └─ JWT manipulation
  └─ Mass assignment
```

</td>
<td width="33%">

### 📡 Network & Wireless

```
✓ Active interception
  └─ MITM in misconfigured nets
  └─ Evil Twin attacks
  └─ ARP spoofing

✓ Wireless exploitation
  └─ Handshake capture
  └─ Deauthentication attacks
  └─ WPA2 cracking

✓ Traffic analysis
  └─ Protocol dissection
  └─ Credential sniffing
  └─ Network mapping
```

</td>
</tr>
</table>

-----

## `ls -la /tools`

```python
arsenal = {
    "Mobile & RE":      ["Frida", "JADX", "ApkTool", "Ghidra"],
    "Web & Network":    ["Burp Suite Pro", "Mitmproxy", "SQLMap", "Nmap"],
    "Wireless":         ["Aircrack-ng", "Wireshark", "Hostapd-wpe"],
    "OSINT":            ["theHarvester", "Shodan", "Maltego", "Subfinder"],
    "Exploitation":     ["Metasploit", "Impacket", "CrackMapExec"],
    "Scripting":        ["Python3", "Bash"],
    "Environment":      ["Kali Linux", "Android Studio", "Genymotion"],
}

for category, tools in arsenal.items():
    print(f"[+] {category}: {', '.join(tools)}")
```

```
[+] Mobile & RE: Frida, JADX, ApkTool, Ghidra
[+] Web & Network: Burp Suite Pro, Mitmproxy, SQLMap, Nmap
[+] Wireless: Aircrack-ng, Wireshark, Hostapd-wpe
[+] OSINT: theHarvester, Shodan, Maltego, Subfinder
[+] Exploitation: Metasploit, Impacket, CrackMapExec
[+] Scripting: Python3, Bash
[+] Environment: Kali Linux, Android Studio, Genymotion
```

-----

## `cat methodology.md`

```
┌─────────────────────────────────────────────────────────────┐
│                    PENTEST METHODOLOGY                      │
├──────────────┬──────────────────────────────────────────────┤
│  Phase 1     │  Reconnaissance & OSINT                      │
│              │  └─ Passive recon, subdomains, leaked creds  │
├──────────────┼──────────────────────────────────────────────┤
│  Phase 2     │  Scanning & Enumeration                      │
│              │  └─ Port scan, service fingerprinting        │
├──────────────┼──────────────────────────────────────────────┤
│  Phase 3     │  Exploitation                                │
│              │  └─ Vulnerability identification & attack    │
├──────────────┼──────────────────────────────────────────────┤
│  Phase 4     │  Post-Exploitation                           │
│              │  └─ Privilege escalation, lateral movement   │
├──────────────┼──────────────────────────────────────────────┤
│  Phase 5     │  Reporting                                   │
│              │  └─ Risk-rated findings with PoC & remediation│
└──────────────┴──────────────────────────────────────────────┘
```

-----

## `cat sample_findings.txt`

> ⚠️ All findings below were discovered during **authorized engagements**. Details are intentionally redacted.

```
[CRITICAL] SQL Injection → Database exfiltration
  Target:   Web application (financial sector)
  Method:   Time-based blind SQLi via login endpoint
  Impact:   Full database dump including user credentials
  Status:   Reported & patched ✓

[HIGH] SSL Pinning Bypass → Traffic Interception  
  Target:   Android banking application
  Method:   Frida hook on certificate validation
  Impact:   Plaintext API traffic exposed, tokens captured
  Status:   Reported & patched ✓

[HIGH] IDOR → Unauthorized Account Access
  Target:   Web API (e-commerce platform)
  Method:   Sequential user ID enumeration
  Impact:   Access to any user's personal & payment data
  Status:   Reported & patched ✓

[MEDIUM] Evil Twin → Credential Harvesting
  Target:   Corporate wireless network (physical assessment)
  Method:   Rogue AP + captive portal
  Impact:   Employee credentials captured
  Status:   Reported & remediated ✓
```

-----

## `./engage.sh`

```bash
#!/bin/bash
# How to work with me

echo "[*] Scope definition & NDA signing"
echo "[*] Contract & payment terms agreement"  
echo "[*] Technical kick-off call"
echo "[*] Engagement execution"
echo "[*] Detailed report delivery with remediation guidance"
echo "[*] Free retest after fixes"
echo ""
echo "[+] Ready to start? See contacts below."
```

-----

## `ifconfig contacts`

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-Nevskiy-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/nvsncis)
[![Email](https://img.shields.io/badge/Email-click%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:alex2034@gmail.com)

</div>

-----

<div align="center">

```
[ NO CONTRACT = NO ENGAGEMENT ]
```

*All security research is conducted ethically and legally.*  
*Unauthorized testing is never performed.*

</div>