README.md
# QiLife-Eos

**The dawn of the QiLife ecosystem.**  
QiLife-Eos is the root superproject: standards, modules, and scaffolds that power QiSuite, QiVault, QiPortals, and beyond.

> **License snapshot**
> - ✅ Personal learning & non-commercial public use allowed **with attribution**.
> - 🚫 Commercial use of any part/idea requires **attribution + paid license**.
> - See: [`LICENSE.qilife-eos`](./LICENSE.qilife-eos).

---

## Why Eos?
**Eos** = the first light. This repo holds the patterns, contracts, and templates that everything else orbits.

## What’s inside (starter layout)


/docs/ # Design notes, architecture, ADRs
/packages/ # Libraries, UI kits, SDKs (monorepo-friendly)
/services/ # Backends, workers, APIs
/apps/ # User-facing apps (web, desktop, mobile)
/tooling/ # CLIs, dev scripts, codegen
/templates/ # Project scaffolds, ISSUE/PR templates

You can start minimal (one app, one service) and grow into a monorepo.

---
# Getting Started
## 1) Clone
git clone https://github.com/<your-org>/QiLife-Eos.git
cd QiLife-Eos
---
## 2) Optional: 
set up workspace (pnpm recommended for monorepos)
corepack enable
pnpm install
---
## 3) Run whatever starter app you seed into /apps

pnpm -C apps/portal dev

Standards (tl;dr)

Language: JS/TS + Python, typed where possible.

Packages: pnpm workspaces for Node; uv/pipx for Python tools.

Style: Prettier + ESLint; Black + Ruff (Python).

Commits: Conventional Commits (feat:, fix:, etc.)

Docs: Markdown first; ADRs in /docs/adr.
---
# Attribution

If you use any portion publicly (even non-commercial), add this to your README or site footer:

Built with QiLife-Eos • © QiAlly (Cody Rice-Velasquez) • https://qially.me

For commercial licenses and attributions, see Commercial Use below.

# Commercial Use

Commercial usage (any activity intended for, related to, or resulting in revenue, including internal business use) requires:

Attribution, and

A paid commercial license from QiAlly.

→ Contact: licensing@qially.me
 (subject: QiLife-Eos Commercial License)

Until a paid license is in place, commercial use is not permitted.
---
# Contributing

We welcome issues and non-commercial contributions that respect this project’s license. Opening a PR implies you license your contribution to the project under the QiLife-Eos License (see LICENSE.qilife-eos).
---
# Security

Report vulnerabilities privately: security@qially.me
. We’ll acknowledge responsibly.
---
# License

Personal learning & non-commercial public use allowed with attribution.
Commercial use requires attribution and payment.
Full terms: LICENSE.qilife-eos

© QiAlly / Cody Rice-Velasquez. All rights reserved where not expressly granted.

---

# `.gitignore` 
### (monorepo-friendly: Node + Python + common build artifacts)

```gitignore
# Node
node_modules/
pnpm-lock.yaml
npm-debug.log*
yarn.lock
*.tsbuildinfo

# Builds / dist
dist/
build/
.cache/
.next/
out/
coverage/
*.log
*.tmp
*.DS_Store

# Vite / bundlers
.vite/
.esbuild/
.parcel-cache/

# Monorepo workspaces
packages/*/node_modules/
apps/*/node_modules/
services/*/node_modules/

# Env / secrets
.env
.env.*
!.env.example

# Python
__pycache__/
*.py[cod]
*.pyo
*.egg-info/
.venv/
venv/
.python-version
.mypy_cache/
.pytest_cache/

# IDEs
.vscode/
.idea/
*.swp

# OS
Thumbs.db
.DS_Store
.Spotlight-V100
.Trashes

# Misc
*.orig
*.bak
```
---
# LICENSE.qilife-eos
## QiLife-Eos License v1.0
**© QiAlly / Cody Rice-Velasquez (“Licensor”)**

