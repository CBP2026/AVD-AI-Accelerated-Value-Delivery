# AVD Framework — Project Structure

Complete documentation and assets for the Accelerated Value Delivery framework.

---

## 📂 Directory Layout

```
AVD-AI-Accelerated-Value-Delivery/
├── README.md                          # Start here — overview & quick links
├── ai_delivery_framework_paper.md     # Main framework paper (v1.0) — 8 sections
├── AVD_knowledge_base.md              # Portuguese knowledge base — detailed governance
├── CLAUDE.md                          # Project context & iterations (v3.1)
├── PROJECT_STRUCTURE.md               # This file
│
├── docs/
│   └── avd_workflow.html              # Interactive workflow visualization
│
└── GETTING_STARTED.md                 # Coming: Setup & usage guide
```

---

## 📖 What Each File Contains

### **README.md**
Your entry point. Contains:
- Framework overview
- The three phases (1-sentence summaries)
- Quick metrics comparison
- Security & governance models
- How to use each document

**Read this first if:** You want a 5-minute overview

---

### **ai_delivery_framework_paper.md**
The complete AVD framework specification. Contains:
- Abstract & problem statement
- The AI inflection point
- Phase 1: Rapid Discovery & MVP Build (Days 1–3)
- Phase 2: Technical Review & Hardening (Days 4–5)
- Phase 3: Continuous Evolution via Stakeholder Sandboxing
- Governance model (6 roles)
- Training & certification approach
- Security model (5 layers)
- Key metrics & conclusions

**Read this if:** You need the full framework specification (~12K words)

---

### **AVD_knowledge_base.md**
Extended knowledge base in Portuguese. Contains:
- Author background
- Framework premises
- Detailed phase descriptions
- Governance model (with tables)
- Security model (5 layers)
- Training requirements
- Gap analysis (9 gaps + solutions)
- Target metrics
- Deliverables & next steps

**Read this if:** You need governance details or are implementing the framework

---

### **CLAUDE.md**
Project iteration context (v3.1). Contains:
- Author bio
- Document state & version history
- Framework positioning
- Language discipline (what language to use)
- Framework spine (3 phases + Living Backlog)
- Governance model
- First-project prerequisites (9 items)
- Target outcomes
- Open items for future iterations

**Read this if:** You're iterating on the framework or implementing it

---

### **docs/avd_workflow.html**
Interactive visual workflow. Features:
- Dark theme design
- Comparison bar: Traditional Agile vs. AVD (3-4 months vs. 1 week)
- Timeline showing all 3 phases
- Role evolution cards
- Security defense pillars
- Key metrics cards
- Responsive design (mobile-friendly)

**Use this if:** You want a visual overview or need to present the framework

---

## 🎯 How to Read This Repository

### **If you have 5 minutes**
→ Read `README.md`

### **If you have 30 minutes**
→ Read `README.md` + open `docs/avd_workflow.html` in a browser

### **If you have 1 hour**
→ Read `ai_delivery_framework_paper.md` (all 8 sections)

### **If you're implementing the framework**
→ Read everything in this order:
1. `README.md` (overview)
2. `ai_delivery_framework_paper.md` (specification)
3. `AVD_knowledge_base.md` (detailed governance)
4. `CLAUDE.md` (iteration context)
5. `docs/avd_workflow.html` (visual reference)

### **If you're iterating on the framework**
→ Focus on:
1. `CLAUDE.md` (current state & decisions)
2. `ai_delivery_framework_paper.md` (what to update)
3. `AVD_knowledge_base.md` (governance implications)

---

## 🔑 Key Concepts to Know

### Vision Brief
One-page artefact from discovery: problem, goals, metrics, scope. Signed by PO before build starts.

### Living Backlog
Continuously maintained record across all phases. Sources: Phase 1 discovery, Phase 2 non-blockers, PO additions, Phase 3 rejections. Nothing is lost.

### Commit Summary
Auto-generated per completed feature: what was built, Living Backlog item satisfied, tests passed. PO approval with timestamp = audit trail.

### Pattern Library
Architect Review Board's catalogue of approved patterns. Phase 2 validates against it (review by exception).

### Deployment Authority Envelope
Pre-agreed boundary where Phase 2 outputs ARE the authorization. Out-of-envelope changes trigger standing-authority review.

### Sandbox
Isolated environment for certified stakeholders to build features. Zero risk to production. Uses synthetic data only.

---

## 📊 Framework at a Glance

| Aspect | Traditional | AVD |
|--------|-------------|-----|
| **Time to First Value** | 3–4 months | 1 week |
| **Build Leader** | Dev team | PM + AI |
| **User Stories** | Required | Eliminated |
| **QA Timing** | Post-sprint | Real-time embedded |
| **Architecture Review** | Multi-week | 1–2 day gate (by exception) |
| **Scope Management** | Sprint planning | Vision Brief + AI alerts |
| **Feature Evolution** | PO-bottleneck | Community sandboxes |
| **Rejected Ideas** | Deleted | Archived with context |
| **Audit Trail** | Documentation | Built into commits |

---

## ✅ Prerequisites for First Project

Before launching:
1. ✅ AI toolchain procured & IT-approved
2. ✅ PM certified on toolchain
3. ✅ Pattern library baseline
4. ✅ Deployment authority envelope agreed
5. ✅ AVD Coach identified
6. ✅ Sandbox infrastructure with SLA
7. ✅ Synthetic data layer (or parallel development)
8. ✅ Programme-level cost pre-approved
9. ✅ Named backup PM certified

---

## 🚀 Next Steps

- [ ] Review all documentation
- [ ] Map framework to your organization
- [ ] Identify AI toolchain candidates
- [ ] Identify first project candidate
- [ ] Establish pattern library baseline
- [ ] Plan synthetic data layer
- [ ] Set up sandbox infrastructure
- [ ] Begin first AVD project

---

## 🔗 GitHub Repository

**AVD-AI-Accelerated-Value-Delivery**  
https://github.com/CBP2026/AVD-AI-Accelerated-Value-Delivery

Clone: `git clone https://github.com/CBP2026/AVD-AI-Accelerated-Value-Delivery.git`

---

**Last Updated:** June 11, 2026  
**Framework Version:** v3.1  
**Author:** CP — Engagement Manager, OutSystems