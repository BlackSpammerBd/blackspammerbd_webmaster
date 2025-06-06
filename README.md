<p align="center">
  <img src="https://raw.githubusercontent.com/BlackSpammerBd/blackspammerbd-webdev/main/bsb-logo.png" alt="BLACKSPAMMERBD Logo" width="350"/>
</p>

<h1 align="center" style="font-size: 54px; margin: 8px 0;">🔥 BLACKSPAMMERBD-WEBMASTER 🔥</h1>
<p align="center" style="font-size: 22px; margin-top: 4px;">
  <strong>The Pinnacle of Web Pentesting</strong><br/>
  <em>Engineered by <strong>BLACK SPAMMER BD</strong> for Elite Security Experts</em>
</p>

<p align="center">
  <a href="https://pypi.org/project/blackspammerbd-webmaster/">
    <img src="https://img.shields.io/pypi/v/blackspammerbd-webmaster.svg?style=for-the-badge" alt="PyPI Version"/>
  </a>
  <a href="https://github.com/BlackSpammerBd/blackspammerbd-webdev">
    <img src="https://img.shields.io/github/stars/BlackSpammerBd/blackspammerbd-webdev.svg?style=for-the-badge" alt="GitHub Stars"/>
  </a>
  <a href="https://github.com/BlackSpammerBd/blackspammerbd-webdev/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/BlackSpammerBd/blackspammerbd-webdev/ci.yml?branch=main&style=for-the-badge" alt="CI Status"/>
  </a>
  <a href="https://github.com/BlackSpammerBd/blackspammerbd-webdev/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/BlackSpammerBd/blackspammerbd-webdev.svg?style=for-the-badge" alt="License"/>
  </a>
</p>

---

<div align="center">
  <sub>🔒 <strong>Disclaimer:</strong> This tool is strictly for <em>authorized</em> and <em>ethical</em> security testing. Use only on targets you own or have explicit permission to audit. 🔒</sub>
</div>

---

## 📑 Table of Contents

