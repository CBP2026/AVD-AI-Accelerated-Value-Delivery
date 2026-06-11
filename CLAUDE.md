# Knowledge Base — Accelerated Value Delivery (AVD)
*Iteration context for the AVD paper — KB v3.1 (June 2026)*

---

## Author

**CP** — Engagement Manager at OutSystems, with certifications in Product Management, Scrum Master, and Project Manager. No development background. In a short window in 2026, used Claude + AI to build and deploy 5–7 functional applications solving real problems — practical proof of the AI-first PM build model that AVD formalises.

---

## Current Document State

- **Live paper:** `avd_paper_v3_1.docx`
- **Previous:** `avd_paper_v3.docx` (annotated)
- **Older:** `avd_paper_v2.docx`, `ai_delivery_framework_paper.md` (v1)
- **Supporting:** `avd_workflow.html`, `avd_presentation.pptx` (both v1-aligned — slated for refresh)
- **Build script:** `outputs/build_v3.js` (regenerates the docx from source)

---

## Framework Positioning (v3.1 — confirmed)

**AVD does not position against traditional development.** The OS platform already collapsed lifecycles that traditional code-and-deploy approaches measured in months. AVD is the next compression on top of that — turbinating an already-fast cycle with AI, not fixing a broken one. The paper credits OS where it is due.

**Stack-agnostic by design.** The AI builds in whatever stack the approved toolchain supports. Where the OS platform is the target, output is either converted into OS via tooling under development by the R&D team, or — once the platform supports it natively — generated directly in OS. The framework's logic does not depend on which path applies.

**Outcome-based contracting** is mentioned briefly as a downstream implication; not delved into. Already being explored at OS.

---

## Language Discipline

- **No day predictions.** Headline language is qualitative: "compressed", "aggressively compressed", "a fraction of the traditional cycle". Specific day counts have been removed throughout to keep the framework defensible.
- **No "near-zero" defect claims.** Use "low and continuously validated" or similar.
- **No finger-pointing at OS or any specific vendor.** The framework is universal; OS is the platform the author works on.

---

## Framework Spine (the three phases + Living Backlog)

### Phase 1 — Inception & Accelerated Build (PM-led)
- Discovery is the **first activity of Phase 1**, not a precursor.
- Vision Brief (one page) is produced from the recorded discovery conversation and signed by the PO before build starts.
- AI extracts backlog candidates from the recording → seeds the Living Backlog.
- UX in Phase 1 is constraints only: existing design system as reference, or short greenfield grounding session.
- PM builds with approved AI toolchain. No user stories, no wireframe handoffs.
- AI-assisted QA continuous. Human QA spot review before handoff.
- **Commit summaries** are the sign-off mechanism: auto-generated per completed feature, naming what was built, the Living Backlog item it satisfies, and the tests that passed. PO approves with timestamp. Defined once in Section 5; referenced elsewhere.
- Acceptance criteria are anchored in the Vision Brief (outcome level) and refined per feature inside each commit summary. AI regenerates technical documentation from current code on demand for maintainers.

### Phase 2 — Technical Gate & Hardening
- PM coordinates parallel tracks: security scanning (automated), architecture review (by exception), compliance documentation (AI-generated), UX flow review.
- **Architect review by exception** against the pattern library. Conforming builds pass via fast lane; only novel or non-conforming patterns consume architect time. This is the bottleneck fix.
- **Pattern library cold-start** is honestly named: empty on project 1; architect reviews everything using standing principles; first project seeds the library. Fast lane begins from project 2.
- **Tiered blocker model:** deployment blockers (security, data exposure, critical compliance) return the build to the PM; non-blockers (UX, minor debt) go to Living Backlog.
- **Deployment Authority Envelope replaces CAB.** Phase 2 outputs (passing security + architecture + compliance) ARE the deployment authority within a pre-agreed risk envelope. Out-of-envelope changes (new external integrations, regulated-data changes, new auth surfaces) trigger asynchronous standing-authority review — not a scheduled meeting. This was the user's call to replace the Sonnet-4.6-introduced fast-track-CAB concept.