# 1. Definitions
1.1 “Work” means the QiLife-Eos repository and all files included herein, including designs, code, templates, documentation, and ideas expressed in such materials.
1.2 “You” means any individual or legal entity exercising permissions granted by this License.
1.3 “Non-Commercial Use” means personal learning, research, experimentation, portfolio demos, and public sharing where no direct or indirect commercial advantage is intended or realized by You or a third party.
1.4 “Commercial Use” means any use intended for, related to, or resulting in revenue, monetization, productivity, or business advantage, whether internal or external, including without limitation: deploying in a business, consulting deliverables, SaaS, client projects, paid prototypes, fundraising demos, or training models for commercial products.
1.5 “Attribution” means a visible credit: “Built with QiLife-Eos • © QiAlly (Cody Rice-Velasquez) • https://qially.me” in user-facing documentation (e.g., README, about page, site footer) and in source headers where practical.

# 2. Grant
2.1 Non-Commercial License. Subject to the terms herein, Licensor grants You a worldwide, royalty-free, non-exclusive, non-transferable license to (a) use, view, reproduce, and modify the Work; and (b) publicly perform and display derivative works, strictly for Non-Commercial Use, provided that Attribution is preserved and this License is included with the Work and substantial portions thereof.
2.2 No Commercial Rights. Commercial Use is NOT granted under Section 2.1. Any Commercial Use requires a separate paid commercial license from Licensor prior to such use.
2.3 Patents. No patent rights are granted under this License. Any patent license must be explicitly agreed in a separate commercial agreement.

# 3. Attribution & Notices
3.1 You must retain all copyright notices, this License, and any NOTICE files.
3.2 For public Non-Commercial Use, You must provide Attribution in reasonable proximity to the Work (e.g., README, site footer).

# 4. Commercial Licensing
4.1 To obtain commercial rights, contact: licensing@qially.me with subject “QiLife-Eos Commercial License.”
4.2 Until a commercial license is executed and any required fees are paid in full, You have no right to any Commercial Use of the Work.

# 5. Restrictions
5.1 You may not remove or alter Attribution or this License in copies or substantial portions of the Work.
5.2 You may not sublicense the Work, in whole or part, except as necessary to host or build non-commercial forks with this License intact.
5.3 You may not use any trademarks, names, or logos of Licensor (including “QiAlly”, “QiLife”, “QiLife-Eos”) except for Attribution as defined herein or as permitted by separate written permission.

# 6. Contributions
6.1 By submitting any contribution (code, design, docs), You irrevocably license it to Licensor under this same License.
6.2 You represent that You have the right to grant such license and that Your contribution does not knowingly infringe third-party rights.

# 7. Warranty Disclaimer
THE WORK IS PROVIDED “AS IS” WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT. YOU ASSUME ALL RISKS.

# 8. Limitation of Liability
IN NO EVENT SHALL LICENSOR BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT, OR OTHERWISE, ARISING FROM, OUT OF, OR IN CONNECTION WITH THE WORK OR THIS LICENSE.

# 9. Termination
9.1 This License terminates automatically if You breach any term.
9.2 Upon termination, You must cease use and distribution of the Work and destroy copies in Your possession, except where retention is required by law.
9.3 Rights properly granted under an executed commercial license survive in accordance with that agreement.

# 10. Governing Law & Venue
This License is governed by the laws of the State of Indiana, USA, without regard to conflict-of-law rules. Exclusive venue for disputes shall be the state or federal courts located in Indiana, USA, and You consent to such jurisdiction and venue.

# 11. Severability
If any provision is held unenforceable, the remaining provisions shall remain in full force and effect.

# 12. Entire Agreement
This License constitutes the entire agreement between the parties regarding the Work’s Non-Commercial Use and supersedes all prior understandings. Commercial rights are only available by separate written license executed by Licensor.

— End of License —

# (Optional) NOTICE
## QiLife-Eos
***© QiAlly / Cody Rice-Velasquez • https://qially.me***

This project includes original designs, code, and documentation.
Non-Commercial Use is permitted with attribution under LICENSE.qilife-eos.
Commercial use requires a paid license from the Licensor.