1. [🌟 Introduction](#🌟-introduction)  
2. [🚀 Why Choose BLACKSPAMMERBD-WEBMASTER?](#🚀-why-choose-blackspammerbd-webmaster)  
3. [🛠️ Comprehensive Feature Set](#🛠️-comprehensive-feature-set)  
4. [💻 Supported Environments](#💻-supported-environments)  
5. [⚙️ Quick & Easy Installation](#⚙️-quick--easy-installation)  
6. [🎯 CLI Usage & Examples](#🎯-cli-usage--examples)  
   - [🔗 Link Extraction](#🔗-link-extraction)  
   - [💥 SQL Injection Testing](#💥-sql-injection-testing)  
   - [🔍 Admin Panel Discovery](#🔍-admin-panel-discovery)  
   - [🔐 Advanced Brute-Force](#🔐-advanced-brute-force)  
   - [📊 Combined Workflow Example](#📊-combined-workflow-example)  
7. [📂 Output Directory Layout](#📂-output-directory-layout)  
8. [🔧 Deep Dive: Configuration & Customization](#🔧-deep-dive-configuration--customization)  
   - [🧩 Payload Libraries](#🧩-payload-libraries)  
   - [⚡ Concurrency & Timeouts](#⚡-concurrency--timeouts)  
   - [🌐 Proxy, Tor & VPN Support](#🌐-proxy-tor--vpn-support)  
   - [📝 Success Indicators & Response Patterns](#📝-success-indicators--response-patterns)  
9. [❓ Troubleshooting & FAQs](#❓-troubleshooting--faqs)  
10. [🚧 Contributing & Roadmap](#🚧-contributing--roadmap)  
11. [📜 License](#📜-license)  
12. [👥 Author & Contact Info](#👥-author--contact-info)  
13. [🙏 Acknowledgements & Credits](#🙏-acknowledgements--credits)

---

## 🌟 Introduction

Welcome to **BLACKSPAMMERBD-WEBMASTER**, the ultimate **2025-grade** web penetration-testing framework built for professionals. If you demand:

- **Unrivaled power** in detecting vulnerabilities  
- **Extensive payload coverage** for SQL injection, admin discovery, brute-forcing  
- **Rock-solid stability** across Termux, Linux, macOS, and Windows  
- **Elegant, organized outputs** for seamless reporting  

…then you’ve found your new go-to toolkit. Every line of code has been handcrafted by **BLACK SPAMMER BD**, the renowned cyber experts dedicated to empowering ethical hackers and red teams.

### What This Toolkit Offers at a Glance

- **Link Extraction:** Harvest all internal/external URLs  
- **SQLi Testing:** 1,000+ unique payloads (error-based, time-based, blind, WAF-bypass)  
- **Admin Panel Scanning:** 1,000+ common & custom paths  
- **Brute-Force Engine:** 1,000+ rotating user-agents + dynamic credentials  
- **Automatic Result Management:** Target-named directories with clear, timestamped logs  
- **Professional CLI Experience:** Colorful banners, clear progress indicators, and detailed summaries  

Forget piecing together multiple scripts—**BLACKSPAMMERBD-WEBMASTER** consolidates everything you need into a single, cohesive command-line suite.

---

## 🚀 Why Choose BLACKSPAMMERBD-WEBMASTER?

<details>
<summary style="font-size: 18px; cursor: pointer;">Click to expand key differentiators & strengths</summary>

<br/>

### 1. Unmatched Payload Repository  
- **1,000+ SQL Injection Vectors**  
  - **Basic & Classic:**  
    `' OR '1'='1`, `" OR "1"="1`, `' OR '1'='1' --`, etc.  
  - **Error-Based:**  
    `UNION SELECT NULL,NULL --`, `AND SLEEP(5) --`, `DBMS_LOCK.SLEEP(5) --`, and more.  
  - **Time-Based (Blind):**  
    `'; WAITFOR DELAY '0:0:5'--`, `' AND SLEEP(10) --`, `SELECT CASE WHEN (1=1) THEN TO_CHAR(1/0) END`, etc.  
  - **WAF Bypass Techniques:**  
    Encoded payloads, comment injections, double-URL-encoded patterns, random suffix generation.  
  - **Database-Specific Variants:**  
    MSSQL (`xp_cmdshell`, `@@version`), Oracle (`DBMS_LOCK.SLEEP`), MySQL (`benchmark()`), PostgreSQL bypasses, and more.

### 2. Hyper-Extensive Admin Path Scanner  
- **1,000+ Preloaded Paths** for common panels:  
  `/admin/`, `/administrator/`, `/cpanel/`, `/manage/`, `/adminpanel/`, `/admin-console/`, etc.  
- **Dynamic Path Generation:**  
  Numerical suffixes, framework-specific endpoints (WordPress, Joomla, Drupal), custom user-defined lists.  
- **Rapid Discovery:**  
  Multi-threaded scanning optional, with customizable request rates and headers.

### 3. Elite Brute-Force Capability  
- **1,000+ Rotating User-Agent Strings**  
  - Chrome, Firefox, Safari, Edge, Opera—across Windows, macOS, Linux, Android, iOS.  
  - Randomized version numbers for maximum stealth.  
- **Dynamic Credential Sets**  
  - Default username list: `admin`, `root`, `administrator`, `test`, `admin123`, etc.  
  - Default password list: `password123`, `admin`, `123456`, `root`, `toor`, plus custom dictionaries.  
- **Advanced Response Handling:**  
  - Success detected by presence of “logout”, “dashboard”, “welcome” (case-insensitive)  
  - Configurable string/regex patterns for custom login pages  
  - Optional CAPTCHA detection & bypass placeholders

### 4. Seamless Automation & Extensibility  
- **Modular Codebase:**  
  Each function lives in its own module (`extractor.py`, `sql_tester.py`, `admin_finder.py`, `brute_forcer.py`, `utils.py`).  
- **Customizable Config Files:**  
  - Drop a `data/user_agents.txt` to override defaults  
  - Add `custom_admin_paths.txt` or `custom_sql_payloads.txt` for tailored scans  
- **Future-Proof:**  
  Easily add new modules (XSS scanning, RCE detection) under the same CLI interface.

### 5. Professional Quality Output  
- **Auto-Creation of Target Folder:**  
  - Sanitized domain name as folder  
  - `links.txt`, `sqli_results.txt`, `admin_paths.txt`, `brute_results.txt` (timestamped)  
- **Colorful Console Banners & Progress Bars:**  
  - ANSI color codes for visually distinct sections  
  - Clear summary at the end of each scan

### 6. Global Recognition & Support  
- **Trusted by Security Teams Worldwide:**  
  Frequently referenced in professional pentesting blogs, training courses, and global security forums.  
- **Active GitHub Community:**  
  Join the [Facebook Group](https://facebook.com/groups/black.spammar.bd/) or open issues/questions on our [GitHub Repo](https://github.com/BlackSpammerBd/blackspammerbd-webdev).

</details>

---

## 🛠️ Comprehensive Feature Set

Below is a high-level overview of each core module and its capabilities:

### 1. Link Extraction (`sp e <url>`)
- **Goal:** Gather all `<a href="">` links from a website.  
- **Mechanism:**  
  - Sends GET request to target URL.  
  - Parses HTML with BeautifulSoup.  
  - Collects unique `href` attributes (absolute & relative).  
- **Output:**  
  - Creates folder `<target-domain>/`  
  - Writes `links.txt` containing one URL per line.

### 2. SQL Injection Testing (`sp c <url>`)
- **Goal:** Identify SQL injection vulnerabilities at a given parameter.  
- **Mechanism:**  
  - Generates **1,000+** payloads via `utils.generate_sql_payloads()`.  
  - Appends each payload to the provided URL (e.g., `?id=1` → `?id=1' OR '1'='1`).  
  - Scans response for SQL error indicators (e.g., “SQL syntax”, “mysql_fetch”, “warning:”).  
  - Time-based checks by measuring response delays (for `SLEEP` payloads).  
- **Output:**  
  - Prints each vulnerable payload + URL to console.  
  - Writes `sqli_results.txt` in target folder, listing payloads and affected endpoints.

### 3. Admin Panel Discovery (`sp find <url>`)
- **Goal:** Locate hidden or unlisted admin/login panels across a site.  
- **Mechanism:**  
  - Loads **1,000+** paths from `utils.generate_admin_paths()`.  
  - Iterates sequentially or (optionally) multi-threaded.  
  - Sends HEAD/GET requests to `<base_url>/<path>`.  
  - Detects HTTP 200 OK or redirects to login.  
- **Output:**  
  - Prints “Found admin page: `<full_url>`” for each hit.  
  - Writes `admin_paths.txt` listing all discovered admin URLs.

### 4. Advanced Brute-Force Login (`sp brute <login_url>`)
- **Goal:** Attempt brute-force against a login form with dynamic stealth.  
- **Mechanism:**  
  - Loads default usernames from `utils.default_usernames()`: [`admin`, `root`, `admin1`, `admin2`, `rootadmin`, …]  
  - Loads default passwords from `utils.default_passwords()`: [`password123`, `admin`, `123456`, …]  
  - Fetches **1,000+** random user-agents via `utils.generate_user_agents(1000)`  
  - For each user-agent, for each username, for each password:  
    - Sends POST request with `{'username': user, 'password': pwd}` and `{'User-Agent': <ua>}`  
    - Checks if response contains any success keyword (“logout”, “dashboard”, “welcome”).  
  - Stops early upon a successful login.  
- **Output:**  
  - On success: prints `Successful login: <user>:<pwd> (UA: <ua>)`, writes to `brute_results.txt`.  
  - If none succeed: prints `Brute force completed. No valid credentials found.`, still writes a summary log.

---

## 💻 Supported Environments

| Platform           | Status         | Notes                              |
|--------------------|----------------|------------------------------------|
| **Termux (Android)** | ✅ Tested      | Works seamlessly in Termux.        |
| **Kali Linux**       | ✅ Fully Tested | Recommended for pentesters.        |
| **Parrot OS**        | ✅ Fully Tested | Parrot-compatible.                 |
| **Ubuntu / Debian**  | ✅ Fully Tested | LTS support, apt-get integration.  |
| **Windows**          | ✅ Fully Tested | Use Git Bash or PowerShell.        |
| **macOS**            | ✅ Fully Tested | Native Terminal & iTerm support.   |

> **Requirement:** Python **3.6+** and `pip`. Dependencies (`requests`, `beautifulsoup4`) auto-install via PyPI.

---

## ⚙️ Quick & Easy Installation

1. **Install from PyPI (Recommended)**  
   ```bash
   pip install blackspammerbd-webmaster