### Handoff to Run (boundary)
- AVD ends at deployment. PM builds, does not operate.
- Application enters the organisation's standard support/operations cycle (SRE, incident response, tiered support).
- Run may itself be re-examined under AI-first lens — explicitly out of scope for this paper.
- This boundary protects the PM from becoming a long-tail support owner.

### Phase 3 — Continuous Evolution via Stakeholder Sandboxing
- Certified stakeholders submit lightweight requests → IT provisions sandbox from standard template within SLA → sandbox includes synthetic data automatically.
- **Synthetic data simplified:** prerequisite for Phase 3, no real production data ever, structure mirrors production. Implementation detail is out of scope for the paper (deferred to later iteration).
- Stakeholders build in isolation → submit to community.
- PO defines eligible voter group per feature (direct use or direct impact, not seniority).
- Votes are signal; PO has final decision; rejections published; rejected ideas archived in Living Backlog with reason.
- Approved features pass through the same Phase 2 gate as the original build.
- Automated agents: duplicate detector, strategy monitor (resurfaces rejected ideas when objectives shift), auto-archive.

### Living Backlog (defined once)
- Connective tissue across all three phases.
- Sources: Phase 1 discovery, Phase 2 non-blocker findings, PO-initiated additions, Phase 3 rejected proposals.
- Every item has timestamp, originator, context. Nothing is lost.

---

## Governance Model

| Role | Traditional | AVD |
|------|-------------|-----|
| Product Owner | Backlog manager, story writer | Decision authority. Daily reviewer. Commit-summary sign-off owner. |
| Business Analyst | Requirements intermediary | Eliminated — direct PM-to-stakeholder conversation. |
| Architect / Tech Lead | Multi-week review | Compressed gate. Reviews by exception against the pattern library. |
| QA Tester | Post-sprint testing | AI-assisted QA continuous; human spot review before Phase 2 handoff. |
| UX Designer | Upfront wireframing | Grounding rules in Phase 1 (greenfield only); flow review in Phase 2. |
| PM / Engagement Manager | Coordinator | Primary builder in Phase 1; Phase 2 coordinator; hands off at deployment. |
| AVD Coach | N/A | First project only. Owned by a **central enablement function** (NOT absorbed by the PO). Lightweight on subsequent projects. |

---

## First-Project Prerequisites

1. AI toolchain procured and IT-approved
2. PM certified on the approved toolchain
3. Pattern library baseline (may be empty on project 1)
4. **Deployment authority envelope agreed** (replaces CAB negotiation)
5. AVD Coach identified — central enablement function
6. Sandbox infrastructure with template + provisioning SLA
7. Synthetic data capability (required for Phase 3, can be built in parallel with Phases 1–2)
8. Programme-level sandbox cost pre-approved
9. **Named backup PM** with equivalent toolchain certification (single-point-of-failure mitigation)

---

## Outcomes the Framework Targets (qualitative)

- Time to First Value: aggressively compressed from already-fast OS cycles
- Defect escape rate: low and continuously validated
- PO sign-off cadence: per feature (trigger-based)
- Idea-to-production: substantially compressed via sandbox → vote → Phase 2 → deploy
- Stakeholder engagement: direct, with governance
- Audit trail: built into build process via commit summaries

---

## Open Items for Future Iterations

- Refresh `avd_workflow.html` and `avd_presentation.pptx` to v3.1
- Bring back Failure Modes when boss-level review demands it
- Draft the pilot proposal (when ready)
- Decide whether to expose the 5–7 apps story as appendix (currently archived)
- Refine OS-specific conversion mechanics once R&D tooling matures

---

*KB v3.1 — Reflects all decisions through the 11-annotation review of v3 (June 2026)*