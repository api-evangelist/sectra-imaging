# Sectra (sectra-imaging)

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

### Sectra Amplifier Marketplace Integration

The Amplifier Marketplace / Amplifier Services ecosystem through which AI and third-party applications integrate with the Sectra viewer. Two partnership tiers (Amplifier Partner, Amplifier Integrator). Partner-gated, available to Sectra PACS customers; no public self-service portal.

- **Human URL:** [Sectra Amplifier Marketplace](https://amplifiermarketplace.sectra.com/)

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
