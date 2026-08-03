<div align="center">

<br>

<!-- ANIMATED STYLE HEADER -->
```ascii
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║    ██████╗ ██████╗  ██████╗     ███████╗██╗  ██╗████████╗██████╗  █████╗     ║
║    ██╔══██╗██╔══██╗██╔═══██╗    ██╔════╝╚██╗██╔╝╚══██╔══╝██╔══██╗██╔══██╗    ║
║    ██╔═══╝ ██╔══██╗██║   ██║    ██╔══╝   ██╔██╗    ██║   ██╔══██╗██╔══██║    ║
║    ██║     ██║  ██║╚██████╔╝    ███████╗██╔╝ ██╗   ██║   ██║  ██║██║  ██║    ║
║    ╚═╝     ╚═╝  ╚═╝ ╚═════╝     ╚══════╝╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝    ║
║                                                                              ║
║                       ⚡ EXTRACTION ENGINE v2.1 ⚡                          ║
║                                                                              ║
║  ⭐The Ultimate Automated Credential Extraction & Exploitation Framework⭐  ║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```
┌───────────────────────────────────────────────────────────────────────────── ┐
│                                                                              │
│   Pro ExtraFinder is a turnkey, end-to-end offensive framework that          │
│   automates the full credential-theft kill chain:                            │
│                                                                              │
│         DISCOVER  →  EXTRACT  →  VALIDATE  →  EXPLOIT  →  NOTIFY             │
│                                                                              │
│   It targets:                                                                │
│     • Misconfigured web servers leaking .env / .git / config files           │
│     • Secrets committed to public GitHub / GitLab repos (411 dorks)          │
│     • Unpatched enterprise apps (34 weaponized CVEs → auto-shell)            │
│     • Cloud metadata, JS bundles, archives, actuator endpoints               │
│     • Crypto wallets (ETH private keys, BTC WIF, BIP39 seeds)                │
│                                                                              │
│   Evasion:                                                                   │
│     • 3-layer WAF bypass (header spoof → path mutation → method rotate)      │
│     • 5 real browser fingerprints rotated per request                        │
│     • Proxy pool with auto health check + round-robin                        │
│     • 150ms rate limit per domain — stays under the radar                    │
│                                                                              │
│   Output:                                                                    │
│     • Only VALIDATED credentials reach your Telegram (80+ APIs tested)       │
│     • Persistent shells deployed on confirmed RCE targets                    │
│     • Full dedup — never see the same result twice, even after restart       │
│     • Runs for hours/days unattended. Set it and forget it.                  │
│                                                                              │
│   Single Go binary. Zero dependencies. 30,000+ lines. Built for scale.       │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────── ─┘
```

<br>

<table>
<tr>
<td align="center"><b>🎯 120+</b><br><sub>Paths/Domain</sub></td>
<td align="center"><b>💀 34</b><br><sub>CVEs Weaponized</sub></td>
<td align="center"><b>✅ 80+</b><br><sub>Auto-Validators</sub></td>
<td align="center"><b>🕵️ 411</b><br><sub>GitHub Dorks</sub></td>
<td align="center"><b>🛡️ 36</b><br><sub>WAF Bypasses</sub></td>
<td align="center"><b>🧵 5K</b><br><sub>Max Threads</sub></td>
</tr>
</table>

## 🎬 How It Works

```
  YOU                          PRO EXTRAFINDER                         YOU
  ───                          ───────────────                         ───

                    ┌────────────────────────────────┐
  domains.txt ───►  │                                │
                    │   ┌─────────┐   ┌──────────┐   │
  (or)              │   │  SCAN   │──►│ EXTRACT  │   │
                    │   │ 120+    │   │ Regex +  │   │        ╔════════════╗
  GitHub ─────────► │   │ paths   │   │ Context  │   │        ║            ║
                    │   └─────────┘   └────┬─────┘   │        ║  TELEGRAM  ║
  (or)              │                      │         │───────►║            ║
                    │              ┌───────▼────── ┐ │        ║ Only VALID ║
  IP ranges ──────► │              │   VALIDATE    │ │        ║  results   ║
                    │              │   80+ APIs    │ │        ║            ║
  (or)              │              │   tested live │ │        ╚════════════╝
                    │              └────────┬──────┘ │
  certstream ────►  │                       │        │        ╔════════════╗
                    │              ┌────────▼──────┐ │        ║            ║
                    │              │   EXPLOIT     │ │───────►║  resultat/ ║
                    │              │   34 CVEs     │ │        ║  files     ║
                    │              │   auto-shell  │ │        ║            ║
                    │              └───────────────┘ │        ╚════════════╝
                    │                                │
                    └────────────────────────────────┘

  ⏱️ Time: Set it up once. Let it run forever. Wake up to results.
