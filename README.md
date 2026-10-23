# MSC Trustgate Public Key Infrastructure (PKI) Repository

Welcome to the official Public Key Infrastructure (PKI) Policy Repository of **MSC Trustgate.com Sdn Bhd** ("MSC Trustgate"). 

This repository contains the active, archived, and draft Certificate Policies (CP), Certification Practice Statements (CPS), and Time-Stamp Authority Practice Statements (TSPPS) governing MSC Trustgate's publicly trusted Certification Authorities (CAs).

## 📌 Document Structure & Navigation

In compliance with root store policies (Mozilla, Microsoft, Apple) and international standards (CA/B Forum, AATL, WebTrust), MSC Trustgate maintains dedicated CP/CPS documents for each distinct certificate use case.

| Use Case / Scope | Document Name | Active Document | Standard Alignment |
| :--- | :--- | :--- | :--- |
| **General** | General CP/CPS | [`/general/CP-CPS-General.md`](./general/CP-CPS-General.md) | RFC 3647 |
| **TLS Server** | Public Trust TLS Server CP/CPS | [`/tls-server/CP-CPS-TLS-Server.md`](./tls-server/CP-CPS-TLS-Server.md) | CA/B Forum TLS Baseline Requirements |
| **S/MIME** | Public Trust S/MIME CP/CPS | [`/smime/CP-CPS-SMIME.md`](./smime/CP-CPS-SMIME.md) | CA/B Forum S/MIME Baseline Requirements |
| **Document Signing** | Public Trust Document Signing CP/CPS | [`/document-signing/CP-CPS-DocSigning.md`](./document-signing/CP-CPS-DocSigning.md) | Adobe Approved Trust List (AATL) |
| **Time-Stamping** | Time-Stamp Authority Practice Statement (TSA) | [`/tspps/TSPPS.md`](./tspps/TSPPS.md) | ETSI EN 319 421, RFC 3161 |

## 📂 Repository Layout

repository/
├── README.md                      # Root index, OID directory, and contact information
├── CONTRIBUTING.md                # Internal policy review & publication workflow guidelines
│
├── general/                       # Master / Root General Policy
│   ├── CP-CPS-General.md          # Active version
│   └── archive/                   # Historical versions (e.g., CP-CPS-General-v1.0-20261021.md)
│
├── tls-server/                    # TLS Server Certificates
│   ├── CP-CPS-TLS-Server.md       # Active version
│   └── archive/                   # Historical versions
│
├── smime/                         # S/MIME Certificates
│   ├── CP-CPS-SMIME.md            # Active version
│   └── archive/                   # Historical versions
│
├── document-signing/              # Document Signing Certificates (AATL / CSC)
│   ├── CP-CPS-DocSigning.md       # Active version
│   └── archive/                   # Historical versions
│
├── tspps/                         # Time-Stamp Authority Practice Statements
│   ├── TSPPS.md                   # Active version
│   └── archive/                   # Historical versions
│
└── drafts/                        # Work-in-Progress (WIP) proposed policy revisions

## 📜 Versioning & Archive Management

To ensure full historical transparency for auditors and relying parties:

1. **Active Version:** The file located at the root of each domain directory (e.g., `/tls-server/CP-CPS-TLS-Server.md`) ALWAYS represents the currently effective policy.

2. **Archived Versions:** When a new version is released, the superseded version is moved to the corresponding `/archive/` folder and renamed using the pattern:`[Document-Type]-v[Major].[Minor]-[YYYYMMDD].md`*(Example: `/tls-server/archive/CP-CPS-TLS-Server-v1.0-20261021.md`)*

3. **Git Releases:** Official versions are tagged cryptographically using GitHub Releases (e.g., `release-tls-v1.1`).

## ✉️ Contact Information & Policy Authority

For inquiries regarding these policies, notice of potential non-compliance, or security concerns:

- **Policy Authority Email:** `pki-policy@msctrustgate.com`

- **Security & Incident Reporting:** `security@msctrustgate.com`

- **Official Website:** [Repository – Trustgate](https://www.msctrustgate.com/repository)
