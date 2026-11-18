# Diwali WhatsApp Phishing Kit — Threat Analysis

Dynamic analysis of a multi-stage phishing campaign distributed 
via WhatsApp targeting South Indian users during the 2026 Diwali 
festival period. Impersonates Airtel offering ₹2,000 cash reward.

## Key Findings
- Polymorphic JavaScript cloaking — evades all VirusTotal scanners
- WhatsApp OG tag spoofing — displays whatsapp.com as source domain
- Vue 3 SPA with full victim profiling and referral tree tracking
- Self-propagating worm engine requiring 19 forced WhatsApp shares
- WebSocket C2 backdoor with eval() remote code execution capability
- CPA ad fraud loop with 70% rigged rejection rate
- No reward ever delivered — dead-end payout by design

## Methodology
Static Analysis → VirusTotal reputation check  
Dynamic Analysis → Burp Suite interception inside isolated Kali VM  
JS Deobfuscation → Manual Base64 decoding and variable renaming analysis  
Infrastructure Mapping → Full IoC extraction across all five stages

## Tools Used
Burp Suite · Kali Linux · JavaScript Deobfuscation · Wireshark

## Live Report
👉 https://pixelized-exe.github.io/diwali-phishing-analysis/

> All analysis performed inside an isolated virtual machine.  
> No real credentials or data were submitted at any point.  
> All malicious domains written in defanged format.
