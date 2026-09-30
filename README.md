<p align="center">
  <img src="assets/hero.svg?v=3" width="100%" alt="Dmitry Moiseenko — Software Engineer, Cloud & Application Security, Dallas, Texas. Production systems. Entirely owned."/>
</p>

<p align="center">
  <b>Dmitry Moiseenko</b> &nbsp;·&nbsp; Software Engineer — Cloud, Security, Full-Stack &nbsp;·&nbsp; Dallas, TX<br/>
  <sub>B.S. Software Engineering, The University of Texas at Dallas, May 2027 &nbsp;·&nbsp; AWS Certified Developer – Associate &nbsp;·&nbsp; Authorized to work in the U.S.</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/moiseenko-dmitry/"><img src="assets/btn-linkedin.svg?v=3" alt="LinkedIn: in/moiseenko-dmitry"/></a>&nbsp;&nbsp;
  <a href="mailto:moiseenko.dmitry@outlook.com"><img src="assets/btn-email.svg?v=3" alt="Email: moiseenko.dmitry@outlook.com"/></a>&nbsp;&nbsp;
  <a href="https://legacyvord.com"><img src="assets/btn-vord.svg?v=3" alt="Vörd — legacyvord.com"/></a>&nbsp;&nbsp;
  <a href="https://www.sixplanets.com"><img src="assets/btn-sixplanets.svg?v=3" alt="sixplanets.com"/></a>&nbsp;&nbsp;
  <a href="https://www.credly.com/badges/d7e15ba3-ab8c-4a73-96e6-a1a65662bb94"><img src="assets/btn-aws.svg?v=3" alt="AWS Certified Developer – Associate (verify on Credly)"/></a>
</p>

<br/>

<img src="assets/section-focus.svg?v=3" width="100%" alt="01 — What I do"/>

<br/>

I build web platforms for real businesses and keep them running: the Angular front end, the Python REST API behind it, the Terraform that stands it up, the tests and CI gates that guard it, and the alarms and runbooks for when something breaks. Two of those platforms are in production today. On both, I was the engineer of record from the first requirements call to the first incident.

<br/>

- **Serverless on AWS** &nbsp;—&nbsp; API Gateway + Lambda, DynamoDB single-table design, Step Functions, Cognito, KMS, CloudFront, SES. All of it as infrastructure as code (Terraform/OpenTofu), with CI/CD that authenticates via OIDC and rolls back by Lambda alias.

- **Security as a design input** &nbsp;—&nbsp; STRIDE and MITRE ATLAS threat models, KMS envelope encryption, zero-knowledge key handling, MFA and passkeys, tenant isolation. Scanners (bandit, checkov, gitleaks, pip-audit) fail the build instead of warning.

- **Client-facing delivery** &nbsp;—&nbsp; Written scope before building, iterative releases with demos, dated release notes, and audit reports a non-technical owner can act on. Comfortable both as a solo contractor and in Scrum teams.

<br/>

<img src="assets/section-systems.svg?v=3" width="100%" alt="02 — Systems I own"/>

<br/>

### Vörd &nbsp;·&nbsp; Co-founder & CTO

<img src="assets/strip-vord.svg?v=3" width="100%" alt="Co-founder & CTO · Zero-knowledge digital inheritance · legacyvord.com · May 2026 – present"/>

- Vaults are encrypted in the browser; the release key is **Shamir-split 2-of-3** across trusted contacts, so no server key can open a vault.
- **81-route REST API** on a framework-free Python Lambda: JWT sessions, passkeys/WebAuthn, TOTP 2FA, rate limiting, Stripe webhooks with signature verification.
- CI/CD on every push (tests → `tofu apply` → deploy → smoke test), alias-based rollback, CloudWatch alarms, cross-region replication with scripted restore drills.
- 214 API tests that run without AWS; UI in six languages with i18n parity tests; Playwright end-to-end with accessibility checks.

<br/>

### CorePractice &nbsp;·&nbsp; Software Engineer, Independent Contractor

<img src="assets/strip-corepractice.svg?v=3" width="100%" alt="Sole engineer, contractor · Back-office automation for dental practices · Core Practice Solutions Inc. · Jun 2026 – present"/>

- Multi-tenant platform that reconciles insurer payments against bank deposits for dental practices. Live in the client's AWS account (ca-central-1) **nine weeks** after the contract was signed.
- **87-endpoint REST API**: Pydantic validation, cursor pagination, DynamoDB conditional writes with a concurrency test suite; Step Functions-orchestrated Playwright connectors for bank and insurer portals.
- PIPEDA/HIPAA-scope security: Cognito with mandatory TOTP MFA, KMS envelope-encrypted credential vault, CloudTrail audit trail, STRIDE threat model, privacy impact assessment, incident-response runbook.
- Two security audits (Jul, Sep 2026) that found and fixed a cross-tenant takeover, a vault privilege bypass, and secret leakage into logs, each with a regression test.
- **800+ Pytest tests** at 80%+ coverage; bandit, pip-audit, checkov, gitleaks, and SHA-pinned GitHub Actions all block the build.

<br/>

### ClawGuardian &nbsp;·&nbsp; Hook 'Em Hacks 2026 — Security in an AI-First World + Best Use of AWS

