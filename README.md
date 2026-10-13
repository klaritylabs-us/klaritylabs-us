# Klarity Labs — FHIR exhibit series

We help U.S. payer–provider teams **verify and harden FHIR and integration payloads** before production traffic. Public repos here are **read-only reference exhibits**—small Rust checkers and cited READMEs—not our product engine and **not** a replacement for [HAPI](https://hapifhir.io/), [Firely](https://fire.ly/), or [Inferno](https://inferno.healthit.gov/).

> **Published on GitHub: https://github.com/klaritylabs-us/klarity-fhir-exhibits; links go live as each repo is published.

## How this relates to other tools

| Tool class | Role |
|------------|------|
| **HL7 FHIR Validator**, **HAPI**, **Firely** | Full validation, servers, SDKs, IG packages |
| **Inferno**, **Touchstone**, vendor cert suites | **Conformance** against test plans |
| **These exhibits** | **Pre-flight construction** on synthetic fixtures—catch shape mistakes before wire traffic |

Conformance tools test whether your **API behaves**; exhibits focus on whether your **payloads and pipes are built** to survive real partners.

## What these repos are

| You get | You do not get |
|--------|----------------|
| Spec-grounded **construction** checks on synthetic JSON/X12 sketches | A full FHIR server, SDK, or IG runtime |
| One integration pain per repo (tables: “what breaks”) | ONC certification or “passed Inferno = production safe” |
| MIT reference code + CLI exit codes | Issues/PRs, releases, or supported libraries |

**Start here:** [Exhibit catalog](https://github.com/klaritylabs-us/klarity-fhir-exhibits) (table of all days) · **Onboarding path:** [01 Patient](https://github.com/klaritylabs-us/klarity-exhibit-01-us-core-patient) → [10 Bulk](https://github.com/klaritylabs-us/klarity-exhibit-10-bulk-fhir-export) → [13 CMS-0057 map](https://github.com/klaritylabs-us/klarity-exhibit-13-cms-0057-patient-access-map) → [20 Fake door](https://github.com/klaritylabs-us/klarity-exhibit-20-fake-door-integration) → [22 Eligibility sketch](https://github.com/klaritylabs-us/klarity-exhibit-22-eligibility-fhir-x12-map)

**Editions:** **FHIR interoperability** (days 1–21, 23, 25–33) · **Claims / EDI sketch** (22, 24, 34, 35)—structural only, not payment or eligibility decisions.

**Need this on your payloads or API?** 20-minute FHIR Scan — **sk@klaritylabs.ai** · [klaritylabs.ai](https://klaritylabs.ai/)

**Commercial work:** [klaritylabs.ai](https://klaritylabs.ai/) · Independent verification (Klarity Sentinel™) and engineering services—exhibits do not ship the Sentinel engine or licensed rule packs.
