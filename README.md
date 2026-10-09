# AKASH SARASWAT

<div align="center">
<img src="./assets/terminal-hero.svg" width="100%" alt="Security operator terminal">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&duration=2300&pause=650&color=00FF41&center=true&vCenter=true&width=820&lines=root%40akash-lab%3A~%24+open+casefile;CASEFILES+%2F+DFIR+%2F+VAPT+%2F+SOC;root%40akash-lab%3A~%24+run+simulation;OBSERVE+%E2%86%92+INVESTIGATE+%E2%86%92+RESPOND" alt="Terminal typing animation">

![Profile Views](https://komarev.com/ghpvc/?username=akash870547-hue&style=flat-square&color=00ff41&label=VISITS)
![Mode](https://img.shields.io/badge/MODE-CASEFILE_SIMULATION-ff3344?style=flat-square&labelColor=080808)
![Scope](https://img.shields.io/badge/SCOPE-AUTHORIZED_LABS-00ff41?style=flat-square&labelColor=080808)
</div>

> **SECURITY OPERATIONS TERMINAL**  
> Operator: **Akash Saraswat** · Environment: **training-lab** · Access: **authorized**  
> Browse the case files below directly in this profile. Expand each file like an incident console; all incident artifacts are synthetic training data.

## ▶ LAUNCH THE INTERACTIVE LAB

**Open the browser-based simulation source:** [simulation/index.html](./simulation/index.html) · [View repository](https://github.com/akash870547-hue/akash870547-hue/tree/main/simulation)

The lab includes a terminal/SOC dashboard, searchable casefile directory, expandable synthetic evidence, DFIR response choices, web-authentication validation choices, network retest decisions, feedback, and session-local scoring. To run it as a website, enable GitHub Pages for this repository and use the `main` branch with `/ (root)` as the source; the simulation will be available at `https://akash870547-hue.github.io/akash870547-hue/simulation/` after Pages finishes publishing.

## ◈ CASEFILE CONSOLE

<details open>
<summary><b>▣ DFIR-001 // WINDOWS RANSOMWARE INVESTIGATION</b> — SIMULATION / SYNTHETIC EVIDENCE</summary>

### SYSTEM ALERT
- **Host:** WS-014
- **User:** analyst-demo
- **Severity:** HIGH
- **Status:** INVESTIGATION OPEN

| Time (UTC) | Event | Analyst note |
|---|---|---|
| 09:14:02 | WINWORD.EXE started | User opened an unexpected document |
| 09:14:08 | PowerShell child process | Suspicious parent-child relationship |
| 09:14:12 | Script launched from Downloads | Review script and command line |
| 09:18:41 | High-volume file modifications | Possible impact activity; validate scope |

### MISSION BRIEF
A user reports documents have become inaccessible. EDR flags an Office process launching PowerShell, followed by unusual file activity. Build a defensible timeline and recommend next steps.

<details>
<summary><b>01 / evidence / network-observations.log</b></summary>

| Time (UTC) | Observation | Confidence |
|---|---|---|
| 09:15:20 | WS-014 → 198.51.100.24:443 | Unverified outbound connection |
| 09:16:02 | WS-014 → 203.0.113.77:443 | Unverified outbound connection |

These are reserved TEST-NET documentation IPs used as placeholders, not live indicators. Correlate proxy, DNS, firewall, and endpoint logs before drawing conclusions.
</details>

<details>
<summary><b>02 / evidence / analyst-notes.md</b></summary>

- Preserve relevant endpoint and central logs.
- Record collection time, time zone, source, collector, and cryptographic hashes.
- Scope other hosts for the same process chain and behavior.
- Follow the approved incident-response procedure for containment.
- Do not execute suspected malware on production systems.
</details>

<details>
<summary><b>03 / analyst terminal / choose your next action</b></summary>

<details>
<summary><b>[A] Preserve evidence first</b></summary>

**Recommended.** Preserve endpoint and central logs, record timestamps, hash collected files, and maintain chain of custody so findings remain defensible.
</details>

<details>
<summary><b>[B] Delete the suspicious file immediately</b></summary>

**Not recommended.** Deletion may destroy evidence and does not establish whether other hosts are affected. Preserve and contain using approved procedures.
</details>

<details>
<summary><b>[C] Declare ransomware confirmed from one alert</b></summary>

**Not supported yet.** The alert is suspicious, but a conclusion needs corroborating process, file, and impact evidence. State confidence and limitations clearly.
</details>

**SIMULATION OBJECTIVE:** write a concise incident timeline, list missing evidence, and propose containment and recovery steps.

[OPEN FULL DFIR CASEBOOK →](https://github.com/akash870547-hue/Digital-Forensics-Incident-Response)
</details>
</details>

<details>
<summary><b>▣ WEB-002 // AUTHENTICATION REVIEW</b> — VAPT SIMULATION</summary>

**Target:** demo-app.local · **Scope:** approved lab only · **Mode:** non-destructive review

### MISSION BRIEF
During an authorized test, session behavior appears inconsistent between browser sessions. Assess the issue without attempting account takeover or touching real user data.

<details>
<summary><b>01 / test observations</b></summary>

| Check | Observation | Next validation |
|---|---|---|
| Session rotation | Not verified | Compare test session identifiers before/after login |
| Logout invalidation | Unknown | Verify invalidation in isolated lab |
| Cookie flags | To inspect | Review Secure, HttpOnly, SameSite in context |
| Rate limiting | To inspect | Use a low-volume agreed test plan |
</details>

<details>
<summary><b>02 / report draft</b></summary>

- **Title:** Session lifecycle weakness (unconfirmed)
- **Evidence:** sanitized request/response excerpts
- **Impact:** state only what evidence demonstrates
- **Severity:** assign after validation
- **Remediation:** rotate sessions after login, invalidate on logout, set appropriate cookie attributes, and regression-test.

**SIMULATION OBJECTIVE:** distinguish an observation from a confirmed vulnerability. Do not claim exploitability until reproduced safely.
</details>

[OPEN WEB VAPT TOOLKIT →](https://github.com/akash870547-hue/web-vapt-suite)
</details>

<details>
<summary><b>▣ NET-003 // NETWORK RETEST DELTA</b> — RETEST SIMULATION</summary>

| Finding | Baseline | Retest | Result |
|---|---|---|---|
| TLS configuration | Weak protocol enabled | Disabled | FIXED — verify with fresh evidence |
| Admin interface exposure | Reachable in lab | Still reachable | OPEN |
| Service version | 1.2 | 1.3 | CHANGED — version change alone is not proof of remediation |

**MISSION BRIEF:** compare like-for-like evidence, record test conditions, and avoid treating a version change alone as proof that a vulnerability is fixed.

[OPEN RETEST AUTOMATION →](https://github.com/akash870547-hue/Network-vapt-retesting-automation)
</details>

## ◈ PROJECT ARCHIVE

| PROJECT | PURPOSE | OPEN |
|---|---|---|
| **0x8Acure** | Interactive cybersecurity learning platform | [Repository →](https://github.com/akash870547-hue/0x8Acure) |
| **Multi-Agent SOC Automation** | AI-assisted SOC workflow exploration | [Repository →](https://github.com/akash870547-hue/multi-agent-soc-automation) |
| **AI DevSecOps Cloud Security** | Cloud security / CI-CD / observability | [Repository →](https://github.com/akash870547-hue/ai-devsecops-cloud-security) |

## ◈ OPERATOR TOOLKIT

<p align="center"><img src="https://skillicons.dev/icons?i=linux,bash,python,git,github,docker,aws,terraform,kubernetes" alt="Technology stack"></p>

- **WEB:** Burp Suite · OWASP · ZAP
- **NETWORK:** Nmap · Wireshark · retesting
- **DFIR:** Windows events · Sysmon · IOC · timelines
- **BUILD:** Python · Docker · AWS · Terraform

## ◈ TELEMETRY

<div align="center">
<img src="https://github-readme-stats.vercel.app/api?username=akash870547-hue&show_icons=true&hide_border=true&bg_color=080808&title_color=00ff41&text_color=c9d1d9&icon_color=ff3344" height="165" alt="GitHub statistics">
<img src="https://streak-stats.demolab.com?user=akash870547-hue&hide_border=true&background=080808&ring=00ff41&fire=ff3344&currStreakLabel=00ff41&sideLabels=c9d1d9&dates=777777" height="165" alt="Contribution streak">
<br>
<img src="https://github-readme-activity-graph.vercel.app/graph?username=akash870547-hue&bg_color=080808&color=00ff41&line=00ff41&point=ff3344&area=true&hide_border=true&custom_title=OPERATOR%20ACTIVITY%20TRACE" width="100%" alt="Activity trace">
</div>

## ◈ RULES OF ENGAGEMENT

- **SCOPE FIRST** — test only with authorization
- **EVIDENCE FIRST** — verify before claiming
- **PRESERVE FIRST** — protect evidence and chain of custody
- **FIX FORWARD** — findings must help remediation
- **LEARN IN LABS** — simulations use synthetic artifacts

<div align="center">
<a href="https://www.linkedin.com/in/akash-saraswat-a81a63295/"><img src="https://img.shields.io/badge/TRANSMIT-LINKEDIN-00ff41?style=for-the-badge&logo=linkedin&logoColor=000000" alt="LinkedIn"></a>
<a href="mailto:akash870547@gmail.com"><img src="https://img.shields.io/badge/TRANSMIT-EMAIL-ff3344?style=for-the-badge&logo=gmail&logoColor=ffffff" alt="Email"></a>
<br><br><img src="./assets/footer.svg" width="100%" alt="Terminal footer">
</div>
