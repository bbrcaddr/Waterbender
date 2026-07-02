# Security Policy

Thanks for helping keep Waterbender and its users safe.

## Reporting a vulnerability

**Please do not open a public issue for anything security‑sensitive.** Public
disclosure before a fix puts users at risk.

Instead, report it privately through **GitHub's private vulnerability reporting**:

> Repository → **Security** tab → **Report a vulnerability**
> (https://github.com/bbrcaddr/Waterbender/security/advisories/new)

If you prefer email, you can reach the maintainer at **<CONTACT-EMAIL>**.

Please include, as best you can:

- The **Waterbender version** and your **OS + version**.
- A description of the issue and its **potential impact**.
- **Steps to reproduce** (a minimal proof of concept helps a lot).
- Any relevant logs, a sample `.wb` project, or screenshots.

## What to expect

- An acknowledgment, typically within a few days.
- An honest assessment of severity and a fix timeline once triaged.
- Coordinated disclosure — we'll agree on timing before any public write‑up.
- Credit for the report if you'd like it (let us know how you'd like to be named).

## Supported versions

Waterbender auto‑updates, so security fixes ship in the **latest release** only.
Please make sure you're on the newest version before reporting.

## Scope

In scope: the Waterbender desktop application, its auto‑updater, and the
static‑site / native export it produces. Out of scope: issues that require a
malicious build you supplied yourself, or vulnerabilities in third‑party
dependencies that already have a public advisory (report those upstream).

The companion SDK is maintained separately —
[bbrcaddr/waterbender-sdk](https://github.com/bbrcaddr/waterbender-sdk).
