# ibm-quantum (ibm-quantum)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

IBM Quantum is IBM's quantum computing program — the operator of the IBM Quantum Platform (quantum.cloud.ibm.com), the publisher of the open-source Qiskit SDK, and the provider of the Qiskit Runtime REST API for submitting Sampler and Estimator primitive jobs to 100+ qubit Heron-generation QPUs and managed simulators. The platform combines an Apache-2.0 software stack (Qiskit, qiskit-ibm-runtime, qiskit-ibm-catalog, Qiskit Aer, Qiskit Serverless, Qiskit Functions) with a tiered access model (Open / Pay-As-You-Go / Flex / Premium / On-Premises) and is the longest-running commercial quantum computing API surface in the industry.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Qiskit Runtime Jobs API

Submit Qiskit Runtime primitive jobs (Sampler and Estimator) to IBM Quantum hardware over the REST API. Includes job creation, listing, retrieval, deletion, cancellation, results, logs, metrics, and tag management. Job submission is rate-limited to 5 requests per minute per IAM token.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Jobs

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](https://quantum.cloud.ibm.com/api/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/ibm-quantum-runtime-jobs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-jobs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-jobs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ibm-quantum-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/ibm-quantum-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/ibm-quantum-create-sampler-job-example.json)

### Qiskit Runtime Backends API

Discover available IBM Quantum backends (Heron, Eagle, and other QPUs plus simulators). Read backend configuration, calibrated properties, defaults, and live status for circuit transpilation and scheduling.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Backends

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](openapi/ibm-quantum-runtime-backends-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-backends.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-backends.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ibm-quantum-backend-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/ibm-quantum-list-backends-example.json)

### Qiskit Runtime Sessions API

Create, inspect, update, and close Qiskit Runtime sessions for grouping primitive jobs against a target backend with priority access. Supports dedicated and batch session modes with configurable max time and interactive timeouts.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Sessions

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](openapi/ibm-quantum-runtime-sessions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-sessions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-sessions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ibm-quantum-session-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/ibm-quantum-create-session-example.json)

### Qiskit Runtime Instances API

Inspect the current Qiskit Runtime instance, view instance limits and configuration, and read per-account configuration. Each Qiskit Runtime instance is identified by an IBM Cloud Service-CRN and governs plan, allocation, region, and access.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Instances
- Accounts

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](openapi/ibm-quantum-runtime-instances-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-instances.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-instances.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qiskit Runtime Analytics API

Usage analytics and active-workload reporting for a Qiskit Runtime instance. Powers FinOps and plan-utilization tracking against Open, Pay-As-You-Go, Flex, and Premium minute pools.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Analytics
- FinOps

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](openapi/ibm-quantum-runtime-analytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-analytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-analytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qiskit Runtime Versions API

Discover supported versions of the Qiskit Runtime REST API and negotiate the date-based IBM-API-Version header value.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Runtime
- Versions

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](openapi/ibm-quantum-runtime-versions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ibm-quantum-runtime-versions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-versions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qiskit Functions Catalog API

Premium / Flex-tier service for discovering and invoking abstracted Qiskit Functions — pre-packaged quantum-classical workflows (e.g. circuit cutting, error-mitigation pipelines) callable through the qiskit-ibm-catalog Python client. Accessible via the QiskitFunctionsCatalog object (catalog.list / load, function.run).

- **Human URL:** [https://github.com/Qiskit/qiskit-ibm-catalog](https://github.com/Qiskit/qiskit-ibm-catalog)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Functions

#### Properties

- [Documentation](https://github.com/Qiskit/qiskit-ibm-catalog)
- [Source Code](https://github.com/Qiskit/qiskit-ibm-catalog)
- [Postman Collection](collections/ibm-quantum-runtime-analytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-analytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-backends.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-backends.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-instances.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-instances.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-jobs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-jobs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-sessions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-sessions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-versions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-versions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qiskit Transpiler as a Service API

Cloud-hosted, AI-augmented transpilation of OpenQASM 3 circuits down to IBM Quantum native gates and backend topology. Bundled with Flex and Premium plans.

- **Human URL:** [https://quantum.cloud.ibm.com/docs/](https://quantum.cloud.ibm.com/docs/)

#### Tags

- IBM Quantum
- Quantum Computing
- Qiskit Transpiler

#### Properties

- [Documentation](https://quantum.cloud.ibm.com/docs/)
- [Postman Collection](collections/ibm-quantum-runtime-analytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-analytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-backends.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-backends.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-instances.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-instances.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-jobs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-jobs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-sessions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-sessions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ibm-quantum-runtime-versions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ibm-quantum-runtime-versions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.ibm.com/quantum)
- [Portal](https://quantum.cloud.ibm.com/)
- [Documentation](https://quantum.cloud.ibm.com/docs)
- [Documentation](https://quantum.cloud.ibm.com/docs/api/qiskit-runtime-rest)
- [OpenAPI](https://quantum.cloud.ibm.com/api/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Pricing](https://quantum.cloud.ibm.com/docs/en/guides/plans-overview)
- [Pricing](https://www.ibm.com/quantum/pricing)
- [Getting Started](https://docs.quantum.ibm.com/start)
- [Sandbox](https://quantum.cloud.ibm.com/composer)
- [Training](https://quantum.cloud.ibm.com/learning)
- [Community](https://www.ibm.com/quantum/network)
- [Blog](https://www.ibm.com/quantum/blog)
- [Research](https://research.ibm.com/quantum-computing)
- [Status Page](https://cloud.ibm.com/status)
- [Sign Up](https://cloud.ibm.com/registration)
- [Authentication](https://www.ibm.com/cloud/iam)
- [Terms of Service](https://www.ibm.com/legal)
- [Privacy Policy](https://www.ibm.com/privacy)
- [Trust Center](https://www.ibm.com/trust)
- [GitHub Organization](https://github.com/Qiskit)
- [GitHub Organization](https://github.com/qiskit-community)
- [SDK](https://github.com/Qiskit/qiskit)
- [SDK](https://github.com/Qiskit/qiskit-ibm-runtime)
- [SDK](https://github.com/Qiskit/qiskit-ibm-runtime-c)
- [SDK](https://github.com/Qiskit/qiskit-ibm-catalog)
- [SDK](https://github.com/Qiskit/qiskit-aer)
- [Tool](https://github.com/Qiskit/qiskit-serverless)
- [Tool](https://github.com/Qiskit/qiskit-fermions)
- [Code Examples](https://github.com/Qiskit/ecosystem)
- [Documentation](https://github.com/Qiskit/documentation)
- [Package](https://pypi.org/project/qiskit/)
- [Package](https://pypi.org/project/qiskit-ibm-runtime/)
- [Forum](https://qisk.it/join-slack)
- [Forum](https://stackoverflow.com/questions/tagged/qiskit)
- [Plans](plans/ibm-quantum-plans-pricing.yml)
- [Rate Limits](rate-limits/ibm-quantum-rate-limits.yml)
- [Fin Ops](finops/ibm-quantum-finops.yml)
- [Spectral Ruleset](rules/ibm-quantum-rules.yml)
- [Vocabulary](vocabulary/ibm-quantum-vocabulary.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
