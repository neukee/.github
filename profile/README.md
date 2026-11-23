<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/org-banner-dark.svg">
    <img alt="Neukee: know what breaks before you upgrade Node.js or Next.js" src="assets/org-banner-light.svg" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/neukee/neukee"><img alt="Scanner: pre-release" src="https://img.shields.io/badge/scanner-pre--release-0B0B0C?style=flat-square"></a>
  <a href="https://github.com/neukee/neukee/blob/main/LICENSE"><img alt="License: Apache-2.0" src="https://img.shields.io/badge/license-Apache--2.0-0B0B0C?style=flat-square"></a>
  <img alt="Node.js 22 and 24" src="https://img.shields.io/badge/node-22%20%7C%2024-0B0B0C?style=flat-square&logo=nodedotjs&logoColor=white">
  <img alt="Local-first: no network, no telemetry" src="https://img.shields.io/badge/local--first-no%20network%20%C2%B7%20no%20telemetry-0B0B0C?style=flat-square">
  <img alt="Written in strict TypeScript" src="https://img.shields.io/badge/TypeScript-strict-0B0B0C?style=flat-square&logo=typescript&logoColor=white">
</p>

<h3 align="center">Upgrades shouldn't be a leap of faith.</h3>

<p align="center">
We build engineering tools for modern software teams. The first one reads your repository the way<br>
a careful reviewer would, and tells you what breaks <b>before</b> you upgrade Node.js or Next.js.
</p>

---

### 🐾 [neukee/neukee](https://github.com/neukee/neukee): the upgrade scanner

Point it at a repository and a target version. It is being built to check your code and configuration against the **official release notes** for that version, and to point at the exact lines that will break.

| Built to find | For example |
| --- | --- |
| **Runtime drift** | `.nvmrc` says 24 but the Dockerfile still runs 20; a Node.js version past end-of-life |
| **Native addons** | dependencies that compile native code at install time and break on a new Node.js version |
| **Next.js 16 changes** | request APIs that became async, and config options that changed |
| **What you really install** | versions from npm and pnpm lockfiles, not just `package.json` ranges |

Results will go to your terminal, Markdown, JSON or SARIF, so they can show up in GitHub code scanning.

### Why teams can trust it

<table>
<tr>
<td width="50%" valign="top">

**🔒 Your code never leaves your machine.**<br>
No network calls, no telemetry, and it never runs your code, scripts or package manager. The tests block the network on purpose.

</td>
<td width="50%" valign="top">

**📚 Every rule has a source.**<br>
Each finding links the official release note it comes from. No rule is written from memory or a blog post.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🎯 Same input, same output.**<br>
Reports are deterministic and sorted by a total order, so they are safe to snapshot and diff in CI.

</td>
<td width="50%" valign="top">

**🛡️ Built for hostile input.**<br>
Every scanned file is untrusted: size caps, no symlinks followed, bounded matching work, and a `.gitignore` matcher tested against real git.

</td>
</tr>
</table>

### Where it stands

**Pre-release.** Version 0.1.0 is planned for **December 8, 2026**, and the work happens in the open: every task, decision and review lives in the repository.

<p>
  <a href="https://github.com/neukee/neukee"><b>⭐ Star the repository</b></a> to follow the launch ·
  <a href="https://github.com/neukee/neukee/blob/main/docs/TASKS.md">See the plan</a> ·
  <a href="https://github.com/neukee/neukee/issues/new/choose">Tell us what blocks your upgrade</a>
</p>

### Follow

[LinkedIn](https://www.linkedin.com/company/neukee) · [X](https://x.com/neukee4dev) · [Crunchbase](https://www.crunchbase.com/organization/neukee)

<p align="center"><sub>Neukee · engineering tools for modern software teams</sub></p>
