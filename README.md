# Klarity FHIR exhibits — catalog (35 chapters)

**Klarity Labs** publishes one small **Rust** library + CLI per topic—synthetic fixtures only, [MIT](https://opensource.org/licenses/MIT) reference code. 
This is an **exhibit hall**, not [HAPI](https://hapifhir.io/), [Firely](https://fire.ly/), or [Inferno](https://inferno.healthit.gov/).

- **Website:** [klaritylabs.ai](https://klaritylabs.ai/)
- **Contact:** sk@klaritylabs.ai
- **Org profile:** [klaritylabs-us](https://github.com/klaritylabs-us)

> **Published on GitHub:** exhibit repos **01–25** are live. Days **26–35** are listed below; links activate when each repo is published.

## How this relates to other tools

| Tool class | Role |
|------------|------|
| **HL7 FHIR Validator**, **HAPI**, **Firely** | Full validation, servers, SDKs, IG packages |
| **Inferno**, **Touchstone**, vendor cert suites | **Conformance** against test plans |
| **These exhibits** | **Pre-flight construction** on synthetic fixtures—catch shape mistakes before wire traffic |

Conformance tools test whether your **API behaves**; exhibits focus on whether your **payloads and pipes are built** to survive real partners.

## Start here (by role)

| If you care about… | Open these exhibits |
|--------------------|---------------------|
| USCDI / demographics & profiles | [01 Patient](https://github.com/klaritylabs-us/klarity-exhibit-01-us-core-patient), [07 MustSupport](https://github.com/klaritylabs-us/klarity-exhibit-07-us-core-mustsupport-slicing) |
| Patient Access / bulk download | [10 Bulk export](https://github.com/klaritylabs-us/klarity-exhibit-10-bulk-fhir-export), [25 $everything](https://github.com/klaritylabs-us/klarity-exhibit-25-patient-compartment-everything), [30 Async bulk polling](https://github.com/klaritylabs-us/klarity-exhibit-30-bulk-export-polling-async) |
| CMS & consumer/payer programs | [13 CMS-0057 map](https://github.com/klaritylabs-us/klarity-exhibit-13-cms-0057-patient-access-map), [14 CARIN BB](https://github.com/klaritylabs-us/klarity-exhibit-14-carin-blue-button) |
| SMART & security | [11 Backend services](https://github.com/klaritylabs-us/klarity-exhibit-11-smart-backend-services), [12 App launch](https://github.com/klaritylabs-us/klarity-exhibit-12-smart-app-launch), [28 Scope drift](https://github.com/klaritylabs-us/klarity-exhibit-28-smart-scope-capability-drift), [29 JWKS](https://github.com/klaritylabs-us/klarity-exhibit-29-jwks-backend-services) |
| Da Vinci / prior auth | [15 PDex](https://github.com/klaritylabs-us/klarity-exhibit-15-da-vinci-pdex), [16 PAS](https://github.com/klaritylabs-us/klarity-exhibit-16-da-vinci-pas), [17 CRD hooks](https://github.com/klaritylabs-us/klarity-exhibit-17-da-vinci-crd-hooks), [21 ATR roster](https://github.com/klaritylabs-us/klarity-exhibit-21-da-vinci-atr-roster) |
| Integration survival | [08 Search](https://github.com/klaritylabs-us/klarity-exhibit-08-fhir-search), [19 HL7v2 bridge](https://github.com/klaritylabs-us/klarity-exhibit-19-hl7v2-fhir-bridge), **[20 Fake door capstone](https://github.com/klaritylabs-us/klarity-exhibit-20-fake-door-integration)** |
| **Claims / EDI sketch edition** | **[22 Eligibility](https://github.com/klaritylabs-us/klarity-exhibit-22-eligibility-fhir-x12-map)**, [24 837P](https://github.com/klaritylabs-us/klarity-exhibit-24-x12-837p-claim-structure), [34 834 enrollment](https://github.com/klaritylabs-us/klarity-exhibit-34-x12-834-enrollment-coverage), [35 835 remittance](https://github.com/klaritylabs-us/klarity-exhibit-35-835-remittance-eob) |

**Onboarding path:** [01](https://github.com/klaritylabs-us/klarity-exhibit-01-us-core-patient) → [10](https://github.com/klaritylabs-us/klarity-exhibit-10-bulk-fhir-export) → [13](https://github.com/klaritylabs-us/klarity-exhibit-13-cms-0057-patient-access-map) → [20](https://github.com/klaritylabs-us/klarity-exhibit-20-fake-door-integration) → [22](https://github.com/klaritylabs-us/klarity-exhibit-22-eligibility-fhir-x12-map)

## Editions

| Edition | Days | Note |
|---------|------|------|
| **FHIR interoperability** | 1–21 (except 22), 23, 25–33 | US Core, REST, SMART, Da Vinci, documents, audit |
| **Claims / EDI sketch** | 22, 24, 34, 35 | Structural X12 + FHIR mapping—**not** adjudication or eligibility decisions |

## Full table (days 1–35)

| Day | Repo | Buyer pain (one line) |
|-----|------|------------------------|
| 1 | [us-core-patient](https://github.com/klaritylabs-us/klarity-exhibit-01-us-core-patient) | Bad demographics & identifiers break matching |
| 2 | [observation-vitals](https://github.com/klaritylabs-us/klarity-exhibit-02-us-core-observation-vitals) | Vitals without LOINC/UCUM fail analytics |
| 3 | [condition](https://github.com/klaritylabs-us/klarity-exhibit-03-us-core-condition) | Problem list bindings wrong at the sink |
| 4 | [medication-request](https://github.com/klaritylabs-us/klarity-exhibit-04-us-core-medication-request) | Rx intent/status/RxNorm gaps |
| 5 | [allergy](https://github.com/klaritylabs-us/klarity-exhibit-05-us-core-allergy) | Allergy negation & criticality |
| 6 | [docref-diagnosticreport](https://github.com/klaritylabs-us/klarity-exhibit-06-us-core-docref-diagnosticreport) | Labs/docs pipeline shape |
| 7 | [mustsupport-slicing](https://github.com/klaritylabs-us/klarity-exhibit-07-us-core-mustsupport-slicing) | MustSupport & slicing surprises |
| 8 | [fhir-search](https://github.com/klaritylabs-us/klarity-exhibit-08-fhir-search) | Search param handlers vs advertised CapabilityStatement |
| 9 | [validate-operation](https://github.com/klaritylabs-us/klarity-exhibit-09-fhir-validate-operation) | `$validate` request/response contract |
| 10 | [bulk-fhir-export](https://github.com/klaritylabs-us/klarity-exhibit-10-bulk-fhir-export) | Bulk manifest & NDJSON stream shape |
| 11 | [smart-backend-services](https://github.com/klaritylabs-us/klarity-exhibit-11-smart-backend-services) | Backend service JWT sketch |
| 12 | [smart-app-launch](https://github.com/klaritylabs-us/klarity-exhibit-12-smart-app-launch) | EHR launch config outline |
| 13 | [cms-0057-patient-access-map](https://github.com/klaritylabs-us/klarity-exhibit-13-cms-0057-patient-access-map) | Patient Access API surface map |
| 14 | [carin-blue-button](https://github.com/klaritylabs-us/klarity-exhibit-14-carin-blue-button) | Consumer-directed EOB patterns |
| 15 | [da-vinci-pdex](https://github.com/klaritylabs-us/klarity-exhibit-15-da-vinci-pdex) | Payer PDex shapes |
| 16 | [da-vinci-pas](https://github.com/klaritylabs-us/klarity-exhibit-16-da-vinci-pas) | PAS preauth Claim shape |
| 17 | [da-vinci-crd-hooks](https://github.com/klaritylabs-us/klarity-exhibit-17-da-vinci-crd-hooks) | CRD hook + prefetch contract |
| 18 | [plan-net-directory](https://github.com/klaritylabs-us/klarity-exhibit-18-plan-net-directory) | Provider directory PractitionerRole |
| 19 | [hl7v2-fhir-bridge](https://github.com/klaritylabs-us/klarity-exhibit-19-hl7v2-fhir-bridge) | v2 ADT seed → FHIR sketch |
| 20 | [fake-door-integration](https://github.com/klaritylabs-us/klarity-exhibit-20-fake-door-integration) | 200 OK but broken Bundle graphs |
| 21 | [da-vinci-atr-roster](https://github.com/klaritylabs-us/klarity-exhibit-21-da-vinci-atr-roster) | ATR/roster attribution shape |
| 22 | [eligibility-fhir-x12-map](https://github.com/klaritylabs-us/klarity-exhibit-22-eligibility-fhir-x12-map) | Eligibility FHIR + 271 sketch |
| 23 | [fhir-consent-exchange](https://github.com/klaritylabs-us/klarity-exhibit-23-fhir-consent-exchange) | Consent for exchange |
| 24 | [x12-837p-claim-structure](https://github.com/klaritylabs-us/klarity-exhibit-24-x12-837p-claim-structure) | 837P / professional Claim structure |
| 25 | [patient-compartment-everything](https://github.com/klaritylabs-us/klarity-exhibit-25-patient-compartment-everything) | Compartment & `$everything` |
| 26 | [operationoutcome-error-semantics](https://github.com/klaritylabs-us/klarity-exhibit-26-operationoutcome-error-semantics) | Partner-debuggable API errors |
| 27 | [provenance-auditevent-access](https://github.com/klaritylabs-us/klarity-exhibit-27-provenance-auditevent-access) | Access audit evidence |
| 28 | [smart-scope-capability-drift](https://github.com/klaritylabs-us/klarity-exhibit-28-smart-scope-capability-drift) | SMART scopes vs server capability |
| 29 | [jwks-backend-services](https://github.com/klaritylabs-us/klarity-exhibit-29-jwks-backend-services) | JWKS rotation shape |
| 30 | [bulk-export-polling-async](https://github.com/klaritylabs-us/klarity-exhibit-30-bulk-export-polling-async) | Bulk async poll JSON |
| 31 | [patient-match-mpi](https://github.com/klaritylabs-us/klarity-exhibit-31-patient-match-mpi) | `$match` / MPI parameters |
| 32 | [ccda-document-bundle](https://github.com/klaritylabs-us/klarity-exhibit-32-ccda-document-bundle) | Document Bundle + Composition |
| 33 | [search-include-chains](https://github.com/klaritylabs-us/klarity-exhibit-33-search-include-chains) | `_include` graph integrity |
| 34 | [x12-834-enrollment-coverage](https://github.com/klaritylabs-us/klarity-exhibit-34-x12-834-enrollment-coverage) | 834 → Coverage sketch |
| 35 | [835-remittance-eob](https://github.com/klaritylabs-us/klarity-exhibit-35-835-remittance-eob) | 835 → EOB sketch |

## Security

Exhibits use **synthetic fixtures only** (no PHI). Reporting and scope: see **[SECURITY.md](./SECURITY.md)** in this repo. Each exhibit repo also has its own `SECURITY.md` at the repository root.

## License

Each exhibit repo is **MIT** unless noted. Synthetic data only; not legal or clinical advice.

**Need this on your payloads or API?** 20-minute FHIR Scan — sk@klaritylabs.ai · [klaritylabs.ai](https://klaritylabs.ai/)

## What we do commercially

Independent **verification** (Klarity Sentinel™) and engineering services—see [klaritylabs.ai](https://klaritylabs.ai/). 
Exhibits do not ship the Sentinel engine or licensed rule packs.
