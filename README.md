# Hi, I'm Derek

I build AI agents and automation that live **inside Microsoft 365** —
Copilot Studio agents that cite their sources and escalate when they're not
sure, Power Automate flows with retry and dedupe baked in, RAG pipelines
that ship with eval harnesses, and consolidation models that actually tie
out.

Most "AI on M365" work I see is either a tenant-admin checking a Copilot
license box, or a generic AI consultant who's never touched a Power Platform
connector. I do both halves: the AI behaviour (grounding, citations,
escalation, evals) **and** the M365 plumbing (SharePoint, Power Automate,
Fabric, DLP, privacy config).

> **Available for hire.** Happy to start with a paid 1-hour scoping call.

---

## Capability demos

Each repo below ships with sample data, a one-command setup, an eval harness,
and a green CI badge. Clone, run, see it work — or click the live-demo link
where one exists.

### Runnable demos (13)

| | Repo | What it shows | CI | Live |
|---|---|---|---|---|
| 🤖 | **[copilot-studio-support-agent](https://github.com/derekgallardo01/copilot-studio-support-agent)** | Microsoft 365 AI agent that cites SharePoint docs and escalates sensitive topics. Multi-turn conversation, two worked corpora (workplace + SaaS support), 30-case eval harness. | [![CI](https://github.com/derekgallardo01/copilot-studio-support-agent/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/copilot-studio-support-agent/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/copilot-studio-support-agent/)** |
| 🔁 | **[power-automate-flow-pack](https://github.com/derekgallardo01/power-automate-flow-pack)** | Scheduled M365 sync with retry, idempotent dedupe, dead-letter queue, and dry-run mode. Two scenario sets (Asana + Microsoft Forms), 14 end-to-end eval cases. | [![CI](https://github.com/derekgallardo01/power-automate-flow-pack/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/power-automate-flow-pack/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/power-automate-flow-pack/)** |
| 📊 | **[powerbi-fabric-consolidation](https://github.com/derekgallardo01/powerbi-fabric-consolidation)** | Multi-entity consolidation (different charts of accounts) into one dashboard with unmapped-account report and variance alerts. Two datasets (campgrounds + hospitality). | [![CI](https://github.com/derekgallardo01/powerbi-fabric-consolidation/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/powerbi-fabric-consolidation/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/powerbi-fabric-consolidation/)** |
| 🏢 | **[sharepoint-intranet-generator](https://github.com/derekgallardo01/sharepoint-intranet-generator)** | Full SharePoint intranet generated from one JSON definition, with schema validation. Two industry templates (professional services + manufacturing). | [![CI](https://github.com/derekgallardo01/sharepoint-intranet-generator/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/sharepoint-intranet-generator/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/sharepoint-intranet-generator/)** |
| 📚 | **[rag-over-docs-kit](https://github.com/derekgallardo01/rag-over-docs-kit)** | RAG kit with citation-first answers (document + chunk per claim), a query-aware re-ranker, and a golden eval set. Two corpora (workplace + technical API docs). | [![CI](https://github.com/derekgallardo01/rag-over-docs-kit/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/rag-over-docs-kit/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/rag-over-docs-kit/)** |
| 💬 | **[nocode-ai-lead-workflow](https://github.com/derekgallardo01/nocode-ai-lead-workflow)** | Lead triage with cross-channel dedupe and a human-review queue for low-confidence classifications. Two leads datasets (B2B SaaS + real estate). | [![CI](https://github.com/derekgallardo01/nocode-ai-lead-workflow/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/nocode-ai-lead-workflow/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/nocode-ai-lead-workflow/)** |
| 🛡️ | **[m365-audit-mcp](https://github.com/derekgallardo01/m365-audit-mcp)** | **MCP server** exposing M365 privacy/compliance audit checks as tools any MCP client (Claude Desktop, Cursor) can call. Five tools, 11 unit tests, mocked tenant backend with documented Microsoft Graph swap point. | [![CI](https://github.com/derekgallardo01/m365-audit-mcp/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/m365-audit-mcp/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/m365-audit-mcp/)** |
| 🧠 | **[claude-agent-sdk-example](https://github.com/derekgallardo01/claude-agent-sdk-example)** | **Claude Agent SDK** demo — production-shaped multi-tool agent: coordinator + 4 tools (search/memory/grade) + session memory + citation tracking. Stub-by-default; one env var swaps to the real Claude API. 16 tests + 5 golden evals. | [![CI](https://github.com/derekgallardo01/claude-agent-sdk-example/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/claude-agent-sdk-example/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/claude-agent-sdk-example/)** |
| 🪟 | **[m365-agents-sdk-example](https://github.com/derekgallardo01/m365-agents-sdk-example)** | **Microsoft 365 Agents SDK** demo — declarative manifest + 5 typed handlers + 4 Graph connectors + channel-aware rendering (Teams chat / Outlook HTML email / Copilot canvas adaptive card). 25 tests + 6 golden evals. | [![CI](https://github.com/derekgallardo01/m365-agents-sdk-example/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/m365-agents-sdk-example/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/m365-agents-sdk-example/)** |
| 📄 | **[pdf-extraction-kit](https://github.com/derekgallardo01/pdf-extraction-kit)** | Schema-driven PDF extraction with pluggable backends (regex by default, LLM swap via one env var), per-field confidence scores, and a golden eval harness asserting **exact extracted values** per fixture per field. 3 schemas (invoice/contract/statement), 6 fixtures, 23 tests + 12 golden evals. | [![CI](https://github.com/derekgallardo01/pdf-extraction-kit/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/pdf-extraction-kit/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/pdf-extraction-kit/)** |
| 🗂️ | **[document-classifier-kit](https://github.com/derekgallardo01/document-classifier-kit)** | Schema-driven document classifier with confidence-routed human review and a golden eval harness reporting per-class precision / recall / F1. 6-class default catalog (invoice, PO, contract, complaint, job application, spam), 7 fixtures, 23 tests + 7 golden evals. Pairs with `pdf-extraction-kit` as a doc-intake pipeline. | [![CI](https://github.com/derekgallardo01/document-classifier-kit/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/document-classifier-kit/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/document-classifier-kit/)** |
| 🧪 | **[prompt-registry-kit](https://github.com/derekgallardo01/prompt-registry-kit)** | Versioned prompt registry with A/B variants, eval-gated promotion, and instant rollback. The production-ops piece every LLM build needs once *"we changed the prompt"* becomes the most common root cause of outages. 3 bundled prompts × 2 versions each, 5 rubric types, 36 tests + 12 golden evals. | [![CI](https://github.com/derekgallardo01/prompt-registry-kit/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/prompt-registry-kit/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/prompt-registry-kit/)** |
| 📬 | **[email-triage-automation](https://github.com/derekgallardo01/email-triage-automation)** | End-to-end inbox triage: parse incoming emails → classify → route to the right queue (sales / support / billing / etc.) → draft a reply where appropriate → send low-confidence cases to human review. 6-class default catalog, 7 EML fixtures, two eval suites (classification P/R/F1 + draft quality), 33 tests + 10 golden evals. Composes `document-classifier-kit` + `prompt-registry-kit` patterns into a complete vertical app. | [![CI](https://github.com/derekgallardo01/email-triage-automation/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/email-triage-automation/actions/workflows/ci.yml) | **[demo →](https://derekgallardo01.github.io/email-triage-automation/)** |

### Delivery & enablement kits (4)

Templates I use on every engagement, with two fully worked examples each
and a placeholder linter so half-finished docs don't reach a client.

| | Repo | What it covers | CI |
|---|---|---|---|
| 📝 | **[ms-delivery-discovery-kit](https://github.com/derekgallardo01/ms-delivery-discovery-kit)** | Discovery questionnaire + statement-of-work template. Two worked engagements (logistics SMB + law firm). | [![CI](https://github.com/derekgallardo01/ms-delivery-discovery-kit/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/ms-delivery-discovery-kit/actions/workflows/ci.yml) |
| 🏗️ | **[solution-architecture-hld](https://github.com/derekgallardo01/solution-architecture-hld)** | HLD document + Mermaid diagram templates. Two worked HLDs (scheduled ETL + AI agent). | [![CI](https://github.com/derekgallardo01/solution-architecture-hld/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/solution-architecture-hld/actions/workflows/ci.yml) |
| 📦 | **[project-handover-pack](https://github.com/derekgallardo01/project-handover-pack)** | Handover guide + runbook + Loom-script templates. Two worked handovers. | [![CI](https://github.com/derekgallardo01/project-handover-pack/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/project-handover-pack/actions/workflows/ci.yml) |
| 🔒 | **[m365-privacy-config](https://github.com/derekgallardo01/m365-privacy-config)** | M365 + Copilot privacy configuration checklist. Two worked checklists (regulated advisory + US healthcare under HIPAA BAA). | [![CI](https://github.com/derekgallardo01/m365-privacy-config/actions/workflows/ci.yml/badge.svg)](https://github.com/derekgallardo01/m365-privacy-config/actions/workflows/ci.yml) |

---

## How I work

- **Discovery before quoting.** I use the
  [discovery + SOW kit](https://github.com/derekgallardo01/ms-delivery-discovery-kit)
  on every engagement so out-of-scope and acceptance criteria are
  written down, not assumed.
- **Eval-gated AI.** No AI build ships without a golden eval set that
  gates the CI. If we can't measure "did this prompt change make things
  better or worse", we shouldn't deploy it.
- **Handover is the deliverable.** A
  [handover guide + runbook + 3-min walkthrough video](https://github.com/derekgallardo01/project-handover-pack)
  ships at the end of every engagement so a non-developer owner can
  maintain what I built.
- **Privacy first for AI on M365.** Regulated clients get the
  [privacy-config checklist](https://github.com/derekgallardo01/m365-privacy-config)
  signed off before any Copilot / Azure OpenAI work touches their tenant.

---

## Stack I work in

**Microsoft:** Copilot Studio · Power Automate · Power BI / Fabric ·
SharePoint Online · Microsoft Teams · Entra ID · Purview / DLP · Azure
OpenAI

**AI engineering:** RAG (retrieval + re-ranking + grounding) · evaluation
harnesses · LLM provider integration (Azure OpenAI, Anthropic) · safety
& human-in-the-loop patterns

**No-code adjacents:** Make.com · Zapier · n8n (mapping into Power
Automate via the [blueprint](https://github.com/derekgallardo01/nocode-ai-lead-workflow/blob/main/blueprint.md))

---

## Worth knowing

- Stdlib-only Python wherever possible — these demos clone-and-run on a
  fresh laptop with no `pip install`.
- Every repo has a CI badge that's currently green. The eval harnesses
  gate every push so the demos don't bit-rot.
- Dockerfiles on all six runnables — `docker build && docker run` works
  on any machine with Docker, no Python install needed.
