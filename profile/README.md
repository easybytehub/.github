## EasyByte

A worker cooperative of software developers in Madrid. We build custom software, and we publish as open source the tools we need ourselves: working tools, not demos.

### EasyxLab

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/easybytehub/.github/main/profile/easyxlab-banner-dark.png">
  <img alt="EasyxLab — Measured, not assumed." src="https://raw.githubusercontent.com/easybytehub/.github/main/profile/easyxlab-banner.png">
</picture>

EasyxLab is our research lab: open studies and verification tools for the rules software has to follow. Every tool cites the rule behind each finding, and every study publishes its method, scripts and aggregated data.

**Tools**

- **[ai-mark-lint](https://github.com/easybytehub/ai-mark-lint)**: checks that AI-generated images, video and audio still carry the machine-readable marks required by the EU AI Act art. 50(2), California SB 942 and China's GB 45438 (C2PA, IPTC, AIGC).
- **[attest-lint](https://github.com/easybytehub/attest-lint)**: flags pinned PyPI dependencies whose PEP 740 attestations regressed or whose Trusted Publisher changed.
- **[crs-lint](https://github.com/easybytehub/crs-lint)**: lints OECD CRS XML offline against the official XSD and the Status Message business rules, citing the OECD error code.

**[Studies](https://github.com/easybytehub/easyxlab)**

- **S1, Verifactu conformance**: 10 of 35 files presented as valid records (28.6%) contain at least one error.
- **S2, spoofed AI crawlers**: 39.3% of 16,548 claims to be an AI or search crawler, on three small sites, were spoofed.
- **S3, AI provenance marks**: every pixel or container rewrite removed the embedded C2PA manifest (124/124).
- **S4, Wikidata drug labels**: about 0.9% of 34,207 multilingual labels are wrong, a lower bound.
- **S5, PyPI attestations**: the latest version is attested for 3,479 of 14,995 top PyPI projects (23.2%); 138 projects that once attested no longer do in the line `pip` installs.
- **S8, Spain's public-sector websites**: of 5,130 home pages served over HTTPS, 1,688 (32.9%) send HSTS; 4 of 5,570 entities serve a `security.txt` that is strictly valid under RFC 9116.

### Other tools

- **[verifactu-lint](https://github.com/easybytehub/verifactu-lint)**: checks in CI that the invoicing records your software generates comply with Spain's Verifactu rules (RD 1007/2023 and Orden HAC/1177/2024), citing the article. Read-only: it is not invoicing software.
- **[hullwork](https://github.com/easybytehub/hullwork)**: turns production errors into draft pull requests, with a person deciding every merge. Pre-alpha.
- **[docshield](https://github.com/easybytehub/docshield)**: document protection.

### How we work

Every release publishes its provenance with GitHub attestations signed with short-lived OIDC credentials: you can check which commit, workflow and runner produced each artifact. Nobody holds a private signing key.

We are a cooperative: the people who build the software decide what gets built and what gets released.

---

**[easybyte.es](https://easybyte.es)** · contact@easybyte.es