<img src="assets/strip-clawguardian.svg?v=3" width="100%" alt="Hackathon, 2 track wins · Prompt-injection firewall for AI agents · Hook 'Em Hacks · Apr 2026"/>

- Prompt-injection firewall for AI agents with on-chain threat sharing. Led AWS architecture and frontend on a four-person team.
- Private VPC with PrivateLink endpoints, Cognito TOTP MFA, KMS signing and envelope encryption, Fargate, zero wildcard IAM, Bedrock with no internet egress.
- Threat model maps **25+ AI-agent threats to MITRE ATLAS** across five trust boundaries. &nbsp;[Devpost ↗](https://devpost.com/software/clawguardian)

<br/>

### Project Tusk &nbsp;·&nbsp; HackSMU VII 2026 — 1st place, Infrastructure Masons track

<img src="assets/strip-tusk.svg?v=3" width="100%" alt="Hackathon, 1st place · Bioacoustic research platform · HackSMU VII, Infrastructure Masons track · Apr 2026"/>

- Turns raw elephant field recordings into research-ready data for ElephantVoices.
- Led frontend and data visualization: an interactive 3D globe and waveform views in React, Next.js, TypeScript, Three.js, and wavesurfer.js. &nbsp;[Devpost ↗](https://devpost.com/software/echofield) &nbsp;·&nbsp; [GitHub ↗](https://github.com/ch1kim0n1/hacksmu26)

<br/>

### sixplanets &nbsp;·&nbsp; Founder

<img src="assets/strip-sixplanets.svg?v=3" width="100%" alt="Founder · Custom print studio, Frisco TX · sixplanets.com · Jan 2025 – present"/>

- Custom-printing business I founded, and the design system this page borrows from.
- Angular storefront on a serverless product/checkout API (Lambda, DynamoDB, Cognito) with Stripe payments; seven AWS services at roughly 60% lower cost than the managed hosting it replaced.

<br/>

<img src="assets/section-stack.svg?v=3" width="100%" alt="03 — Stack"/>

<br/>

<img src="assets/stack-build.svg?v=3" width="100%" alt="Build: Python, TypeScript, Angular, React, Next.js, Tailwind CSS, Java, C++, SQL, Bash, REST API design, Nx monorepo"/>

<br/>

<img src="assets/stack-run.svg?v=3" width="100%" alt="Run: AWS, Lambda, API Gateway, DynamoDB, Terraform / OpenTofu, Step Functions, Cognito, KMS, S3 + CloudFront, Route 53, SES, CloudWatch, Docker, GitHub Actions (OIDC), GCP, Linux"/>

<br/>

<img src="assets/stack-secure.svg?v=3" width="100%" alt="Secure: STRIDE threat modeling, MITRE ATLAS, KMS envelope encryption, zero-knowledge design, OWASP LLM Top 10, prompt-injection defense, MFA / TOTP / passkeys, least-privilege IAM, tenant isolation, incident response, PIPEDA / HIPAA, bandit, checkov, gitleaks, pip-audit, Dependabot"/>

<br/>

<img src="assets/stack-verify.svg?v=3" width="100%" alt="Verify: Pytest, Playwright, Jest, Selenium, Cypress, Postman, property-based and concurrency tests, mypy + ruff, axe accessibility"/>

<details>
<summary><sub>Plain-text version of the stack</sub></summary>
<br/>

**Build:** Python, TypeScript, JavaScript, Angular, React, Next.js, Tailwind CSS, Java, C++, SQL, Bash, REST API design, Nx monorepo
**Run:** AWS (Lambda, API Gateway, DynamoDB, Step Functions, Cognito, KMS, S3, CloudFront, Route 53, SES, CloudWatch), Terraform / OpenTofu, Docker, GitHub Actions CI/CD with OIDC, Google Cloud, Linux
**Secure:** STRIDE and MITRE ATLAS threat modeling, KMS envelope encryption, zero-knowledge design, OWASP LLM Top 10, prompt-injection defense, MFA (TOTP, passkeys / WebAuthn), least-privilege IAM, tenant isolation, incident response, PIPEDA / HIPAA controls, bandit, checkov, gitleaks, pip-audit, Dependabot
**Verify:** Pytest, Playwright, Jest, Selenium, Cypress, Postman, property-based and concurrency tests, mypy, ruff, axe accessibility testing

</details>

<br/>

<img src="assets/section-now.svg?v=3" width="100%" alt="04 — Right now"/>

<br/>

- Finishing a **B.S. in Software Engineering at The University of Texas at Dallas**, graduating May 2027.
- Operating CorePractice in production for a Canadian client, and shipping Vörd with a co-founder.
- **Open to Summer 2027 internships and 2027 new-grad roles** in cloud, security, or full-stack engineering. Dallas or remote. U.S. work authorization, no sponsorship needed.

<br/>

<p align="center">
  <img src="assets/footer.svg?v=3" width="100%" alt="Languages: Dutch, English, Russian, Ukrainian"/>
</p>

<p align="center">
  <sub>moiseenko.dmitry@outlook.com &nbsp;·&nbsp; <a href="https://www.linkedin.com/in/moiseenko-dmitry/">linkedin.com/in/moiseenko-dmitry</a> &nbsp;·&nbsp; Dallas, TX</sub>
</p>
