<p align="center">
  <a href="https://repowrit.com">
    <img src="https://repowrit.com/icon.svg" alt="RepoWrit" width="64" height="64" />
  </a>
</p>

<h1 align="center">RepoWrit</h1>

<p align="center">
  <strong>Documentation on Autopilot.</strong><br />
  Push code. Get docs, executive briefings, and architecture maps. That's it.
</p>

<p align="center">
  <a href="https://repowrit.com">Website</a> · <a href="https://repowrit.com/pricing">Pricing</a> · <a href="https://repowrit.com/changelog">Changelog</a> · <a href="https://github.com/RepoWrit/repowrit/issues">Community</a> · <a href="https://www.linkedin.com/company/repowrit">LinkedIn</a>
</p>

---

### What is RepoWrit?

RepoWrit is a GitHub App that turns your git history into executive briefings, architecture maps, and up-to-date documentation — powered by Claude 4.5.

Every commit triggers an AI analysis. Every analysis produces actionable output. No manual effort. No stale READMEs.

---

### How It Works

```mermaid
graph LR
    A["🔀 Git Commits"] -->|webhook| B["⚙️ RepoWrit Engine<br/><i>Claude 4.5</i>"]
    B --> C["📊 Executive Briefing"]
    B --> D["🗺️ Architecture Map"]
    B --> E["🔎 Ask RepoWrit"]
    B --> F["📄 Documentation PR"]
    B --> G["🛡️ PR Review"]
    B --> H["📅 Weekly Briefing Email"]
    B --> I["📈 Commit Timeline + CSV"]
    B --> J["🧮 Developer Scores"]
    B --> K["🧾 SOC 2 / Audit Export"]

    style A fill:#1e1e2e,stroke:#6366f1,color:#e4e4e7
    style B fill:#1e1e2e,stroke:#a78bfa,color:#e4e4e7
    style C fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style D fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style E fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style F fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style G fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style H fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style I fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style J fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
    style K fill:#1e1e2e,stroke:#818cf8,color:#e4e4e7
```

**1. Connect** — Install the GitHub App. Select your repositories. Multi-branch tracking is supported out of the box.

**2. Push** — Write code like normal. Every commit triggers RepoWrit. The first sync analyzes your last 3 commits instantly so you have a baseline.

**3. Ship** — Get AI-generated documentation PRs, executive summaries (Founder / PM / CTO), architecture visualizations, semantic search ("Ask RepoWrit"), PR reviews, and weekly briefings.

---

### Features at a glance

#### 🤖 AI-Native Documentation
- **Auto-generated docs** — README, CHANGELOG, and `docs/*.md` updates as PRs on every push
- **Self-correcting agent** — retries up to 3 times if CI fails on the doc PR
- **Multi-branch tracking** — track docs and metrics across every branch, not just `main`
- **Bring Your Own Key (BYOK)** — Anthropic, OpenAI, DeepSeek, or any compatible endpoint (AES-256-GCM encrypted at rest)

#### 📊 Executive Intelligence
- **Founder View** — knowledge moat %, documentation coverage, exit-readiness score, business impact
- **PM View** — velocity, energy distribution (features / bugs / refactor / docs / infra), Jira-aware sprint coverage
- **CTO View** — tech debt trends, architectural drift, security risk flags, dependency health
- **Weekly Email Briefings** — KPI row, achievements, top contributors, tech debt alerts every Monday
- **PDF Export** — one-click leadership-ready reports

#### 🗺️ Architecture & Code Intelligence
- **Architecture Map** — module layers, import relationships, dependency graphs (24 h cache, force-refresh on demand)
- **Ask RepoWrit** — plain-English semantic search across every commit, summary, and doc (powered by `text-embedding-3-small` + Claude 4.5)
- **Commit Timeline** — date-range slicing (1–730 days) with author / repo / branch filters and CSV export
- **Developer Scores** — cubic-weighted impact scoring that resists trivial-commit gaming

#### 🛡️ PR Reviews & Guardrails
- **Architecture Guardrail** — auto-review on every external PR with severity-graded comments
- **Risk flags** — flags missing docs, single-author modules, dependency drift, security-relevant changes
- **Tier-aware processing** — per-tier concurrency (1 → 20), queue priority, and resource limits

#### 🏢 Team & Enterprise
- **Organization dashboards** — shared org KPIs, code ownership, per-team rollups
- **Role-based access control** — Owner / Admin / Viewer with Supabase RLS isolation
- **Jira integration** — epic & ticket sync, PM-view enrichment
- **Governance & Compliance** — SOC 2-friendly exports, redaction tracking, tamper-evident audit trail (SHA-256 hashed)
- **Per-seat pricing** — Team ($20/seat/mo) and Enterprise ($49.99/seat/mo)

#### ⚙️ Developer Experience
- **30-second setup** — install the GitHub App, pick repos, done. No CI, no config files, no CLI.
- **Four themes** — Dark, Light, Ocean, Rosé — switch from any page
- **Privacy-first analytics** — PostHog identified-only, cookie-consent gated; Sentry for errors
- **5-day money-back guarantee** on every paid plan

---

### Who It's For

| Audience | What You Get |
|---|---|
| **Founders & CEOs** | Exit-readiness reports, knowledge moat analysis, business impact summaries |
| **Engineering Managers** | PM velocity panels, developer impact scores, effort distribution, Jira sync |
| **CTOs & Architects** | Tech debt trends, architecture maps, security risk flags, dependency analysis |
| **Developers** | Auto-generated READMEs, CHANGELOGs, doc PRs, and PR review comments — zero manual work |
| **Compliance & Ops** | SOC 2 exports, audit trails, governance reports (Team / Enterprise) |

---

### Privacy

Your full source code is **never stored long-term**. Diffs are processed in-memory by Claude 4.5 with **zero-retention** API settings and discarded immediately. Your code is never used to train any AI model. [Read our full privacy policy →](https://repowrit.com/privacy)

---

### Plans

| | Hobbyist | BYOK | Team | Enterprise |
|---|---|---|---|---|
| **Price** | Free | $4.99/mo | $20/seat/mo | $49.99/seat/mo |
| **Doc Generations** | 5/month | Unlimited | Unlimited | Unlimited |
| **Executive Views** | Founder | Founder + PM + CTO | Founder + PM + CTO | Founder + PM + CTO |
| **Ask RepoWrit (semantic search)** | 10/day | Unlimited | Unlimited | Unlimited |
| **Architecture Map** | ✓ | ✓ | ✓ | ✓ |
| **PR Reviews & Commit Timeline** | — | ✓ | ✓ | ✓ |
| **Weekly Email Briefings** | — | ✓ | ✓ | ✓ |
| **Jira Integration & Governance** | — | — | ✓ | ✓ |
| **PDF Export** | — | ✓ | ✓ | ✓ |
| **Analysis Window** | 24 hours | 7 days | 30 days | 30 days |
| **Bring Your Own AI Key** | — | ✓ | ✓ | ✓ |

[Get started free →](https://repowrit.com)

---

<p align="center">
  <sub>Built with conviction in India. Powered by Claude 4.5.</sub>
</p>
