<p align="center">
  <img src="assets/hero.svg" width="100%" alt="Dmitry Moiseenko — Software Engineer, Cloud & Application Security, Dallas, Texas. Production systems. Entirely owned."/>
</p>

<p align="center">
  <b>Dmitry Moiseenko</b> &nbsp;·&nbsp; Software Engineer — Cloud, Security, Full-Stack &nbsp;·&nbsp; Dallas, TX<br/>
  <sub>B.S. Software Engineering, The University of Texas at Dallas, May 2027 &nbsp;·&nbsp; AWS Certified Developer – Associate &nbsp;·&nbsp; Authorized to work in the U.S.</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/moiseenko-dmitry/"><img src="assets/btn-linkedin.svg" alt="LinkedIn: in/moiseenko-dmitry"/></a>&nbsp;&nbsp;
  <a href="mailto:moiseenko.dmitry@outlook.com"><img src="assets/btn-email.svg" alt="Email: moiseenko.dmitry@outlook.com"/></a>&nbsp;&nbsp;
  <a href="https://legacyvord.com"><img src="assets/btn-vord.svg" alt="Vörd — legacyvord.com"/></a>&nbsp;&nbsp;
  <a href="https://www.sixplanets.com"><img src="assets/btn-sixplanets.svg" alt="sixplanets.com"/></a>&nbsp;&nbsp;
  <a href="https://www.credly.com/badges/d7e15ba3-ab8c-4a73-96e6-a1a65662bb94"><img src="assets/btn-aws.svg" alt="AWS Certified Developer – Associate (verify on Credly)"/></a>
</p>

<br/>

<img src="assets/section-focus.svg" width="100%" alt="01 — What I do"/>

<br/>

I build web platforms for real businesses and keep them running: the Angular front end, the Python REST API behind it, the Terraform that stands it up, the tests and CI gates that guard it, and the alarms and runbooks for when something breaks. Two of those platforms are in production today. On both, I was the engineer of record from the first requirements call to the first incident.

<br/>

- **Serverless on AWS** &nbsp;—&nbsp; API Gateway + Lambda, DynamoDB single-table design, Step Functions, Cognito, KMS, CloudFront, SES. All of it as infrastructure as code (Terraform/OpenTofu), with CI/CD that authenticates via OIDC and rolls back by Lambda alias.

- **Security as a design input** &nbsp;—&nbsp; STRIDE and MITRE ATLAS threat models, KMS envelope encryption, zero-knowledge key handling, MFA and passkeys, tenant isolation. Scanners (bandit, checkov, gitleaks, pip-audit) fail the build instead of warning.

- **Client-facing delivery** &nbsp;—&nbsp; Written scope before building, iterative releases with demos, dated release notes, and audit reports a non-technical owner can act on. Comfortable both as a solo contractor and in Scrum teams.

<br/>

<img src="assets/section-systems.svg" width="100%" alt="02 — Systems I own"/>

<br/>

### Vörd &nbsp;·&nbsp; Co-founder & CTO

<img src="assets/project-vord.svg" width="100%" alt="Co-founder & CTO · Zero-knowledge digital inheritance · legacyvord.com · May 2026 – present"/>

- Vaults are encrypted in the browser; the release key is **Shamir-split 2-of-3** across trusted contacts, so no server key can open a vault.
- **81-route REST API** on a framework-free Python Lambda: JWT sessions, passkeys/WebAuthn, TOTP 2FA, rate limiting, Stripe webhooks with signature verification.
- CI/CD on every push (tests → `tofu apply` → deploy → smoke test), alias-based rollback, CloudWatch alarms, cross-region replication with scripted restore drills.
- 214 API tests that run without AWS; UI in six languages with i18n parity tests; Playwright end-to-end with accessibility checks.

<br/>

### CorePractice &nbsp;·&nbsp; Software Engineer, Independent Contractor

<img src="assets/project-corepractice.svg" width="100%" alt="Sole engineer, contractor · Back-office automation for dental practices · Core Practice Solutions Inc. · Jun 2026 – present"/>

