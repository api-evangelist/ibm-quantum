# IBM Quantum (ibm-quantum)

IBM Quantum is IBM's quantum computing program — operator of the IBM Quantum Platform (quantum.cloud.ibm.com), publisher of the open-source Qiskit SDK, and provider of the Qiskit Runtime REST API for submitting Sampler and Estimator primitive jobs against 100+ qubit Heron-generation QPUs and managed simulators. The platform combines an Apache-2.0 software stack (Qiskit, qiskit-ibm-runtime, qiskit-ibm-catalog, Qiskit Aer, Qiskit Serverless, Qiskit Functions) with a tiered access model (Open / Pay-As-You-Go / Flex / Premium / On-Premises) and is the longest-running commercial quantum computing API surface in the industry.

**URL:** [Visit APIs.yml](https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - IBM Quantum, Quantum Computing, Qiskit, Qiskit Runtime, Qiskit Functions, OpenQASM, Quantum Hardware

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Plans

| Plan | Pricing | Notes |
|---|---|---|
| Open | Free | 10 quantum compute minutes per 28-day rolling window; 180-minute / 12-month opt-in bonus |
| Pay-As-You-Go | Per-second metered ($1.60 / second of QPU time) | No commitment, billed in arrears |
| Flex | $72 / minute, $30,000 minimum, 12-month pool | Premium-level access without an annual subscription |
| Premium | $48 / minute, annual subscription (5,200 minute floor) | Qiskit Functions + Qiskit Transpiler as a Service |
| On-Premises | Contact IBM | Dedicated on-premises quantum system |

## APIs

### Qiskit Runtime Jobs API
Submit Qiskit Runtime primitive jobs (Sampler and Estimator) to IBM Quantum hardware. Includes creation, listing, retrieval, deletion, cancellation, results, logs, metrics, and tag management. POST /v1/jobs is rate-limited to 5 requests / minute per IAM token.

**Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

- [OpenAPI](openapi/ibm-quantum-runtime-jobs-openapi.yml)
- [JSON Schema — Job](json-schema/ibm-quantum-job-schema.json)
- [JSON-LD context](json-ld/ibm-quantum-context.jsonld)
- [Naftiko Capability — Runtime Jobs](capabilities/runtime-jobs.yaml)
- [Example — Create Sampler job](examples/ibm-quantum-create-sampler-job-example.json)

### Qiskit Runtime Backends API
Discover available IBM Quantum backends (Heron, Eagle QPUs plus simulators). Read backend configuration, calibrated properties, defaults, and live status for circuit transpilation and scheduling.

- [OpenAPI](openapi/ibm-quantum-runtime-backends-openapi.yml)
- [JSON Schema — Backend](json-schema/ibm-quantum-backend-schema.json)
- [Naftiko Capability — Runtime Backends](capabilities/runtime-backends.yaml)
- [Example — List backends](examples/ibm-quantum-list-backends-example.json)

### Qiskit Runtime Sessions API
Create, inspect, update, and close Qiskit Runtime sessions for grouping primitive jobs against a target backend with priority access. Supports `dedicated` and `batch` modes.

- [OpenAPI](openapi/ibm-quantum-runtime-sessions-openapi.yml)
- [JSON Schema — Session](json-schema/ibm-quantum-session-schema.json)
- [Naftiko Capability — Runtime Sessions](capabilities/runtime-sessions.yaml)
- [Example — Create session](examples/ibm-quantum-create-session-example.json)

### Qiskit Runtime Instances API
Inspect the current Qiskit Runtime instance, view instance limits and configuration, and read per-account configuration. Instances are identified by IBM Cloud Service-CRN and govern plan, allocation, region, and access.

- [OpenAPI](openapi/ibm-quantum-runtime-instances-openapi.yml)
- [Naftiko Capability — Runtime Instances](capabilities/runtime-instances.yaml)

### Qiskit Runtime Analytics API
Usage analytics and active-workload reporting for a Qiskit Runtime instance. Powers FinOps reporting and minute-pool utilization tracking across Open, Pay-As-You-Go, Flex, and Premium plans.

- [OpenAPI](openapi/ibm-quantum-runtime-analytics-openapi.yml)
- [Naftiko Capability — Runtime Analytics](capabilities/runtime-analytics.yaml)

### Qiskit Runtime Versions API
Discover supported versions of the Qiskit Runtime REST API and negotiate the date-based `IBM-API-Version` header value.

- [OpenAPI](openapi/ibm-quantum-runtime-versions-openapi.yml)
- [Naftiko Capability — Runtime Versions](capabilities/runtime-versions.yaml)

### Qiskit Functions Catalog API
Premium / Flex-tier service for discovering and invoking abstracted Qiskit Functions — pre-packaged quantum-classical workflows callable through the `qiskit-ibm-catalog` Python client.

**Human URL:** [https://github.com/Qiskit/qiskit-ibm-catalog](https://github.com/Qiskit/qiskit-ibm-catalog)

### Qiskit Transpiler as a Service
Cloud-hosted, AI-augmented transpilation of OpenQASM 3 circuits down to IBM Quantum native gates and backend topology. Bundled with Flex and Premium plans.

## Common Properties

- [Portal — ibm.com/quantum](https://www.ibm.com/quantum)
- [Portal — IBM Quantum Platform](https://quantum.cloud.ibm.com/)
- [Documentation](https://quantum.cloud.ibm.com/docs)
- [Documentation — Qiskit Runtime REST](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI — live spec](https://quantum.cloud.ibm.com/api/openapi.json)
- [Pricing — plans overview](https://quantum.cloud.ibm.com/docs/en/guides/plans-overview)
- [Pricing — ibm.com/quantum/pricing](https://www.ibm.com/quantum/pricing)
- [GettingStarted](https://docs.quantum.ibm.com/start)
- [Sandbox — IBM Quantum Composer](https://quantum.cloud.ibm.com/composer)
- [Training — IBM Quantum Learning](https://quantum.cloud.ibm.com/learning)
- [Community — IBM Quantum Network](https://www.ibm.com/quantum/network)
- [Blog — IBM Quantum](https://www.ibm.com/quantum/blog)
- [Research — IBM Research Quantum](https://research.ibm.com/quantum-computing)
- [StatusPage — IBM Cloud Status](https://cloud.ibm.com/status)
- [SignUp — IBM Cloud](https://cloud.ibm.com/registration)
- [Authentication — IBM Cloud IAM](https://www.ibm.com/cloud/iam)
- [TrustCenter — ibm.com/trust](https://www.ibm.com/trust)
- [TermsOfService](https://www.ibm.com/legal)
- [PrivacyPolicy](https://www.ibm.com/privacy)
- [GitHub — Qiskit](https://github.com/Qiskit)
- [GitHub — Qiskit Community](https://github.com/qiskit-community)
- [SDK — Qiskit (Python + Rust + C)](https://github.com/Qiskit/qiskit)
- [SDK — qiskit-ibm-runtime](https://github.com/Qiskit/qiskit-ibm-runtime)
- [SDK — qiskit-ibm-runtime-c](https://github.com/Qiskit/qiskit-ibm-runtime-c)
- [SDK — qiskit-ibm-catalog](https://github.com/Qiskit/qiskit-ibm-catalog)
- [SDK — Qiskit Aer simulator](https://github.com/Qiskit/qiskit-aer)
- [Tool — Qiskit Serverless](https://github.com/Qiskit/qiskit-serverless)
- [Tool — Qiskit Fermions](https://github.com/Qiskit/qiskit-fermions)
- [Package — qiskit on PyPI](https://pypi.org/project/qiskit/)
- [Package — qiskit-ibm-runtime on PyPI](https://pypi.org/project/qiskit-ibm-runtime/)
- [Forum — Qiskit Slack](https://qisk.it/join-slack)
- [Forum — Stack Overflow](https://stackoverflow.com/questions/tagged/qiskit)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Qiskit Runtime Jobs API](openapi/ibm-quantum-runtime-jobs-openapi.yml)
- [Qiskit Runtime Backends API](openapi/ibm-quantum-runtime-backends-openapi.yml)
- [Qiskit Runtime Sessions API](openapi/ibm-quantum-runtime-sessions-openapi.yml)
- [Qiskit Runtime Instances API](openapi/ibm-quantum-runtime-instances-openapi.yml)
- [Qiskit Runtime Analytics API](openapi/ibm-quantum-runtime-analytics-openapi.yml)
- [Qiskit Runtime Versions API](openapi/ibm-quantum-runtime-versions-openapi.yml)

### JSON Schema

- [Job](json-schema/ibm-quantum-job-schema.json)
- [Backend](json-schema/ibm-quantum-backend-schema.json)
- [Session](json-schema/ibm-quantum-session-schema.json)

### JSON-LD

- [IBM Quantum Context](json-ld/ibm-quantum-context.jsonld)

### Capabilities (Naftiko)

- [Runtime Jobs](capabilities/runtime-jobs.yaml)
- [Runtime Backends](capabilities/runtime-backends.yaml)
- [Runtime Sessions](capabilities/runtime-sessions.yaml)
- [Runtime Instances](capabilities/runtime-instances.yaml)
- [Runtime Analytics](capabilities/runtime-analytics.yaml)
- [Runtime Versions](capabilities/runtime-versions.yaml)

### Examples

- [Create Sampler job](examples/ibm-quantum-create-sampler-job-example.json)
- [List backends](examples/ibm-quantum-list-backends-example.json)
- [Create session](examples/ibm-quantum-create-session-example.json)

### Commercial artifacts

- [Plans / Pricing](plans/ibm-quantum-plans-pricing.yml)
- [Rate Limits](rate-limits/ibm-quantum-rate-limits.yml)
- [FinOps Definition](finops/ibm-quantum-finops.yml)

### Governance

- [Spectral Ruleset](rules/ibm-quantum-rules.yml)
- [Vocabulary](vocabulary/ibm-quantum-vocabulary.yml)

## Authentication

Every Qiskit Runtime REST call requires three headers:

- `Authorization: Bearer <IBM Cloud IAM token>`
- `Service-CRN: crn:v1:bluemix:public:quantum-computing:<region>:a/<account>:<instance>::`
- `IBM-API-Version: 2026-03-15` (date-based contract pin)

Regional endpoints:

- Global — `https://quantum.cloud.ibm.com/api/v1`
- EU-DE — `https://eu-de.quantum.cloud.ibm.com/api/v1`

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
