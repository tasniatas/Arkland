# Arkland
### Check Before You Pay.

**A land-document screening platform for Bangladesh.**

Arkland aims to make preliminary land-document screening more accessible by helping users identify inconsistencies across property records before proceeding with a transaction. The platform is designed around document analysis, automated discrepancy detection, and evidence-based human review.

**Live Demo:** [https://tasniatas.github.io/Arkland/](https://tasniatas.github.io/Arkland/)

**Repository:** [Arkland](https://github.com/tasniatas/Arkland)

---

## Overview

Land transactions require careful examination of ownership records and supporting documents. However, identifying inconsistencies across multiple documents can be difficult and time-consuming.

Arkland proposes a structured approach to this challenge by combining document processing, information comparison, and a review workflow in a single platform.

The long-term vision is to support more informed property decisions in Bangladesh through accessible technology and responsible verification practices.

## Core Capabilities

### Document Management
- Organize land-related documents within individual verification cases.
- Support multiple documents for cross-document comparison.
- Maintain references to original documents for review.

### Document Information Extraction
- Apply Optical Character Recognition (OCR) to extract relevant information from scanned documents.
- Preserve original extracted values alongside normalized information.
- Plan for Bangla-language document processing.

### Discrepancy Detection
- Compare available owner names and identifying information.
- Examine land identifiers, including khatian, dag/plot, mouza, and survey details.
- Flag conflicting land areas, dates, missing fields, and potential duplicate documents.
- Present detected discrepancies for further investigation.

### Verification and Review
- Track verification cases through defined processing stages.
- Provide reviewers with extracted information and supporting evidence.
- Record review decisions and explanations.
- Produce structured summaries of identified issues.

### Future Government Integration
Arkland is designed with the possibility of integrating authorized Bangladesh government land services in the future. Such integrations will depend on official approval, API availability, credentials, and applicable technical and legal requirements.

## How It Works

1. **Submit documents** — A user creates a verification case and provides available land-related documents.
2. **Extract information** — An OCR component identifies relevant text and fields.
3. **Compare records** — Automated rules compare available information across documents.
4. **Identify discrepancies** — Potential conflicts and missing information are flagged.
5. **Review evidence** — An authorized reviewer examines the findings.
6. **Generate a report** — The system summarizes detected issues and the recorded review outcome.

This workflow describes the intended system design; individual steps should be marked as implemented only after they have been developed and tested.

## Technology Stack

The planned architecture includes the following technologies. The final list should reflect the actual implementation.

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend API | Node.js, Express |
| Database | PostgreSQL |
| Document processing | OCR with Bangla-language support |
| Discrepancy detection | Rule-based comparison engine |
| File storage | Private object storage |
| Frontend deployment | GitHub Pages |

## Getting Started

### Prerequisites

For the current static website:

- A modern web browser
- Git
- Visual Studio Code (recommended)

### Run Locally

Clone the repository:

```bash
git clone https://github.com/tasniatas/Arkland.git
```

Navigate to the project directory:

```bash
cd Arkland
```

Open the folder in Visual Studio Code and launch `index.html` using Live Server, if supported by the project.

Alternatively, visit the [live website](https://tasniatas.github.io/Arkland/).

*Note: These instructions apply to a static HTML/CSS/JavaScript implementation. A future backend may require additional setup.*

## Development Roadmap

- [ ] Complete and refine the land-search and verification interface.
- [ ] Implement secure document upload and case management.
- [ ] Integrate OCR-based information extraction.
- [ ] Develop and test the discrepancy detection engine.
- [ ] Build evidence-based verification reports.
- [ ] Implement reviewer workflows and audit trails.
- [ ] Introduce appropriate security and privacy controls.
- [ ] Explore authorized government data integrations.
- [ ] Conduct pilot testing and obtain appropriate legal and security reviews.

## Security and Privacy

Land documents may contain sensitive personal and property information. A production deployment should incorporate:

- Authentication and role-based authorization.
- Secure document storage and restricted access.
- File validation and upload security.
- Encryption in transit and appropriate protection at rest.
- Auditable access and review histories.
- Secure management of credentials and API secrets.
- Appropriate retention and deletion policies.
- Compliance reviews for applicable Bangladesh data-protection and cybersecurity requirements.

## Limitations and Responsible Use

Arkland is intended to support preliminary document screening and due diligence. Automated results must be interpreted carefully.

- OCR may misinterpret handwritten text, stamps, low-quality scans, or Bangla characters.
- A discrepancy is a signal for investigation, not proof of fraud.
- Matching document fields does not establish legal ownership.
- A khatian or any single document should not be treated as conclusive proof of ownership.
- Official verification requires reliable, authorized sources where applicable.
- Government verification results must not be represented as real unless an authorized integration has been implemented and tested.

Arkland does not replace official verification or professional legal advice.

## Contributing

Feedback and contributions are welcome. Contributions should include clear documentation, appropriate testing, and instructions for reproducing changes.

Do not commit real land records, personal documents, credentials, or other sensitive information to the repository.

## License

This project is licensed under the **MIT License**. See the [`LICENSE`](LICENSE) file for details.

---

**Arkland — Check Before You Pay.**

*Building toward more accessible, transparent, and evidence-based land-document screening in Bangladesh.*
