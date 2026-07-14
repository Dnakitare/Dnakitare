# Daniel Nakitare

Backend systems where the consequences are real. Healthcare, regulated industries, the trust substrate for AI agents. Former 101st Airborne (Purple Heart). MBA.

📍 Rio Rancho, NM · [dnakitare.github.io](https://dnakitare.github.io) · [LinkedIn](https://linkedin.com/in/dnakitare)

---

### What I do

Senior Software Engineer at Carefeed. I own the backend integration architecture across 9+ external EHR and healthcare platforms (Epic, PointClickCare, MatrixCare): data exchange, webhook infrastructure, PDF/OCR pipelines for hundreds of facilities, and the identity and auth layer behind a multi-tenant SaaS platform. I inherited a four-year backlog of 27,000+ failed uploads, fixed the root cause, and shipped the cleanup tooling that brought integrity back above 99%. PHP and Laravel are my primary production stack.

Before Carefeed: API and integration infrastructure at legal-tech (nQ Zebraworks) and behavioral-health (Sensible Care) SaaS. Seven years of shipping production backends where a wrong record is a real-world problem, not a failed unit test.

---

### Backend and integration

**[laravel-outbox](https://github.com/Dnakitare/laravel-outbox)** — Transactional outbox for Laravel. Domain events are persisted atomically with the data that produced them, so a committed write and its event can never disagree.

---

### The trust substrate for AI agents

This is where my side work concentrates: the infrastructure *around* an LLM, not the model itself. The LLM is the easy part. The interesting work is everything around it.

**[imara](https://github.com/Dnakitare/imara)** — Runtime governance proxy for the Model Context Protocol. Intercepts every tool call, evaluates it against YAML policy (allow, deny, rate-limit, escalate), and records every decision to a tamper-evident, SHA-256 hash-chained audit log (genesis-anchored, with truncation detection). Published on npm. Composes with Mavryn.

**[mavryn](https://github.com/Dnakitare/mavryn)** — MCP gateway. Proxies many upstream MCP servers behind a single endpoint, with tool namespacing, semantic search across tools, policy, and a hash-chained audit trail. Where Imara governs one server's calls, Mavryn routes across many. They are two layers of the same stack.

**[prior-auth-assistant](https://github.com/Dnakitare/prior-auth-assistant)** — A HIPAA-shaped reference architecture for healthcare AI. Postgres row-level security, field-level PHI encryption, HMAC-chained audit, prompt-injection hardening, and magic-byte upload validation wrapped around a Claude OCR and extraction pipeline. 99 tests, CI against SQLite and Postgres.

**[aether](https://github.com/Dnakitare/aether)** — AI-agent runtime with hardware-level isolation via Firecracker microVMs. A single-region control plane: in-process scheduler (bin-packing, spread, best-fit placement), multi-tenant RBAC, PostgreSQL state, and Kubernetes and Terraform deployment. Beta.

---

### Shipped

**[PhotoPare](https://apps.apple.com/app/id6762467066)** — Privacy-first iOS app built on Apple's Vision framework: duplicate, blur, and screenshot cleanup, fully on-device, no tracking. On the App Store with a one-time unlock.

---

### Background

Former 11B infantryman, U.S. Army 101st Airborne Division (Combat Infantry Badge, Purple Heart, Afghanistan). MBA, Temple University (Fox). BA, Pomona College.

<sub>深層降下 — <a href="https://dnakitare.github.io/strata-dive/">nine layers down, arrive quietly</a></sub>
