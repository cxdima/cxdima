<p align="center">
  <img src="assets/hero.svg" width="100%" alt="Dmitry Moiseenko — Production systems. Entirely owned."/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/moiseenko-dmitry/"><img src="assets/btn-linkedin.svg" alt="LinkedIn"/></a>&nbsp;
  <a href="mailto:moiseenko.dmitry@outlook.com"><img src="assets/btn-email.svg" alt="Email"/></a>&nbsp;
  <a href="https://legacyvord.com"><img src="assets/btn-vord.svg" alt="Vörd"/></a>&nbsp;
  <a href="https://www.sixplanets.com"><img src="assets/btn-sixplanets.svg" alt="sixplanets"/></a>&nbsp;
  <a href="https://www.credly.com/badges/d7e15ba3-ab8c-4a73-96e6-a1a65662bb94"><img src="assets/btn-aws.svg" alt="AWS Certified Developer – Associate"/></a>
</p>

<br/>

<img src="assets/section-focus.svg" width="100%" alt="01 — What I do"/>

I build web platforms for real businesses and then keep them running. That means the Angular front end, the Python API behind it, the Terraform that stands it up, the tests and CI gates that guard it, and the alarms and runbooks for when something breaks at 2 a.m. Two of those platforms are in production today; on both I was the engineer of record from the first requirements call to the first incident.

- **Serverless on AWS** — API Gateway + Lambda, DynamoDB single-table design, Step Functions, Cognito, KMS, CloudFront, SES; all of it in Terraform/OpenTofu with CI that authenticates via OIDC and rolls back by Lambda alias
- **Security as a design input** — STRIDE and MITRE ATLAS threat models, KMS envelope encryption, zero-knowledge key handling, MFA and passkeys, tenant isolation, and scanners (bandit, checkov, gitleaks, pip-audit) that fail the build instead of warning
- **Client-facing delivery** — written scopes before building, iterative releases with demos, dated release notes, and audit reports a non-technical owner can act on

<br/>

<img src="assets/section-systems.svg" width="100%" alt="02 — Systems I own"/>

<img src="assets/project-vord.svg" width="100%" alt="Vörd — Co-founder & CTO"/>

- Vaults are encrypted in the browser; the release key is **Shamir-split 2-of-3** across trusted contacts, so no server key can open a vault
- **81-route REST API** on a framework-free Python Lambda: JWT sessions, passkeys/WebAuthn, TOTP 2FA, rate limiting, Stripe webhooks with signature verification, 214 tests that run without AWS
- CI/CD on every push: tests → `tofu apply` → deploy → smoke test; alias-based rollback, CloudWatch alarms, cross-region replication with scripted restore drills; UI in six languages with i18n parity tests

<img src="assets/project-corepractice.svg" width="100%" alt="CorePractice — sole engineer, contractor"/>

- Multi-tenant platform that reconciles insurer payments against bank deposits for dental practices; live in the client's AWS account (ca-central-1) nine weeks after the contract was signed
- **87-endpoint REST API** (Pydantic validation, cursor pagination, conditional writes with a concurrency test suite) plus Step Functions-orchestrated Playwright connectors for bank and insurer portals
- PIPEDA/HIPAA-scope posture: Cognito with mandatory TOTP MFA, KMS envelope-encrypted credential vault, CloudTrail, STRIDE threat model, privacy impact assessment, incident-response runbook; **800+ Pytest tests** at 80%+ coverage, all security scanners blocking

<img src="assets/project-clawguardian.svg" width="100%" alt="ClawGuardian — Hook 'Em Hacks, two track wins"/>

