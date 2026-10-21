<div align="center">

# 📰 Web Scraper Headlines Using Python

**An automated Python web scraper that extracts real-time headlines from Google News RSS feeds and compiles them into a clean, interactive HTML news dashboard.**

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![BeautifulSoup](https://img.shields.io/badge/Parser-BeautifulSoup4-4B8BBE)](https://www.crummy.com/software/BeautifulSoup/)
[![Requests](https://img.shields.io/badge/HTTP-Requests-orange)](https://requests.readthedocs.io/)
[![Format](https://img.shields.io/badge/Output-HTML5%20Dashboard-E34F26?logo=html5&logoColor=white)](news.html)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completed-success)](#)

<br/>

> *Developed by **Sharad Sharma** for **SyntecXHub Technologies Pvt. Ltd.** (Task-3: Python Programming Internship).*

</div>

---

## 📌 Project Overview

**Web Scraper Headlines** is a lightweight, efficient Python automation script designed to fetch, parse, and organize live world news. 

Instead of relying on fragile web scrapers that break whenever page layouts change, this tool interfaces directly with **Google News' official XML/RSS feed** (`https://news.google.com/rss`). It extracts trending articles, timestamps, and direct URLs, dynamically synthesizing a standalone, beautifully styled HTML newspaper dashboard (`news.html`).

---

## ✨ Key Features

- ⚡ **Direct RSS Feed Parsing**: Fetches structured XML data directly from Google News with spoofed user-agent headers to guarantee high uptime.
- 🥣 **Intelligent XML Extraction**: Uses **BeautifulSoup4** with XML parsing to cleanly extract article titles, publication timestamps, and destination hyperlinks.
- 🎨 **Automated Dashboard Generation**: Automatically generates a clean, readable HTML dashboard (`news.html`) with styled cards, shadows, and hover animations.
- 🛡️ **Robust Error Handling**: Built-in network exception handling (`RequestException`) and timeouts to handle connection drops gracefully.
- 🚀 **Zero Database Requirement**: Stateless and portable — generates a ready-to-open HTML report in seconds.

---

## 🔄 Workflow Diagram

```text
┌───────────────────────────┐
│   Google News RSS Feed    │
│  (https://news.google.com)│
└─────────────┬─────────────┘
              │  HTTP GET (requests with User-Agent)
              ▼
┌───────────────────────────┐
│    web_scraper_headlines  │
│  - Parses XML with BS4    │
│  - Extracts Title, Link,  │
│    and Publication Date   │
└─────────────┬─────────────┘
              │  Compiles HTML markup
              ▼
┌───────────────────────────┐
│     news.html Dashboard   │
│  - Modern Card Layout     │
│  - Direct Story Links     │
└───────────────────────────┘
```

---

## 🛠️ Tech Stack & Libraries

| Module / Package | Version | Purpose |
| :--- | :--- | :--- |
| **Python** | `3.8+` | Core programming language |
| **`requests`** | `^2.31` | Dispatches HTTP GET requests with custom headers and timeout |
| **`beautifulsoup4`** | `^4.12` | XML and HTML parser for navigating the document tree |
| **`lxml`** *(optional)* | `^5.0` | High-performance XML parser backend |
| **`os`** | Standard Library | File path resolution and disk write operations |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.8 or higher installed on your computer:

```bash
python --version
```

### Installation

1. **Clone this repository:**
   ```bash
   git clone https://github.com/sharad1sharma/WEB-SCRAPING-HEADLINES-USING-PYTHON.git
   cd WEB-SCRAPING-HEADLINES-USING-PYTHON
   ```

2. **(Optional) Create and activate a virtual environment:**
   - **Windows:**
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - **macOS / Linux:**
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

3. **Install required packages:**
   ```bash
   pip install requests beautifulsoup4 lxml
   ```

---

## 💻 How to Run

Execute the script from your terminal:

```bash
python web_scraper_headlines.py
```

### Sample Terminal Output:

```text
Successfully saved 35 news articles.
HTML file created successfully!
Location: C:\Projects\WEB-SCRAPING-HEADLINES-USING-PYTHON\news.html
```

---

## 📰 Generated Dashboard Preview

The script compiles a standalone `news.html` dashboard formatted with modern cards:

```text
========================================================================
                         Google News Headlines
========================================================================

+----------------------------------------------------------------------+
| [Headline Title: Tech Giant Announces Breakthrough in Quantum AI]   |
| Date: Wed, 21 Oct 2026 14:30:00 GMT                                  |
| Link: https://news.google.com/rss/articles/CBMi...                   |
+----------------------------------------------------------------------+

+----------------------------------------------------------------------+
| [Headline Title: Global Markets React to Latest Economic Policy]    |
| Date: Wed, 21 Oct 2026 12:15:00 GMT                                  |
| Link: https://news.google.com/rss/articles/CBMi...                   |
+----------------------------------------------------------------------+
```

To view the dashboard, simply open `news.html` in any browser:
```bash
# Windows
start news.html

# macOS
open news.html

# Linux
xdg-open news.html
```

---

## 📂 Project Structure

```text
WEB-SCRAPING-HEADLINES-USING-PYTHON/
│
├── web_scraper_headlines.py    # Main web scraping & HTML synthesis engine
├── news.html                   # Generated news dashboard (created upon run)
└── README.md                   # Comprehensive documentation
```

---

## 👤 Author

**Sharad Sharma**
- GitHub: [@sharad1sharma](https://github.com/sharad1sharma)
- Email: [sharmasharad9531@gmail.com](mailto:sharmasharad9531@gmail.com)
- Organization: **SyntecXHub Technologies Pvt. Ltd.**

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
