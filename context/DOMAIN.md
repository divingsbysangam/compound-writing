# Technical & Domain Integrity Guide (DOMAIN.md)

This file defines the factual, technical, and domain standards for *Divings by Sangam*, specifically covering Salesforce, agentic AI, developer tooling, and systems architecture.

---

## Technical Rigor & Sourcing

1. **Release Notes PDF as Ground Truth**:
   - For any Salesforce release claims (Spring, Summer, Winter), the official release notes PDF is the sole source of truth.
   - If a feature or capability is not documented in the official release notes, do not claim it. Cancel or reframe.
2. **Field-Tested vs. Beta Transparency**:
   - State beta, pilot, or developer preview status plainly. Zero-caveat technical posts read like vendor marketing.
   - Field-tested claims must be empirically true and time-boxed when hands-on access has lapsed (e.g., "I ran this pipeline for seven months").
3. **No Client or Customer Org Data**:
   - Never reference client orgs, enterprise customer names, or production data.
   - All walkthroughs and demonstrations use personal projects, scratch orgs, and developer orgs exclusively.
4. **No Invented Metrics or Hypotheticals**:
   - Never fabricate statistics ("cuts time by 40%"). Use verified timings ("cut the cycle from 20 minutes to 3") or qualify as an estimate.
   - Clearly distinguish between actual observed behavior and hypothetical scenarios (use "suppose" or "imagine").