- Led AWS architecture and frontend: private VPC with PrivateLink endpoints, Cognito TOTP MFA, KMS signing and envelope encryption, Fargate, zero wildcard IAM, Bedrock with no internet egress
- Threat model maps **25+ AI-agent threats to MITRE ATLAS** across five trust boundaries; on-chain threat sharing between deployments — [Devpost](https://devpost.com/software/clawguardian)

<img src="assets/project-tusk.svg" width="100%" alt="Project Tusk — HackSMU VII, 1st place"/>

- Turns raw elephant field recordings into research-ready data for ElephantVoices; I led frontend and data visualization — an interactive 3D globe and waveform views in React, Next.js, Three.js, and wavesurfer.js — [Devpost](https://devpost.com/software/echofield) · [GitHub](https://github.com/ch1kim0n1/hacksmu26)

<img src="assets/project-sixplanets.svg" width="100%" alt="sixplanets — Founder"/>

- The business behind this page's design system. Angular storefront on a serverless product/checkout API with Stripe payments; seven AWS services at roughly 60% lower cost than the managed hosting it replaced

<br/>

<img src="assets/section-stack.svg" width="100%" alt="03 — Stack"/>

<table>
<tr>
<td align="right" width="90"><b>Build</b></td>
<td>
<img src="https://img.shields.io/badge/Python-1d4ed8?style=flat-square&logo=python&logoColor=fefdfb" alt="Python"/>
<img src="https://img.shields.io/badge/TypeScript-1d4ed8?style=flat-square&logo=typescript&logoColor=fefdfb" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Angular-1d4ed8?style=flat-square&logo=angular&logoColor=fefdfb" alt="Angular"/>
<img src="https://img.shields.io/badge/React-f3f0e9?style=flat-square&logo=react&logoColor=1d4ed8" alt="React"/>
<img src="https://img.shields.io/badge/Next.js-f3f0e9?style=flat-square&logo=nextdotjs&logoColor=111827" alt="Next.js"/>
<img src="https://img.shields.io/badge/Tailwind-f3f0e9?style=flat-square&logo=tailwindcss&logoColor=1d4ed8" alt="Tailwind"/>
<img src="https://img.shields.io/badge/Java-f3f0e9?style=flat-square&logo=openjdk&logoColor=111827" alt="Java"/>
<img src="https://img.shields.io/badge/C++-f3f0e9?style=flat-square&logo=cplusplus&logoColor=1d4ed8" alt="C++"/>
<img src="https://img.shields.io/badge/SQL-f3f0e9?style=flat-square&logo=postgresql&logoColor=111827" alt="SQL"/>
<img src="https://img.shields.io/badge/Bash-f3f0e9?style=flat-square&logo=gnubash&logoColor=111827" alt="Bash"/>
</td>
</tr>
<tr>
<td align="right"><b>Run</b></td>
<td>
<img src="https://img.shields.io/badge/AWS-1d4ed8?style=flat-square&logo=amazonwebservices&logoColor=fefdfb" alt="AWS"/>
<img src="https://img.shields.io/badge/Lambda-1d4ed8?style=flat-square&logo=awslambda&logoColor=fefdfb" alt="Lambda"/>
<img src="https://img.shields.io/badge/API_Gateway-1d4ed8?style=flat-square&logo=amazonapigateway&logoColor=fefdfb" alt="API Gateway"/>
<img src="https://img.shields.io/badge/DynamoDB-1d4ed8?style=flat-square&logo=amazondynamodb&logoColor=fefdfb" alt="DynamoDB"/>
<img src="https://img.shields.io/badge/Terraform_%2F_OpenTofu-1d4ed8?style=flat-square&logo=opentofu&logoColor=fefdfb" alt="Terraform / OpenTofu"/>
<img src="https://img.shields.io/badge/Step_Functions-f3f0e9?style=flat-square&logoColor=111827" alt="Step Functions"/>
<img src="https://img.shields.io/badge/Cognito-f3f0e9?style=flat-square&logoColor=111827" alt="Cognito"/>
<img src="https://img.shields.io/badge/S3_%2B_CloudFront-f3f0e9?style=flat-square&logoColor=111827" alt="S3 + CloudFront"/>
<img src="https://img.shields.io/badge/Route_53-f3f0e9?style=flat-square&logoColor=111827" alt="Route 53"/>
<img src="https://img.shields.io/badge/SES-f3f0e9?style=flat-square&logoColor=111827" alt="SES"/>
<img src="https://img.shields.io/badge/Docker-f3f0e9?style=flat-square&logo=docker&logoColor=1d4ed8" alt="Docker"/>
<img src="https://img.shields.io/badge/GitHub_Actions_(OIDC)-f3f0e9?style=flat-square&logo=githubactions&logoColor=1d4ed8" alt="GitHub Actions"/>
<img src="https://img.shields.io/badge/GCP-f3f0e9?style=flat-square&logo=googlecloud&logoColor=1d4ed8" alt="GCP"/>
<img src="https://img.shields.io/badge/Linux-f3f0e9?style=flat-square&logo=linux&logoColor=111827" alt="Linux"/>
</td>
</tr>
<tr>
<td align="right"><b>Secure</b></td>
<td>
<img src="https://img.shields.io/badge/STRIDE-1d4ed8?style=flat-square&logoColor=fefdfb" alt="STRIDE"/>
<img src="https://img.shields.io/badge/MITRE_ATLAS-1d4ed8?style=flat-square&logoColor=fefdfb" alt="MITRE ATLAS"/>
<img src="https://img.shields.io/badge/KMS_envelope_encryption-1d4ed8?style=flat-square&logoColor=fefdfb" alt="KMS envelope encryption"/>
<img src="https://img.shields.io/badge/Zero--knowledge_design-1d4ed8?style=flat-square&logoColor=fefdfb" alt="Zero-knowledge design"/>
<img src="https://img.shields.io/badge/OWASP_LLM_Top_10-f3f0e9?style=flat-square&logo=owasp&logoColor=111827" alt="OWASP LLM Top 10"/>
<img src="https://img.shields.io/badge/Prompt--injection_defense-f3f0e9?style=flat-square&logoColor=111827" alt="Prompt-injection defense"/>
<img src="https://img.shields.io/badge/MFA_%C2%B7_TOTP_%C2%B7_Passkeys-f3f0e9?style=flat-square&logoColor=111827" alt="MFA · TOTP · Passkeys"/>
<img src="https://img.shields.io/badge/Least--privilege_IAM-f3f0e9?style=flat-square&logoColor=111827" alt="Least-privilege IAM"/>
<img src="https://img.shields.io/badge/Tenant_isolation-f3f0e9?style=flat-square&logoColor=111827" alt="Tenant isolation"/>
<img src="https://img.shields.io/badge/Incident_response-f3f0e9?style=flat-square&logoColor=111827" alt="Incident response"/>
<img src="https://img.shields.io/badge/bandit-f3f0e9?style=flat-square&logoColor=111827" alt="bandit"/>
<img src="https://img.shields.io/badge/checkov-f3f0e9?style=flat-square&logoColor=111827" alt="checkov"/>
<img src="https://img.shields.io/badge/gitleaks-f3f0e9?style=flat-square&logoColor=111827" alt="gitleaks"/>
<img src="https://img.shields.io/badge/pip--audit-f3f0e9?style=flat-square&logoColor=111827" alt="pip-audit"/>
<img src="https://img.shields.io/badge/Dependabot-f3f0e9?style=flat-square&logo=dependabot&logoColor=1d4ed8" alt="Dependabot"/>
</td>
</tr>
<tr>
<td align="right"><b>Verify</b></td>
<td>
<img src="https://img.shields.io/badge/Pytest-1d4ed8?style=flat-square&logo=pytest&logoColor=fefdfb" alt="Pytest"/>
<img src="https://img.shields.io/badge/Playwright-1d4ed8?style=flat-square&logo=playwright&logoColor=fefdfb" alt="Playwright"/>
<img src="https://img.shields.io/badge/Jest-f3f0e9?style=flat-square&logo=jest&logoColor=111827" alt="Jest"/>
<img src="https://img.shields.io/badge/Selenium-f3f0e9?style=flat-square&logo=selenium&logoColor=111827" alt="Selenium"/>
<img src="https://img.shields.io/badge/Cypress-f3f0e9?style=flat-square&logo=cypress&logoColor=111827" alt="Cypress"/>
<img src="https://img.shields.io/badge/Postman-f3f0e9?style=flat-square&logo=postman&logoColor=111827" alt="Postman"/>
<img src="https://img.shields.io/badge/Property--based_%26_concurrency_tests-f3f0e9?style=flat-square&logoColor=111827" alt="Property-based and concurrency tests"/>
<img src="https://img.shields.io/badge/mypy_%2B_ruff-f3f0e9?style=flat-square&logoColor=111827" alt="mypy + ruff"/>
<img src="https://img.shields.io/badge/axe_accessibility-f3f0e9?style=flat-square&logoColor=111827" alt="axe accessibility"/>
</td>
</tr>
</table>

<br/>

<img src="assets/section-now.svg" width="100%" alt="04 — Right now"/>

- Finishing a B.S. in Software Engineering at UT Dallas (May 2027)
- Operating CorePractice in production for a Canadian client and shipping Vörd with a co-founder
- Open to Summer 2027 internships and new-grad roles in cloud, security, or full-stack engineering — Dallas or remote

<br/>

<p align="center">
  <img src="assets/footer.svg" width="100%" alt="Dutch · English · Russian · Ukrainian"/>
</p>
