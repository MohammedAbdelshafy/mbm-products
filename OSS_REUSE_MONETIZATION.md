# Open-Source Reuse & Monetization Plan
**Updated:** 2026-10-21  
**Operating rule:** Sell one narrow outcome before expanding engineering. Dr. Mia Dental remains the active priority; the other repositories are reusable delivery components or secondary offers, not a reason to start six new products.

## Executive decisions

1. **P0 — Dr. Mia Dental: close a paid founding pilot.** Lead with patient-access/front-desk workflow mapping, synthetic-data demo, approved FAQ/intake flow, and staff handoff design. The current `ai-front-desk` demo is local, synthetic-data-only, and not production-ready. Treat the previously proposed $500 pilot as a price hypothesis. Any paid scope must state which deliverables are design/configuration versus a live production deployment.
2. **P1 — DataClean AI / Lead Cleaner: sell a bounded CSV cleanup sprint.** Use a customer-authorized export, report duplicates/invalid/inconsistent fields, deliver a cleaned copy plus QA summary, and never write automatically into the canonical MBM lead database. Price-test a fixed-scope $99–$499 sprint depending on size/complexity; optional recurring cleanup is a hypothesis, not proven demand.
3. **P2 — Ads Audit service powered by Claude Ads.** Client supplies exports/screenshots and context; deliver evidence-backed findings, prioritized fixes, and a test plan. Price-test $199–$299 for a narrow first audit; larger scopes only after discovery. The Reel's $1,500 agency figure is an unverified marketing claim, not a price anchor or revenue forecast.
4. **P3 — ClipOps Studio / MBM-Social plus HyperFrames.** Add an optional HTML-to-MP4 rendering backend to the existing pipeline, not a replacement for the proven FFmpeg path. Package launch clips or short-form batches as done-for-you creative services after render quality and delivery cost are tested.
5. **P4 — Open Generative AI studio as a creative-service accelerator.** Use it to produce client-approved assets only after actual model/API cost and rights are understood. The README advertises a MuAPI white-label plan starting at $49/month, so “open source” does not mean unlimited zero-cost generations or free hosted service.
6. **Later / internal-first — Camofox, Fincept Terminal, Vibe-Trading.** Use Camofox for permitted public-site workflows and authorized browser QA, not access-control evasion. Use Fincept Terminal and Vibe-Trading for internal market research or paper-trading experiments, not promises of investment returns or a rushed financial product.

## Repository-to-existing-work map