```
## 💎 Why Clients Choose Pro ExtraFinder

### ❌ Without Pro ExtraFinder

- Run 10+ different tools manually
- Write custom scripts for each target
- Get thousands of dead/invalid results
- Lose progress when tools crash
- Miss secrets in git history & JS bundles
- Manually verify every credential
- No notifications — check results manually
- WAFs block you after 5 requests
- Spend hours on one target

### ✅ With Pro ExtraFinder

- **One command** does everything
- **120+ paths** scanned automatically
- **Only valid results** reach your Telegram
- **Auto-resume** — never lose progress
- **Deep scanning** — git packs, JS, archives
- **80+ validators** test every credential live
- **Real-time Telegram** alerts for valid hits
- **3-layer WAF bypass** keeps you undetected
- **5,000 threads** — scan 100K domains overnight


### 🏆 What You Get

┌──────────────────────────────────────────────────────────────────────── ─┐
│                                                                          │
│   ✅ Working AWS keys (with IAM access confirmed)                       │
│   ✅ Working SMTP accounts (SendGrid, Brevo, Mailgun, Mailjet...)       │
│   ✅ Working AI API keys (OpenAI, Anthropic, Groq, xAI...)              │
│   ✅ Working payment keys (Stripe, PayPal, Square...)                   │
│   ✅ Working cloud tokens (GitHub, GitLab, Slack, Discord...)           │
│   ✅ Working proxy credentials (25+ providers validated)                │
│   ✅ Working OSINT API keys (Shodan, Censys, VirusTotal...)             │
│   ✅ Crypto wallets with balance (ETH, BTC, BIP39 seeds)                │
│   ✅ Admin panel access (40+ bypass techniques)                         │
│   ✅ Deployed shells (auto-exploit 34 CVEs)                             │
│   ✅ Full .git history credentials (deleted secrets recovered)          │
│                                                                         │
│   All delivered to Telegram. All deduplicated. All validated.           │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

## ⚡ Feature Breakdown

### 📊 80+ Services — Extracted & Auto-Validated

> ⚠️ **Every credential is tested LIVE. Dead = discarded. Working = Telegram alert.**

| Category | Services |
|----------|----------|
| ☁️ **Cloud** | AWS Keys, Azure, GCP, Cloudflare, DigitalOcean, Supabase, Vault, Terraform, K8s |
| 📧 **Email/SMS** | SendGrid, Mailgun, Brevo, Twilio, Mailjet, Postmark, Resend, Plivo, Nexmo, SMTP |
| 🤖 **AI/LLM** | OpenAI, Anthropic, Groq, xAI, DeepSeek, Perplexity, Mistral, Cohere, ElevenLabs |
| 💳 **Payments** | Stripe, PayPal, Square |
| 🛠️ **DevOps** | GitHub, GitLab, Bitbucket, Slack, Discord, Telegram, Grafana, Datadog, Sentry |
| 🌐 **Proxies** | Smartproxy, BrightData, Oxylabs, IPRoyal + 20 more |
| 🔍 **OSINT** | Shodan, Censys, VirusTotal, Hunter.io, FOFA, ZoomEye + 10 more |
| 💰 **Crypto** | ETH private keys, BTC WIF, BIP39 seeds, Solana keys |

<br>

---

### 💀 CVE Auto-Exploitation — 34 Weaponized

> **Detects → Confirms → Exploits → Deploys shell. Zero human interaction.**

<br>

<details>
<summary><b>🔽 Click to expand all 34 CVEs</b></summary>
<br>

- [x] CVE-2021-3129 — **Laravel Ignition** → RCE + .env dump
- [x] CVE-2022-22965 — **Spring4Shell** → JSP/PHP shell deploy
- [x] CVE-2024-27198 — **TeamCity** → Auth bypass + all configs
- [x] CVE-2024-4040 — **CrushFTP** → Path traversal + file read
- [x] CVE-2024-40711 — **Veeam Backup** → Credential extraction
- [x] CVE-2024-21762 — **FortiOS** → SSL VPN config extract
- [x] CVE-2021-44228 — **Log4Shell** → JNDI + env dump
- [x] CVE-2017-9841 — **PHPUnit** → RCE + shell deploy
- [x] CVE-2023-23752 — **Joomla** → API disclosure + secrets
- [x] CVE-2024-23897 — **Jenkins** → File read + master.key
- [x] CVE-2021-43798 — **Grafana** → Path traversal + configs
- [x] CVE-2025-29927 — **Next.js** → Middleware bypass
- [x] CVE-2024-1709 — **ScreenConnect** → Auth bypass + RCE
- [x] CVE-2024-3400 — **PAN-OS** → PHP auth bypass
- [x] CVE-2024-24919 — **Check Point VPN** → File read
- [x] CVE-2024-40766 — **SonicWall** → VPN auth bypass
- [x] CVE-2024-8190 — **Ivanti CSA** → RCE
- [x] CVE-2024-20767 — **ColdFusion** → File read / RCE
- [x] CVE-2024-53677 — **Struts2** → OGNL injection
- [x] CVE-2024-4358 — **Telerik** → File upload / RCE
- [x] CVE-2024-50623 — **Cleo** → Groovy RCE
- [x] CVE-2024-28255 — **OpenMetadata** → Auth bypass
- [x] CVE-2023-22518 — **Confluence** → Auth bypass
- [x] CVE-2023-46604 — **ActiveMQ** → Protocol RCE
- [x] CVE-2025-47953 — **Langflow** → Component + shell
- [x] CVE-2025-31324 — **SAP NetWeaver** → Metadata RCE
- [x] CVE-2025-32432 — **Craft CMS** → Injection + shell
- [x] CVE-2025-0108 — **PAN-OS** → PHP bypass
- [x] CVE-2024-4577 — **PHP CGI (Win)** → Arg injection
- [x] CVE-2017-12617 — **Tomcat** → PUT shell upload
- [x] CVE-2017-5638 — **Struts2** → OGNL via headers
- [x] CVE-2024-21887 — **Ivanti Connect** → Cmd injection
- [x] CVE-2024-37085 — **VMware** → Auth bypass
- [x] CVE-2024-43090 — **mod_fcgid** → RCE

</details>

<br>

---

### 🛡️ Stealth & Evasion — 3 Layers

> **Stays undetected even against aggressive WAFs.**

╔══════════════════════════════════════════════════════════════════════════╗
║                                                                          ║
║   LAYER 1 — BROWSER FINGERPRINTING                                       ║
║   ┌──────────────────────────────────────────────────────────────────┐   ║
║   │ 5 real browser profiles rotated per request:                     │   ║
║   │   Chrome 120 · Firefox 121 · Safari 17 · Edge 120 · Chrome iOS   │   ║
║   │ + matching Accept, Accept-Language, Sec-CH-UA, Sec-Fetch-*       │   ║
║   └──────────────────────────────────────────────────────────────────┘   ║
║                                                                          ║
║   LAYER 2 — WAF BYPASS  (triggers on 403 / block)                        ║
║   ┌──────────────────────────────────────────────────────────────────┐   ║
║   │ Step 1: Header spoofing  —  12 IPs × 7 headers  =  84 combos     │   ║
║   │ Step 2: Path mutation    —  12 variants  (//path, /./path, %00)  │   ║
║   │ Step 3: Method bypass    —  POST · HEAD · OPTIONS · PUT · PATCH  │   ║
║   └──────────────────────────────────────────────────────────────────┘   ║
║                                                                          ║
║   LAYER 3 — INFRASTRUCTURE                                               ║
║   ┌──────────────────────────────────────────────────────────────────┐   ║
║   │ • Proxy pool with auto-health-check (drops dead nodes)           │   ║
║   │ • Round-robin rotation across all alive proxies                  │   ║
║   │ • 150 ms per-unique-domain rate limit                            │   ║
║   │ • Custom TLS CONNECT tunnel for HTTPS through HTTP proxies       │   ║
║   │ • Connection pooling + keep-alive management                     │   ║
║   └──────────────────────────────────────────────────────────────────┘   ║
║                                                                          ║
╚══════════════════════════════════════════════════════════════════════════╝

---

### 🕵️ GitHub Hunt — 411 Dork Queries

> **Automated credential hunting across all public GitHub repos.**

<br>

- [x] **411 Queries** — AWS · SMTP · AI keys · Git tokens · Slack · Crypto · CI/CD · Docker · K8s · Databases · Proxy · OSINT · Payment
- [x] **Token Pool** — Multi-token rotation · Auto rate limit detection · Pause + switch · Wait for reset
- [x] **Persistence** — Progress saved every query (crash-safe) · Deduped across sessions · Resumes where it stopped
- [x] **Deep Scan** — Downloads actual file content · Scans with credential regex · Not just search results

<br>

---

### 🔬 Advanced Scanning Modules

> **Beyond basic .env scanning — deep extraction from complex targets.**

<br>

- [x] **JS Bundle Analysis** — Extracts all `<script src>` from HTML, downloads each bundle (<20MB), scans minified code for embedded API keys, tokens, and connection strings
- [x] **Archive Scanner** — Detects exposed ZIP/TAR.GZ/JAR/WAR files, extracts and scans internal files (.env, .properties, .yml, credentials.json, private keys)
- [x] **HeapDump Extraction** — Downloads Spring Boot `/actuator/heapdump` (HPROF format), saves locally, extracts passwords/tokens/connection strings from JVM memory
- [x] **Git Pack Parsing** — Downloads `.git/objects/pack/*.idx` + `.pack`, parses fan-out tables, decompresses zlib objects, reconstructs **full commit history** — finds deleted credentials
- [x] **phpinfo() Scanner** — Extracts all sensitive variables from phpinfo HTML output, detects PHP version and maps to applicable CVEs
- [x] **SSRF to Cloud Metadata** — Tests `169.254.169.254` (IMDSv1) for EC2/GCP/Azure IAM tokens, user-data, instance profiles
- [x] **Spring Cloud Config** — Extracts property sources with credentials from exposed config endpoints
- [x] **Consul KV Dump** — Enumerates Consul key-value store for secrets, tokens, database credentials
- [x] **Elasticsearch Index Dump** — Lists indices, reads `_search` results, extracts credentials from indexed documents
- [x] **Docker API Extraction** — Connects to exposed Docker daemon (2375/2376), enumerates containers, reads `/proc/1/environ` for all env vars
- [x] **Kubernetes Secrets** — Accesses unauthorized K8s API, lists namespaces, reads secrets and configmaps
- [x] **WebDAV/NTLM Enum** — PROPFIND enumeration + NTLM authentication detection for relay attacks
- [x] **Hadoop/Spark** — Scans ResourceManager, NameNode JMX, Spark Environment for AWS keys in Hadoop XML configs

<br>

---

### 🌐 Web Security Scanners

> **Full web app assessment beyond credential extraction.**

<br>

- [x] **Admin Panel Finder** — Discovers admin/login panels across multiple CMS paths with response analysis
- [x] **CORS Misconfiguration** — Tests for wildcard origins, reflected origins, credential inclusion with arbitrary domains
- [x] **Cookie Security Audit** — Checks HttpOnly, Secure, SameSite flags, identifies session fixation risks
- [x] **Deep Web Crawler** — Recursive link extraction + JS URL discovery, configurable depth, with optional credential scanning on discovered pages
- [x] **Vulnerability Scanner** — SQLi (UNION/error-based), XSS (reflected/stored), LFI (path traversal + PHP filters), SSRF (internal access)
- [x] **Credential Validator** — Direct protocol testing: SSH, FTP, MySQL, PostgreSQL, Redis, MongoDB, Elasticsearch brute-force

<br>

---

### 🌍 Domain & Target Discovery

> **Multiple sources for finding new targets automatically.**

<br>

- [x] **CertStream** — Real-time WebSocket to Certificate Transparency logs, filters by keywords, optional auto-scan
- [x] **crt.sh** — Subdomain enumeration from CT logs with dedup + auto-scan integration
- [x] **Google Dorking** — Targeted dork queries for exposed configurations and credentials
- [x] **Multi-Source Harvest** — Combines 10+ OSINT sources (OTX, DNSDumpster, RapidDNS, HackerTarget, Wayback, URLScan, etc.)
- [x] **IP Scanner** — Scans official IP ranges from AWS/GCP/Azure/DO/Vultr/Hetzner/Oracle/Alibaba/Tencent, port scanning + service fingerprinting
- [x] **Random IP Generation** — Generates random public IPs and scans for web services
- [x] **SaaS Scoring** — Fingerprints and scores domains by technology stack, prioritizes high-value targets
- [x] **Cascade Mode** — SaaS scoring → prioritized envdump, scans best targets first
- [x] **S3 Bucket Scanner** — Generates bucket name variants from domain, lists contents, downloads credentials from open buckets (AWS, GCP, Azure, Oracle, DO)

<br>

---

### 📱 Remote Control & Export

> **Manage everything remotely, export in any format.**

<br>

- [x] **Telegram C2 Bot** — Full remote control: scan targets, receive results, upload domain lists, check stats, graceful shutdown
- [x] **Web Dashboard** — Real-time stats + results viewer on `http://localhost:8080` with authentication
- [x] **JSON Export** — `toolkit export-json output.json` — structured export of all results
- [x] **CSV Export** — `toolkit export-csv output.csv` — spreadsheet-compatible export
- [x] **Retro-Send** — `toolkit retro-send` — re-sends all validated results to Telegram (for missed notifications)
- [x] **Checkpoint/Resume** — All scan progress saved to disk, auto-resumes on restart from exact position
- [x] **Credential Dedup** — SHA256-based deduplication persisted across restarts, never processes same credential twice

<br>

---

### ⚔️ Manual Exploit Mode

> **Targeted exploitation with custom payloads.**

<br>

```bash
toolkit exploit --cve CVE-2017-9841 --target https://target.com --cmd "id"
toolkit exploit --cve CVE-2024-27198 --target https://target.com --add-user admin:pass
toolkit exploit --cve JENKINS-SCRIPT --target https://target.com --cmd "cat /etc/passwd"
toolkit exploit --cve CVE-2024-24919 --target https://target.com --file /etc/shadow
toolkit exploit --cve CVE-2024-4040 --target https://target.com --file /etc/passwd
```

| Flag | Purpose |
|------|---------|
| `--cve` | CVE identifier to exploit |
| `--target` | Target URL |
| `--cmd` | Command to execute (default: `id`) |
| `--add-user` | Create backdoor user (`user:pass`) |
| `--reverse-shell` | Reverse shell callback (`host:port`) |
| `--file` | File path to read from target |

<br>

---

## 📁 Output Structure

```
resultat/
│
│  ╔═══ RAW HITS (credentials found, pending validation) ═══╗
│  ║                                                          ║
├──╫── aws_hits.txt              AWS AKIA + Secret pairs       ║
├──╫── smtp_hits.txt             SMTP host:user:pass           ║
├──╫── sendgrid_hits.txt         SG.xxxxx keys                 ║
├──╫── brevo_hits.txt            xkeysib-xxxxx keys            ║
├──╫── twilio_hits.txt           ACsid:token pairs             ║
├──╫── mailgun_hits.txt          domain:key pairs              ║
├──╫── mailjet_hits.txt          public:secret pairs           ║
├──╫── api_keys_hits.txt         Generic API keys              ║
├──╫── github_tokens.txt         GitHub PATs discovered        ║
│  ║                                                          ║
│  ╚══════════════════════════════════════════════════════════╝
│
│  ╔═══ VALIDATED (confirmed working — sent to Telegram) ══════╗
│  ║                                                            ║
├──╫── aws_valid.txt             ✅ Working AWS keys           ║
├──╫── aws_backdoors.txt         ✅ IAM backdoors created      ║
├──╫── api_keys_valid.txt        ✅ Working API keys           ║
├──╫── mailjet_valid.txt         ✅ Working Mailjet            ║
├──╫── admin_panels_valid.txt    ✅ Confirmed admin access     ║
├──╫── eth_keys_valid.txt        ✅ ETH keys with balance      ║
├──╫── btc_wif_valid.txt         ✅ BTC keys validated         ║
├──╫── deepseek_valid.txt        ✅ Working DeepSeek keys      ║
│  ║                                                           ║
│  ╚═══════════════════════════════════════════════════════════╝
│
│  ╔═══ EXPLOITATION ══════════════════════════════════════════╗
│  ║                                                           ║
├──╫── git_hits.txt              Exposed .git repositories     ║
├──╫── rce_verified.txt          Confirmed RCE targets         ║
├──╫── deployed.txt              Shells successfully deployed  ║
├──╫── env_raw_hits.txt          Full .env file contents       ║
│  ║                                                           ║
│  ╚═══════════════════════════════════════════════════════════╝
│
└── telegram_resultat.txt        Full log of all notifications
```

## 🏗️ Source Architecture

```
Pro ExtraFinder/
│
├── toolkit.go              ← CLI dispatcher, Telegram bot, proxy pool,
│                              WAF bypass, dark web module (~3,900 lines)
│
├── rezandtlg.go            ← Core engine: envdump, extraction, provider
│                              validators, BIP39, detection (~8,800 lines)
│
├── verif_rce.go            ← 34 CVE verifications, exploitation, git pack
│                              parsing, post-exploitation (~3,900 lines)
│
├── checkers.go             ← 80+ credential validators: cloud, email, AI,
│                              proxy, OSINT, crypto, hosting (~7,300 lines)
│
├── github_scan.go          ← GitHub/GitLab code search, 411 queries, token
│                              rotation, private repo dump (~2,900 lines)
│
├── scanners.go             ← S3/IP scanning, domain discovery, SaaS
│                              scoring engine (~2,600 lines)
│
├── auth_bypass.go          ← 40+ auth bypass techniques (~350 lines)
├── certstream.go           ← Real-time CT monitoring (~600 lines)
├── admin_scanner.go        ← Admin panel discovery
├── cors_scanner.go         ← CORS misconfiguration testing
├── cookie_scanner.go       ← Cookie security analysis
├── advanced_crawler.go     ← Deep web crawler + JS analysis
├── vuln_scanner.go         ← SQLi/XSS/LFI/SSRF scanner
├── credential_validator.go ← SSH/FTP/MySQL/Redis/MongoDB validator
├── exploit.go              ← Active CVE exploitation engine
├── dashboard.go            ← Web dashboard + stats API (~180 lines)
├── config.go               ← Configuration, queues, workers (~480 lines)
│
├── settings.json           ← Runtime configuration
├── domains.txt             ← Target input file
├── proxies1.txt            ← Proxy list
├── token.txt               ← GitHub tokens
│
├── Start_Work_Extractor.bat ← Interactive launcher
├── Start_Bot.bat            ← Telegram bot launcher
├── Start_Dashboard.bat      ← Dashboard launcher
│
└── resultat/               ← All output (hits, validated, exploits)
```

<a href="https://t.me/Itachi3d">
<img src="https://img.shields.io/badge/Telegram-@Itachi3d-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" />
</a>

<br><br>

```
  ┌─────────────────────────────────────────────────────┐
  │                                                     │
  │    Built with precision by @ItachiDEV               │
  │                                                     │
  │   "Why use 10 tools when one does it all?"          │
  │                                                     │
  └─────────────────────────────────────────────────────┘
```

<br>

<img src="https://img.shields.io/badge/Made_with-Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
<img src="https://img.shields.io/badge/Code-30K+_Lines-8B5CF6?style=flat-square" />
<img src="https://img.shields.io/badge/Status-Active_Development-success?style=flat-square" />
<img src="https://img.shields.io/badge/License-Private-FF0000?style=flat-square" />

<br><br>

⭐ **Star this repo if it impressed you.**

</div>