- Multi-tenant platform that reconciles insurer payments against bank deposits for dental practices. Live in the client's AWS account (ca-central-1) **nine weeks** after the contract was signed.
- **87-endpoint REST API**: Pydantic validation, cursor pagination, DynamoDB conditional writes with a concurrency test suite; Step Functions-orchestrated Playwright connectors for bank and insurer portals.
- PIPEDA/HIPAA-scope security: Cognito with mandatory TOTP MFA, KMS envelope-encrypted credential vault, CloudTrail audit trail, STRIDE threat model, privacy impact assessment, incident-response runbook.
- Two security audits (Jul, Sep 2026) that found and fixed a cross-tenant takeover, a vault privilege bypass, and secret leakage into logs, each with a regression test.
- **800+ Pytest tests** at 80%+ coverage; bandit, pip-audit, checkov, gitleaks, and SHA-pinned GitHub Actions all block the build.

<br/>

### ClawGuardian &nbsp;·&nbsp; Hook 'Em Hacks 2026 — Security in an AI-First World + Best Use of AWS

<img src="assets/project-clawguardian.svg" width="100%" alt="Hackathon, 2 track wins · Prompt-injection firewall for AI agents · Hook 'Em Hacks · Apr 2026"/>

- Prompt-injection firewall for AI agents with on-chain threat sharing. Led AWS architecture and frontend on a four-person team.
- Private VPC with PrivateLink endpoints, Cognito TOTP MFA, KMS signing and envelope encryption, Fargate, zero wildcard IAM, Bedrock with no internet egress.
- Threat model maps **25+ AI-agent threats to MITRE ATLAS** across five trust boundaries. &nbsp;[Devpost ↗](https://devpost.com/software/clawguardian)

<br/>

### Project Tusk &nbsp;·&nbsp; HackSMU VII 2026 — 1st place, Infrastructure Masons track

<img src="assets/project-tusk.svg" width="100%" alt="Hackathon, 1st place · Bioacoustic research platform · HackSMU VII, Infrastructure Masons track · Apr 2026"/>

- Turns raw elephant field recordings into research-ready data for ElephantVoices.
- Led frontend and data visualization: an interactive 3D globe and waveform views in React, Next.js, TypeScript, Three.js, and wavesurfer.js. &nbsp;[Devpost ↗](https://devpost.com/software/echofield) &nbsp;·&nbsp; [GitHub ↗](https://github.com/ch1kim0n1/hacksmu26)

<br/>

### sixplanets &nbsp;·&nbsp; Founder

<img src="assets/project-sixplanets.svg" width="100%" alt="Founder · Custom print studio, Frisco TX · sixplanets.com · Jan 2025 – present"/>

- Custom-printing business I founded, and the design system this page borrows from.
- Angular storefront on a serverless product/checkout API (Lambda, DynamoDB, Cognito) with Stripe payments; seven AWS services at roughly 60% lower cost than the managed hosting it replaced.

<br/>

<img src="assets/section-stack.svg" width="100%" alt="03 — Stack"/>

<br/>

**Build**

<img src="https://img.shields.io/badge/Python-1d4ed8?style=flat-square&logo=python&logoColor=fefdfb" alt="Python"/>&nbsp;
<img src="https://img.shields.io/badge/TypeScript-1d4ed8?style=flat-square&logo=typescript&logoColor=fefdfb" alt="TypeScript"/>&nbsp;
<img src="https://img.shields.io/badge/Angular-1d4ed8?style=flat-square&logo=angular&logoColor=fefdfb" alt="Angular"/>&nbsp;
<img src="https://img.shields.io/badge/React-f3f0e9?style=flat-square&logo=react&logoColor=1d4ed8" alt="React"/>&nbsp;
<img src="https://img.shields.io/badge/Next.js-f3f0e9?style=flat-square&logo=nextdotjs&logoColor=111827" alt="Next.js"/>&nbsp;
<img src="https://img.shields.io/badge/Tailwind_CSS-f3f0e9?style=flat-square&logo=tailwindcss&logoColor=1d4ed8" alt="Tailwind CSS"/>&nbsp;
<img src="https://img.shields.io/badge/Java-f3f0e9?style=flat-square&logo=openjdk&logoColor=111827" alt="Java"/>&nbsp;
<img src="https://img.shields.io/badge/C++-f3f0e9?style=flat-square&logo=cplusplus&logoColor=1d4ed8" alt="C++"/>&nbsp;
<img src="https://img.shields.io/badge/SQL-f3f0e9?style=flat-square&logo=postgresql&logoColor=111827" alt="SQL"/>&nbsp;
<img src="https://img.shields.io/badge/Bash-f3f0e9?style=flat-square&logo=gnubash&logoColor=111827" alt="Bash"/>&nbsp;
<img src="https://img.shields.io/badge/REST_API_design-f3f0e9?style=flat-square&logoColor=111827" alt="REST API design"/>

<br/>

**Run**

<img src="https://img.shields.io/badge/AWS-1d4ed8?style=flat-square&logo=amazonwebservices&logoColor=fefdfb" alt="AWS"/>&nbsp;
<img src="https://img.shields.io/badge/Lambda-1d4ed8?style=flat-square&logo=awslambda&logoColor=fefdfb" alt="AWS Lambda"/>&nbsp;
<img src="https://img.shields.io/badge/API_Gateway-1d4ed8?style=flat-square&logo=amazonapigateway&logoColor=fefdfb" alt="API Gateway"/>&nbsp;
<img src="https://img.shields.io/badge/DynamoDB-1d4ed8?style=flat-square&logo=amazondynamodb&logoColor=fefdfb" alt="DynamoDB"/>&nbsp;
<img src="https://img.shields.io/badge/Terraform_%2F_OpenTofu-1d4ed8?style=flat-square&logo=opentofu&logoColor=fefdfb" alt="Terraform / OpenTofu"/>&nbsp;
<img src="https://img.shields.io/badge/Step_Functions-f3f0e9?style=flat-square&logoColor=111827" alt="Step Functions"/>&nbsp;
<img src="https://img.shields.io/badge/Cognito-f3f0e9?style=flat-square&logoColor=111827" alt="Cognito"/>&nbsp;
<img src="https://img.shields.io/badge/KMS-f3f0e9?style=flat-square&logoColor=111827" alt="KMS"/>&nbsp;
<img src="https://img.shields.io/badge/S3_%2B_CloudFront-f3f0e9?style=flat-square&logoColor=111827" alt="S3 + CloudFront"/>&nbsp;
<img src="https://img.shields.io/badge/Route_53-f3f0e9?style=flat-square&logoColor=111827" alt="Route 53"/>&nbsp;
<img src="https://img.shields.io/badge/SES-f3f0e9?style=flat-square&logoColor=111827" alt="SES"/>&nbsp;
<img src="https://img.shields.io/badge/CloudWatch-f3f0e9?style=flat-square&logoColor=111827" alt="CloudWatch"/>&nbsp;
<img src="https://img.shields.io/badge/Docker-f3f0e9?style=flat-square&logo=docker&logoColor=1d4ed8" alt="Docker"/>&nbsp;
<img src="https://img.shields.io/badge/GitHub_Actions_(OIDC)-f3f0e9?style=flat-square&logo=githubactions&logoColor=1d4ed8" alt="GitHub Actions CI/CD with OIDC"/>&nbsp;
<img src="https://img.shields.io/badge/GCP-f3f0e9?style=flat-square&logo=googlecloud&logoColor=1d4ed8" alt="Google Cloud"/>&nbsp;
<img src="https://img.shields.io/badge/Linux-f3f0e9?style=flat-square&logo=linux&logoColor=111827" alt="Linux"/>

<br/>

**Secure**

<img src="https://img.shields.io/badge/STRIDE_threat_modeling-1d4ed8?style=flat-square&logoColor=fefdfb" alt="STRIDE threat modeling"/>&nbsp;
<img src="https://img.shields.io/badge/MITRE_ATLAS-1d4ed8?style=flat-square&logoColor=fefdfb" alt="MITRE ATLAS"/>&nbsp;
<img src="https://img.shields.io/badge/KMS_envelope_encryption-1d4ed8?style=flat-square&logoColor=fefdfb" alt="KMS envelope encryption"/>&nbsp;
<img src="https://img.shields.io/badge/Zero--knowledge_design-1d4ed8?style=flat-square&logoColor=fefdfb" alt="Zero-knowledge design"/>&nbsp;
<img src="https://img.shields.io/badge/OWASP_LLM_Top_10-f3f0e9?style=flat-square&logo=owasp&logoColor=111827" alt="OWASP LLM Top 10"/>&nbsp;
<img src="https://img.shields.io/badge/Prompt--injection_defense-f3f0e9?style=flat-square&logoColor=111827" alt="Prompt-injection defense"/>&nbsp;
<img src="https://img.shields.io/badge/MFA_%C2%B7_TOTP_%C2%B7_Passkeys-f3f0e9?style=flat-square&logoColor=111827" alt="MFA, TOTP, Passkeys / WebAuthn"/>&nbsp;
<img src="https://img.shields.io/badge/Least--privilege_IAM-f3f0e9?style=flat-square&logoColor=111827" alt="Least-privilege IAM"/>&nbsp;
<img src="https://img.shields.io/badge/Tenant_isolation-f3f0e9?style=flat-square&logoColor=111827" alt="Tenant isolation"/>&nbsp;
<img src="https://img.shields.io/badge/Incident_response-f3f0e9?style=flat-square&logoColor=111827" alt="Incident response"/>&nbsp;
<img src="https://img.shields.io/badge/PIPEDA_%2F_HIPAA-f3f0e9?style=flat-square&logoColor=111827" alt="PIPEDA / HIPAA controls"/>&nbsp;
<img src="https://img.shields.io/badge/bandit-f3f0e9?style=flat-square&logoColor=111827" alt="bandit"/>&nbsp;
<img src="https://img.shields.io/badge/checkov-f3f0e9?style=flat-square&logoColor=111827" alt="checkov"/>&nbsp;
<img src="https://img.shields.io/badge/gitleaks-f3f0e9?style=flat-square&logoColor=111827" alt="gitleaks"/>&nbsp;
<img src="https://img.shields.io/badge/pip--audit-f3f0e9?style=flat-square&logoColor=111827" alt="pip-audit"/>&nbsp;
<img src="https://img.shields.io/badge/Dependabot-f3f0e9?style=flat-square&logo=dependabot&logoColor=1d4ed8" alt="Dependabot"/>

<br/>

**Verify**

<img src="https://img.shields.io/badge/Pytest-1d4ed8?style=flat-square&logo=pytest&logoColor=fefdfb" alt="Pytest"/>&nbsp;
<img src="https://img.shields.io/badge/Playwright-1d4ed8?style=flat-square&logo=playwright&logoColor=fefdfb" alt="Playwright"/>&nbsp;
<img src="https://img.shields.io/badge/Jest-f3f0e9?style=flat-square&logo=jest&logoColor=111827" alt="Jest"/>&nbsp;
<img src="https://img.shields.io/badge/Selenium-f3f0e9?style=flat-square&logo=selenium&logoColor=111827" alt="Selenium"/>&nbsp;
<img src="https://img.shields.io/badge/Cypress-f3f0e9?style=flat-square&logo=cypress&logoColor=111827" alt="Cypress"/>&nbsp;
<img src="https://img.shields.io/badge/Postman-f3f0e9?style=flat-square&logo=postman&logoColor=111827" alt="Postman"/>&nbsp;
<img src="https://img.shields.io/badge/Property--based_%26_concurrency_tests-f3f0e9?style=flat-square&logoColor=111827" alt="Property-based and concurrency tests"/>&nbsp;
<img src="https://img.shields.io/badge/mypy_%2B_ruff-f3f0e9?style=flat-square&logoColor=111827" alt="mypy + ruff"/>&nbsp;
<img src="https://img.shields.io/badge/axe_accessibility-f3f0e9?style=flat-square&logoColor=111827" alt="axe accessibility testing"/>

<br/>

<img src="assets/section-now.svg" width="100%" alt="04 — Right now"/>

<br/>

- Finishing a **B.S. in Software Engineering at The University of Texas at Dallas**, graduating May 2027.
- Operating CorePractice in production for a Canadian client, and shipping Vörd with a co-founder.
- **Open to Summer 2027 internships and 2027 new-grad roles** in cloud, security, or full-stack engineering. Dallas or remote. U.S. work authorization, no sponsorship needed.

<br/>

<p align="center">
  <img src="assets/footer.svg" width="100%" alt="Languages: Dutch, English, Russian, Ukrainian"/>
</p>

<p align="center">
  <sub>moiseenko.dmitry@outlook.com &nbsp;·&nbsp; <a href="https://www.linkedin.com/in/moiseenko-dmitry/">linkedin.com/in/moiseenko-dmitry</a> &nbsp;·&nbsp; Dallas, TX</sub>
</p>