| Upstream project | License / dependency note checked in repo | Reuse in existing MBM work | Monetizable deliverable | Priority / gate |
|---|---|---|---|---|
| [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | MIT. README promotes MuAPI white-label; pricing shown from $49/mo. | ClipOps Studio, MBM-Social creative workflows, customer ad assets. | Branded content-production service; price per approved asset/video bundle plus disclosed pass-through generation costs. | P4. First benchmark quality, cost per accepted asset, commercial rights, and provider dependency. Don't claim 600 models are locally hosted or free to run. |
| [AgriciDaniel/claude-ads](https://github.com/AgriciDaniel/claude-ads) | MIT. Reads campaign data and reports; documents draft-only optimization rather than silently changing live ad accounts. | Revenue Recovery / agency services; future read-only Ads Audit skill or MCP. | Audit report, prioritised repair backlog, measurement plan, optional monthly reporting. | P2. Start with client-provided exports. Redact secrets and personal data. Do not mutate ad accounts without explicit authorization. |
| [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | AGPL-3.0 dual-licensing notice in LICENSE. | Internal finance/research workspace; possible later MBM research content. | None as an immediate customer offer. | Later. Legal review required before redistributing, embedding, or offering a modified network-accessible service. Avoid scope creep. |
| [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | MIT. README includes paper-trading mode and explicit impersonation/token warning. | Internal research and educational content; possible later finance-terminal integration. | No immediate trading product. | Later. Paper accounts first; no live broker execution, personalised financial advice, or performance/return guarantees. |
| [jo-inc/camofox-browser](https://github.com/jo-inc/camofox-browser) | MIT. Provides browser automation and anti-detection features. | Website QA for Mia/MBM; authorized public-business research; future browser QA skill. | Setup/QA automation service only where sites and access methods permit it. | Internal-first. Respect terms, rate limits, privacy, authentication boundaries, CAPTCHAs and opt-outs. Never sell “bypass any wall” as a product promise. |
| [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | Apache-2.0; README specifies Node.js >=22 and deterministic HTML/CSS/media-to-MP4 rendering. | MBM-Social, ClipOps Studio, launch films, customer creative production. | Launch-video pack, branded explainers, or recurring short-form delivery. | P3. Prototype a reversible renderer adapter; preserve FFmpeg fallback and the existing quality/release gates. |

## Skills and MCPs: productize the work, not just the upstream code

### First three reusable packages

1. **Mia Dental Pilot Skill Pack** (internal first): discovery checklist, clinic configuration template, approved-FAQ content checklist, synthetic-demo runner, staff-handoff test plan, release/readiness checklist, and pilot report. Sell the workflow design and configured deliverable, not a claim that an unconnected agent is live.
2. **MBM DataClean MCP** (candidate): tools for validating a customer-authorized CSV, profiling schema/data quality, proposing deduplication keys, generating a cleaned downloadable artifact, and returning a QA report. Read input, write only a separate output artifact, require explicit confirmation, log provenance, and never silently edit `leads_database.json` or bypass DialerSingleWriter.
3. **Ads Audit Skill/MCP** (candidate): accept client-provided exports, identify missing tracking/measurement and suspicious metrics, create a source-linked report and test plan. Read-only by default, no account writes, and no fabricated ROI.

### Second wave

- **ClipOps Render MCP:** submit brand-approved HTML/media jobs to the HyperFrames adapter; return render status, QA summary, and MP4 artifact. Publishing remains a separate human-approved action.
- **Browser QA skill:** use Camofox/standard browser automation to test our own websites and customer-authorized environments; capture reproducible screenshots and findings.
- **Generative Creative skill:** choose from approved generation providers, estimate cost before execution, track source/rights and model, and package only outputs the client has approved.

### How the skill/MCP revenue works

- **One-time setup:** install/configure in the client's permitted runtime, map their fields, test, document, and train staff.
- **Managed recurring plan:** monitored workflow, versioned updates, run reports, and support, only once service cost and demand are proven.
- **Implementation premium:** connect to an existing customer workflow/PMS/CRM only after access, data rights, security, and acceptance criteria are documented.
- **Free distribution hook:** publish a genuinely useful, limited skill/template/demo; funnel users to a paid setup, audit, support or hosted implementation. Do not make the free artifact appear more capable than it is.
- **License discipline:** preserve copyright and license notices; check dependencies and provider terms; distinguish the upstream license from model/API, trademark, hosted-service, and data rights. Do not relabel third-party code as proprietary.

All listed prices are experiments, not validated market rates. Track conversations, qualified interest, proposal, payment, delivery time, inference/hosting/support cost, acceptance, and repeat demand separately.

## Dr. Mia first: execution queue

1. Confirm the current synthetic-data demo runs from the documented local command; preserve the explicit non-production warning.
2. Prepare a 3–5 minute demo with fictional patient data and show patient intake → dentist-facing summary → staff correction/handoff.
3. Offer a **$500 founding pilot hypothesis** with a written, bounded scope. State up front if the initial deliverable is workflow design/configuration/demo rather than a live clinic deployment.
4. Keep a **$99–$199 front-desk opportunity audit** as a fallback test only if a qualified buyer declines the pilot but will pay for a smaller diagnostic deliverable.
5. Revalidate the existing US dental-clinic list at send time and prepare a small personalized batch. Founder reviews every message; no unattended sends, and no Contec mailbox.
6. Measure replies, qualified conversations, confirmed pain, proposals and payments. Do not record a pilot as won before payment is confirmed.
7. Before live clinical use: complete the existing [production-hardening checklist](https://github.com/MohammedAbdelshafy/ai-front-desk/issues/1), qualified-dentist review, clinic approval, hosting/vendor/privacy review, consent, authentication/tenant isolation, webhook signature verification, idempotency/outbox/retries, staff handoff, retention/deletion, and backup/restore tests. Until then, no real patient data, live messaging, booking writes, diagnosis, prescribing, or medication recommendations.

## Suggested implementation sequence (only after evidence)

- **Now:** Dr. Mia buyer conversations and a truthful synthetic demo. No broad engineering.
- **Then:** DataClean service package and Claude Ads audit report template, using existing product entry points and customer-provided data.
- **After a paid creative job:** benchmark HyperFrames and add an optional render adapter in MBM-Social/ClipOps with regression tests and FFmpeg fallback.
- **After repeated customer demand:** build the narrow DataClean/Ads MCP tools with explicit input/output schemas, authentication, audit trail, rate limits and tests.
- **Later:** Open Generative AI, Camofox, Fincept Terminal and Vibe-Trading integrations only when a paid workflow justifies the dependency and licensing review.

## Existing source-of-truth links

- Dr. Mia / clinical reference build: https://github.com/MohammedAbdelshafy/ai-front-desk
- Dental production-hardening gates: https://github.com/MohammedAbdelshafy/ai-front-desk/issues/1
- Mia site, launch and sales kit: https://github.com/MohammedAbdelshafy/mia-ai-site
- Existing product index and buyer entry points: https://github.com/MohammedAbdelshafy/mbm-products
- Existing social publishing/render pipeline: https://github.com/MohammedAbdelshafy/MBM-Social
- Current revenue-first Dr. Mia mission: https://github.com/MohammedAbdelshafy/jarvis-mbm/issues/122
