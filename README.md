<p align="center">
  <img src="https://raw.githubusercontent.com/BlackSpammerBd/blackspammerbd-webdev/main/bsb-logo.png" alt="BLACKSPAMMERBD Logo" width="300"/>
</p>

<h1 align="center" style="font-size: 48px; margin-bottom: 0;">🔥 BLACKSPAMMERBD-WEBMASTER 🔥</h1>
<p align="center" style="font-size: 20px; margin-top: 4px;">
  <strong>The World’s Most Powerful & Professional Web Pentesting Toolkit — 2025 Edition</strong><br/>
  <em>Brought to you by <strong>BLACK SPAMMER BD</strong></em>
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
  <sub>⚠️ This toolkit is intended strictly for authorized, ethical testing and educational purposes only. By using BLACKSPAMMERBD-WEBMASTER, you agree to comply with all applicable laws and regulations. ⚠️</sub>
</div>

---

## 📑 Table of Contents
1. [🔎 Introduction](#🔎-introduction)  
2. [⭐ Why BLACKSPAMMERBD-WEBMASTER?](#⭐-why-blackspammerbd-webmaster)  
3. [🚀 Key Features](#🚀-key-features)  
4. [💻 Supported Platforms](#💻-supported-platforms)  
5. [⚙️ Installation & Prerequisites](#⚙️-installation--prerequisites)  
6. [🛠️ Quick Start & Usage](#🛠️-quick-start--usage)  
   - [Extract All Links](#extract-all-links)  
   - [SQL Injection Testing](#sql-injection-testing)  
   - [Admin Panel Finder](#admin-panel-finder)  
   - [Brute-Force Login](#brute-force-login)  
7. [📂 Output Structure](#📂-output-structure)  
8. [🔧 Advanced Configuration](#🔧-advanced-configuration)  
9. [❓ Troubleshooting](#❓-troubleshooting)  
10. [🤝 Contributing & Roadmap](#🤝-contributing--roadmap)  
11. [📜 License](#📜-license)  
12. [👤 Author & Contact](#👤-author--contact)  
13. [🙏 Acknowledgements](#🙏-acknowledgements)

---

## 🔎 Introduction
Welcome to **BLACKSPAMMERBD-WEBMASTER**—the most **powerful**, **flexible**, and **professional** command-line toolkit for web penetration testing in 2025. Engineered by the cybersecurity experts at **BLACK SPAMMER BD**, this suite empowers security professionals, red teams, and ethical hackers worldwide to:

- 🔍 **Discover** every link on a target website  
- 🧠 **Test** for SQL injection vulnerabilities using 1,000+ advanced payloads  
- 🕵️ **Locate** hidden or obscure admin login panels (1,000+ common paths)  
- 🔐 **Brute-force** login forms with rotating, realistic user-agent strings  

All modules are designed for **ease of use**, **extreme performance**, and **professional results**. By integrating this toolkit into your workflow, you can confidently assess web applications for critical flaws and reinforce your organization’s security posture.

---

## ⭐ Why BLACKSPAMMERBD-WEBMASTER?

- 🔥 **Unmatched Payload Library:** Over **1,000 unique SQL injection vectors** (basic, blind, time-based, error-based, UNION SELECT, WAF bypass, and more).  
- 🌐 **Comprehensive Admin Scanner:** Pre-loaded with **1,000+ admin paths** plus the ability to expand and customize.  
- 🦾 **High-Performance Brute-Force Engine:** Utilizes **1,000+ rotating user-agent strings** to mimic diverse clients, combined with a robust username/password dictionary.  
- 🗄️ **Automated Output Management:** Results are neatly organized into target-named folders, making reporting and analysis effortless.  
- 🎨 **Professional Branding:** Includes a **multi-colored ASCII “BSB” logo**, styled for maximum impact in your terminal.  
- 🌍 **Global Recognition:** 2025-certified toolkit, trusted by security consultants and pen testers around the world.  

---

## 🚀 Key Features

### 1. **Link Extraction**
- Crawl a target website and extract **all internal & external `<a href="">` links**.  
- Stores extracted URLs in a text file under a folder named after the target domain (sanitized).  
- Ideal for mapping attack surfaces or building custom crawlers.

### 2. **SQL Injection Testing**
- Leverages **1,000+ pre-crafted payloads** spanning:  
  - **Basic & Classic:** `' OR '1'='1`, `"' OR '1'='1"`, etc.  
  - **Error-Based:** `UNION SELECT NULL,NULL --`, `AND SLEEP(5) --`, etc.  
  - **Time-Based (Blind):** `'; WAITFOR DELAY '0:0:5'--`, `DBMS_LOCK.SLEEP(5)`, etc.  
  - **WAF Bypass:** Encoded/strategic payloads to bypass mod_security and other filters.  
- Automatically appends each payload to the provided URL parameter and inspects responses for common SQL error patterns (e.g., “mysql_fetch”, “SQL syntax”, “Warning:, etc.).  
- Reports any potentially vulnerable endpoints along with the exact payload used.

### 3. **Admin Panel Finder**
- Scans **1,000+ common admin paths** (e.g., `/admin/`, `/administrator/`, `/cpanel/`, `/adminpanel/`, `/manager/`, **and more**).  
- Customizable path generator allows you to easily add additional endpoints or numbering variations (e.g., `/admin1`, `/admin2`, etc.).  
- Any path returning HTTP **200 OK** is reported as a found admin page.  
- Quickly unearth hidden or unadvertised control panels and dashboards.

### 4. **Brute-Force Login**
- Integrates a curated list of **default usernames** (`admin`, `root`, `admin1`, `admin2`, `rootadmin`, etc.) and **default passwords** (`password123`, `admin`, `123456`, `root`, `toor`, etc.).  
- Utilizes a **500+ (or 1,000+) rotating user-agent engine**—each request appears from a different, realistic browser/client combination (Chrome, Firefox, Safari, Edge, Opera on Windows/macOS/Linux/Android/iPhone).  
- Sends POST requests to the target login form and looks for “logout” (case-insensitive) or other customizable success indicators in the response.  
- Gracefully handles timeouts, HTTP errors, and rate limits.  
- Option to adjust threads/concurrency for large-scale brute-force campaigns.

---

## 💻 Supported Platforms

| Platform                | Status      |
|-------------------------|-------------|
| **Termux (Android)**    | ✅ Fully Tested |
| **Kali Linux**          | ✅ ✅ ✅      |
| **Parrot OS**           | ✅ ✅ ✅      |
| **Ubuntu / Debian**     | ✅ ✅ ✅      |
| **Windows (CMD/PowerShell)** | ✅ ✅ ✅ |
| **macOS (Terminal)**    | ✅ ✅ ✅      |

_For maximum compatibility, ensure you have **Python 3.6+** installed along with `pip`._

---

## ⚙️ Installation & Prerequisites

1. **Clone the repository (optional)**  
   If you wish to customize or inspect source code:
   ```bash
   git clone https://github.com/BlackSpammerBd/blackspammerbd-webdev.git
   cd blackspammerbd-webdev
