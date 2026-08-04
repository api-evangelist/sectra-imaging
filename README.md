# Sectra (sectra-imaging)

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

Sectra is a Swedish medical technology company providing an enterprise imaging platform (PACS/VNA) for radiology, pathology, cardiology, orthopaedics, and other clinical -ologies. Rather than a single open developer API, Sectra delivers integration through established healthcare interoperability standards: **DICOM/DICOMweb** for imaging, **HL7** for orders and results messaging, **IHE XDS/XDS-I** for cross-enterprise document sharing, **FHIR/FHIRcast** for clinical context synchronization, and a **Web Content API** for embedding third-party content into the diagnostic viewer. AI and third-party applications integrate through the **Sectra Amplifier Marketplace / Amplifier Services** ecosystem.

**Access model:** Sectra's API and integration surface is **partner- and customer-gated**. Integrations are deployed per-site within a Sectra PACS installation; there is no public self-service developer portal, open API reference, or downloadable OpenAPI catalog. This entry is therefore an **honest stub** - the API entries are modeled from Sectra's publicly documented standards and interfaces (DICOMweb, HL7, XDS, FHIRcast, Web Content API), not scraped from an open, self-service API surface. Endpoint-level detail is marked `endpointsModeled: true` and not fabricated as Sectra-hosted public endpoints.

Notably, Sectra co-originated the **FHIRcast** standard (with Epic) and published the first open-source FHIRcast sandbox and reference implementation under the FHIRcast GitHub organization - the one genuinely open, public developer resource in the Sectra story.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sectra-imaging/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sectra-imaging/refs/heads/main/apis.yml)

## Tags

- Medical Imaging
- Enterprise Imaging
- PACS
- VNA
- Radiology
- Pathology
- Healthcare
- DICOM
- DICOMweb
- HL7
- FHIR
- FHIRcast
- IHE XDS
- Interoperability
- Partner API

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs (modeled from documented standards)

### Sectra DICOMweb API

Web-based access to imaging studies, series, and instances via the DICOM standard's RESTful services - QIDO-RS (query), WADO-RS (retrieve), STOW-RS (store). Base URL is deployed per customer site; endpoints are modeled from the DICOMweb standard, not a public Sectra-hosted surface.

- **Human URL:** [Enterprise imaging platform](https://medical.sectra.com/solutionarea/enterprise-imaging-platform/)

### Sectra HL7 Integration Interface

HL7 v2 messaging for orders, scheduling, worklist, and results/reports between Sectra PACS/RIS and surrounding EMR/RIS systems. Message-based (typically MLLP/HL7 v2), configured per deployment - not a public REST API.

- **Human URL:** [Enterprise imaging platform](https://medical.sectra.com/solutionarea/enterprise-imaging-platform/)

### Sectra FHIRcast Interface

Clinical context synchronization using the FHIRcast standard, which Sectra helped originate and for which it published the first open-source sandbox and reference implementation.

- **Human URL:** [Sectra at the forefront of FHIRcast development](https://medical.sectra.com/resources/sectra-forefront-development-fhircast/)
- **Source Code:** [github.com/fhircast](https://github.com/fhircast)

### Sectra Web Content API

Embeds third-party web content, results, and applications into the Sectra diagnostic viewer in patient/study context, and launches Sectra in context from other systems. A customer/partner-configured integration point.

- **Human URL:** [Enterprise imaging platform](https://medical.sectra.com/solutionarea/enterprise-imaging-platform/)

### Sectra IHE XDS Interface

IHE Cross-Enterprise Document Sharing (XDS/XDS-I) for registering, querying, and retrieving imaging documents and manifests across enterprise boundaries. Profile-based interoperability, configured per deployment.

- **Human URL:** [Enterprise imaging platform](https://medical.sectra.com/solutionarea/enterprise-imaging-platform/)


## Common Properties

- [LinkedIn](https://www.linkedin.com/company/sectra)
- [Website](https://sectra.com/)
- [Sectra Medical](https://medical.sectra.com/)
- [Documentation - Enterprise imaging platform](https://medical.sectra.com/solutionarea/enterprise-imaging-platform/)
- [Amplifier Marketplace](https://amplifiermarketplace.sectra.com/)
- [FHIRcast Source Code](https://github.com/fhircast)

## Pricing

Not publicly listed. Sectra sells enterprise imaging to healthcare organizations via direct sales; Amplifier Marketplace / Amplifier Services access is arranged through Sectra sales and partnership channels. Contact Sectra for pricing.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
