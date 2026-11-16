# Awesome-HTTP-Cookie-Session-Management

# Top HTTP Cookie & Session Management Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Cookie Inspection, Consent Management & Self-Hosted Session Tooling*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **HTTP Cookie & Session Management**. These tools help developers and security teams inspect, edit, and audit cookies and sessions—covering everything from browser extensions that manage session state to self-hosted consent platforms that enforce privacy compliance.

**Examples** include Postman Cookie Management, Bokal, OWASP PTK, Hugin, ConsentOS, and Conzent OCI (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted cookie editing, open-source session tooling, and community-driven consent management—ideal for teams seeking data sovereignty and avoiding per-domain SaaS pricing. The open-source landscape is genuinely functional: **Bokal** is the trustworthy successor to EditThisCookie with full HttpOnly control , **Hugin** bundles a cookie jar into a security testing proxy , and **ConsentOS** provides a self-hosted OneTrust alternative with IAB TCF v2.3 support .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Postman Cookie Management](https://www.postman.com/)** | Cookie jar within Postman for managing session cookies across API requests. Supports domain-level cookie management and automatic cookie persistence. | Free: **$0** (1 user); Solo: **$9/month**; Team: **$19/user/month** | **Free**: 1 user only, unlimited collection runs, no team workspace (March 2026 restructure) |
| **[Charles Proxy](https://www.charlesproxy.com/)** | HTTP proxy with cookie inspection and session management. View and edit cookies in transit. | ~**$50** (license) | Free trial with 30-minute session limits |
| **[Fiddler](https://www.telerik.com/fiddler)** | Web debugging proxy with cookie inspection. | Lite: **$7/user/month** (annual); Pro: **$13** | Lite plan available; Pro features require paid subscription |
| **[Cookiebot](https://www.cookiebot.com/)** | Cookie consent management platform (CMP) with automated scanning and compliance reporting. | Quote-only | Free trial available |
| **[OneTrust Cookie Compliance](https://www.oneTrust.com/)** | Enterprise cookie consent and compliance platform. | Quote-only (module-based) | No free tier; demo via sales |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Bokal](https://github.com/yuvisbabbar/Bokal)** | [![Stars](https://img.shields.io/github/stars/yuvisbabbar/Bokal?style=social&color=white)](https://github.com/yuvisbabbar/Bokal/stargazers) | **The trustworthy open-source successor to EditThisCookie.** **Chrome extension** for developers, QA, and privacy-conscious users . **Full cookie control**: view, edit, add, and delete cookies **including HttpOnly cookies** that UI-only tools can't touch . **Search, filter, protect, pin, and block** cookies by domain . **Automatic cleanup** with a preserve list—clear everything else with one click or daily sweep . **Cookie audit hints**: flags missing SameSite, unpartitioned cross-site cookies, and oversized cookies . **Export to JSON, Netscape, and cookie-header formats**; **Playwright/Puppeteer storageState export** for test automation . **CHIPS partition inspector** for modern partitioned cookies. **DevTools panel** for in-browser inspection . **No telemetry, no tracking, local-first**—cookies never leave your device . **Best for QA engineers and developers** needing a safe, open-source cookie editor with test automation export. |
| **[OWASP Penetration Testing Kit (PTK)](https://github.com/DenisPodgurskii/pentestkit)** | — | **Open-source browser extension for interactive security testing.** **Capture and inspect HTTP requests and responses** from real browser workflows . **Cookie and session inspection**: review cookies, browser storage, security headers, and application technologies . **JWT inspection and editing** built in . **R-Builder** for replaying and modifying requests with cURL import/export . **Runs from the live browser session**—no separate proxy required for normal workflows . **Integrates with OWASP ZAP** for combined browser-side and proxy-based testing . **Best for security practitioners** wanting cookie/session inspection alongside broader web app testing. |
| **[Hugin](https://github.com/HuginCyber/Hugin)** | [![Stars](https://img.shields.io/github/stars/HuginCyber/Hugin?style=social&color=white)](https://github.com/HuginCyber/Hugin/stargazers) | **Local-first security testing power tool in a single Rust binary.** **Intercepting proxy** with **cookie jar, session macros, and WebSocket message interception** . **HTTP/1.1, HTTP/2, HTTP/3 (QUIC), and WebSocket** support . **No accounts, no telemetry, no cloud**. **Cookie jar** manages session cookies across requests; **session macros** automate authentication flows . **Active scanner** with 64 checks including session fixation and CSRF . **Best for security testers** wanting a comprehensive proxy with cookie/session management built in. |
| **[PhoenixBox](https://github.com/avihayf/PhoenixBox)** | — | **Multi-container extension for pentesting with full session isolation.** **Color-coded containers** isolate cookies, storage, and sessions by role . **Route traffic through Burp Suite or custom proxies** per container . **No telemetry, no data collection** . **Best for bug bounty hunters and pentesters** needing to maintain multiple authenticated sessions simultaneously without collisions. |
| **[AuthForge](https://github.com/mthcht/AuthForge)** | [![Stars](https://img.shields.io/github/stars/mthcht/AuthForge?style=social&color=white)](https://github.com/mthcht/AuthForge/stargazers) | **Browser addon for cookie and token extraction.** **Network capture** of `Set-Cookie` headers, `Authorization` headers, and JWT detection . **Request Workbench** for replaying captured requests with editable headers, body, and **`Use captured token…`** to swap in any detected token . **Best for security testers** wanting to inspect and manipulate cookies/tokens during testing. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[ConsentOS](https://github.com/consentos/consentos)** | — | **Self-hosted OneTrust/Cookiebot alternative.** **Elastic License 2.0** (source-available, self-host indefinitely) . **IAB TCF v2.3, GPP v1, Google Consent Mode v2, GPC** support . **Auto-blocking** intercepts script creation and cookie writes until consent is granted . **Cookie scanner** with Playwright and Open Cookie Database (2,200+ patterns) . **Dark pattern detection** and **compliance engine** for GDPR, CCPA/CPRA, ePrivacy . **Best for teams wanting privacy-first consent management** on their own infrastructure. |
| **[Conzent OCI](https://github.com/conzent-net/oci)** | — | **PHP-based open-source consent management platform.** **IAB TCF v2.2/v2.3 and Google Consent Mode v2** support . **Built-in cookie scanner** with headless Chromium . **Multi-tenant** with organisations, sites, and role-based access . **12 domain boundaries** including Identity, Cookie, Consent, Banner, Compliance, and Scanning . **Best for organizations wanting a self-hosted CMP** with compliance reporting. |
| **[next-iron-session](https://github.com/vvo/next-iron-session)** | — | **Secure, stateless, cookie-based session library for Next.js.** **4.1k GitHub stars** . Encrypted session cookies with no server-side storage. **Best for Next.js developers** needing secure session management without a database. |
| **[gorilla/securecookie](https://github.com/gorilla/securecookie)** | — | **Go library for authenticated and encrypted cookie values.** **668 stars** . **Best for Go developers** needing secure cookie encoding/decoding. |

**Frameworks for building custom systems**: Choose **Bokal** for a safe, open-source cookie editor with Playwright/Puppeteer export , **ConsentOS** for a self-hosted consent platform with IAB TCF compliance , or **next-iron-session** for encrypted session cookies in Next.js —all without per-domain SaaS fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cookie and session management tools handle authentication tokens and potentially sensitive session data; **only inspect or modify cookies on systems you own or have explicit authorization to test**. Cookie theft enables account takeover.
- **The cookie tooling landscape has a trust problem.** **Bokal explicitly positions itself as the trustworthy successor to EditThisCookie**, which was taken down and replaced by a copycat—Bokal has **no telemetry, no remote code, and minimal permissions** (no "tabs" permission, requests host access only when you choose to manage a site) . **OWASP PTK and Hugin are purpose-built for authorized security testing**—using them on production sites without permission can modify data and trigger security monitoring . **ConsentOS and Conzent OCI solve a different problem**: they are **consent management platforms** that block cookies until user consent is granted, not tools for inspecting or editing existing cookies . **Commercial CMPs (OneTrust, Cookiebot) are quote-only enterprise contracts**—ConsentOS offers a source-available self-hosted alternative with IAB TCF v2.3 support . **Validate whether you need cookie inspection/editing (Bokal, PTK, Hugin), session isolation (PhoenixBox), or consent management (ConsentOS, Conzent)** before committing.

---

**Made for developers, QA engineers, and security teams managing cookies and sessions.**  
Let's make HTTP cookie and session management more open, trustworthy, and privacy-respecting.
