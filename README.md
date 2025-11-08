# FACEBOOK-AUTOMATION

![Status: Archive](https://img.shields.io/badge/status-archive-lightgrey) ![Platform: Windows](https://img.shields.io/badge/platform-Windows-blue) ![Tech: Selenium](https://img.shields.io/badge/tech-Selenium-brightgreen)

FACEBOOK-AUTOMATION is a Windows automation demo that uses Selenium WebDriver to collect profile IDs from a configured target follower list and send friend requests to selected profiles. This repository currently includes a compiled Windows executable for demonstration and testing purposes. Use responsibly and only on accounts you own or have explicit permission to test.

---

## Table of contents

- Overview
- Features
- Quick start
- Configuration
- Security and responsible use
- Repository contents
- Contributing
- License
- SEO metadata

---

## Overview

**What it does:** Logs into Facebook (runtime prompt for credentials), navigates to a preconfigured follower list, auto-scrolls to harvest profile links/IDs, randomly selects profiles from the harvested list, visits profiles one by one, and attempts to send friend requests.

**Intended purpose:** Educational demo and local testing of browser automation techniques using Selenium WebDriver on Windows.

---

## Features

- Automated Facebook login prompt
- Auto-scrolling of follower/following list to collect profile IDs
- Randomized selection of harvested profiles
- Sequential profile visits and friend request attempts
- Packaged as a Windows executable for one-click runs

---

## Quick start

1. Clone or download this repository.
2. Use a disposable or test Facebook account you control.
3. Run the included executable (`BULK REQUEST.exe`) on a Windows machine in an isolated environment.
4. Enter credentials when prompted.
5. The program navigates to the configured follower list, collects profile IDs, and attempts friend requests.

Do not run this on personal or production accounts you rely on.

---

## Configuration

- **Target profile ID:** Embedded in the program/binary. To change it, replace the executable with a rebuilt binary containing your desired target or add a config mechanism in source before compiling.
- **Delays and limits:** If you build from source, implement conservative, randomized delays and processing limits to mimic human behaviour during testing.
- **Credentials:** Provide credentials at runtime only; never hardcode or commit real account credentials to the repository.

In future we will add this feature:
- `target_id` — Facebook profile ID whose followers will be harvested
- `max_profiles` — Maximum profiles to process
- `min_delay` / `max_delay` — Random delay range (seconds) between actions
- `headless` — Run with browser visible (recommended for testing) or headless

---

## Security and responsible use

**Legal and ethical notice:** Automating unsolicited actions on third‑party services can violate Terms of Service and local laws. You are solely responsible for how you use this tool. Always:

- Test only on accounts you own or have written permission to test.
- Use isolated environments (VMs) and disposable test accounts.
- Avoid mass unsolicited messaging or actions that constitute spam or harassment.
- Do not distribute harvested personal data or credentials.
- Verify unknown executables in a sandbox before running.

---

## Repository contents

- `BULK REQUEST.exe` — Precompiled Windows executable that performs the automation described.
- `README.md` — This document.
- (Optional) Future additions: source code, build scripts, config templates, tests.

---

## Contributing

Contributions are welcome only when they improve safety, transparency, and usability. Acceptable contributions:

- Adding source code with build and config instructions
- Implementing explicit consent checks, logging, and rate limits
- Improving documentation and security guidance

Contributions that enable evasion of platform protections, mass unsolicited messaging, or abuse will be rejected.

---


## ___________________________

**Topics / keywords:** facebook-automation, selenium, selenium-webdriver, social-media-automation, bulk-friend-request, follower-scraping, windows-executable, automation-demo

---
