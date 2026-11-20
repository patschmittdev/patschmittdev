Hi, I'm Pat.

Lately I've been building with AI agents and trying to figure out how much they should be allowed to do without someone checking. I also go looking for security bugs in open-source projects now and then.

**Security findings I reported**

- [GHSA-vwq2-c539-xpr6](https://github.com/agentrust-io/weight-custody-manifest/security/advisories/GHSA-vwq2-c539-xpr6) in weight-custody-manifest: the Azure confidential-VM verifiers checked every signature but never checked that the evidence came from Azure's paravisor, so any SNP or TDX guest that controls REPORT_DATA could satisfy them. Fixed in 0.32.0.
- [CVE-2026-119193](https://github.com/advisories/GHSA-9vw2-f4vp-x7gf) in PHPUnit: other local users could run code through a shared temporary directory used for PHPT code coverage. Fixed in 13.4.4.

**Projects**

- [Ziggurat](https://github.com/patschmittdev/Ziggurat): a reference implementation of a write gate for AI memory. Nothing becomes durable context until a trusted key signs it.
- [trust-surface-ratchet](https://github.com/patschmittdev/trust-surface-ratchet): pins short security lists, like permission modes, in tests so a change to one shows up in review.

**Contributions**

- [weight-custody-manifest](https://github.com/agentrust-io/weight-custody-manifest): fixes to the attestation and key-release verifiers
- [chamber](https://github.com/ianphil/chamber): chatroom orchestration, IPC validation, tool allowlists, permission prompts, some UI

Most of my code is still in private repos. I'm going through it and making public what's worth sharing.
