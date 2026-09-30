<div align="center">

<img
  width="100%"
  src="https://capsule-render.vercel.app/api?type=rect&color=0:0b0f14,50:0f1b2d,100:12263a&height=230&section=header&text=DMITRY%20MOISEENKO&fontSize=42&fontColor=F2F5F7&fontAlignY=38&desc=FULL-STACK%20%2F%2F%20CLOUD%20INFRASTRUCTURE%20%2F%2F%20APPLICATION%20SECURITY&descAlignY=59&descSize=15&descColor=8FB3C9"
  alt="Dmitry Moiseenko"
/>

<a href="https://readme-typing-svg.demolab.com">
  <img
    src="https://readme-typing-svg.demolab.com?font=IBM+Plex+Mono&weight=500&size=14&duration=2600&pause=900&color=8FB3C9&center=true&vCenter=true&repeat=true&width=800&height=45&lines=%5BSHIP%5D+Production+platforms+on+AWS%2C+end+to+end;%5BSECURE%5D+Threat+models%2C+encryption%2C+CI+gates+that+fail+the+build;%5BOWN%5D+From+client+requirements+to+alarms+and+restore+drills"
    alt="Engineering focus"
  />
</a>

<br/>

<a href="https://www.linkedin.com/in/moiseenko-dmitry/">
  <img src="https://img.shields.io/badge/LINKEDIN-0B1116?style=for-the-badge&logo=linkedin&logoColor=9FC2D6" alt="LinkedIn"/>
</a>
<a href="mailto:moiseenko.dmitry@outlook.com">
  <img src="https://img.shields.io/badge/EMAIL-0B1116?style=for-the-badge&logo=maildotru&logoColor=9FC2D6" alt="Email"/>
</a>
<a href="https://legacyvord.com">
  <img src="https://img.shields.io/badge/V%C3%96RD-0B1116?style=for-the-badge&logo=googlechrome&logoColor=9FC2D6" alt="Vörd"/>
</a>
<a href="https://www.credly.com/badges/d7e15ba3-ab8c-4a73-96e6-a1a65662bb94">
  <img src="https://img.shields.io/badge/AWS_CERTIFIED_DEVELOPER-0B1116?style=for-the-badge&logo=amazonwebservices&logoColor=9FC2D6" alt="AWS Certified Developer – Associate"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/STATUS-SHIPPING_TO_PRODUCTION-14202E?style=flat-square&labelColor=080C0F&color=14202E" alt="Status"/>
<img src="https://img.shields.io/badge/FOCUS-CLOUD_%2B_SECURITY-14202E?style=flat-square&labelColor=080C0F&color=14202E" alt="Focus"/>
<img src="https://img.shields.io/badge/LOCATION-DALLAS_TX-14202E?style=flat-square&labelColor=080C0F&color=14202E" alt="Location"/>
<img src="https://img.shields.io/badge/UTD-B.S._SOFTWARE_ENGINEERING_'27-14202E?style=flat-square&labelColor=080C0F&color=14202E" alt="UT Dallas"/>
<img src="https://komarev.com/ghpvc/?username=cxdima&style=flat-square&color=14202E&label=PROFILE+VIEWS" alt="Profile views"/>

</div>

---

## Focus
- Serverless platforms on AWS: Python + API Gateway/Lambda, DynamoDB single-table design, Terraform/OpenTofu, CI/CD with OIDC and rollback
- Application security: STRIDE and MITRE ATLAS threat modeling, KMS envelope encryption, MFA/passkeys, tenant isolation, blocking security gates in CI
- Client-facing delivery: sole engineer for real businesses, from written requirements to production ownership

---

## Flagship Systems

### Vörd — [legacyvord.com](https://legacyvord.com)
Zero-knowledge digital-inheritance platform. Co-founder & CTO.
- Vaults are encrypted in the browser; the release key is Shamir-split 2-of-3 across trusted contacts, so no server key can open a vault
- 81-route REST API on a framework-free Python Lambda: JWT sessions, passkeys/WebAuthn, TOTP 2FA, rate limiting, Stripe webhooks with signature verification
- CI/CD via GitHub Actions + OIDC: tests → `tofu apply` → deploy → smoke test; Lambda alias rollback, CloudWatch alarms, cross-region replication with restore drills

### CorePractice — Core Practice Solutions Inc. *(private)*
Multi-tenant back-office automation for dental practices, built as sole engineer and independent contractor. Live in the client's AWS account (ca-central-1).
- 87-endpoint REST API (API Gateway + Python Lambda, Pydantic, cursor pagination, conditional writes) and Step Functions-orchestrated Playwright connectors for bank and insurer portals
- Security posture for PIPEDA/HIPAA-scope data: Cognito with mandatory TOTP MFA, KMS envelope-encrypted credential vault, CloudTrail, STRIDE threat model, PIA, incident-response runbook
- 800+ Pytest tests at 80%+ coverage; bandit, pip-audit, checkov, gitleaks, and SHA-pinned actions all fail the build

### ClawGuardian — [Devpost](https://devpost.com/software/clawguardian)
Prompt-injection firewall for AI agents with on-chain threat sharing. **Hook 'Em Hacks 2026: Security in an AI-First World + Best Use of AWS.**
- Led AWS architecture and frontend: private VPC with PrivateLink, Cognito TOTP MFA, KMS signing, Fargate, zero wildcard IAM, Bedrock with no internet egress
- Threat model maps 25+ AI-agent threats to MITRE ATLAS across five trust boundaries

### Project Tusk — [Devpost](https://devpost.com/software/echofield) · [GitHub](https://github.com/ch1kim0n1/hacksmu26)
Bioacoustic research platform for ElephantVoices. **HackSMU VII 2026: 1st place, Infrastructure Masons track.**
- Led frontend and data visualization: interactive 3D globe and waveform views (React, Next.js, Three.js, wavesurfer.js)

### sixplanets — [sixplanets.com](https://www.sixplanets.com)
Custom-printing e-commerce business I founded. Angular storefront on a serverless product/checkout API with Stripe payments; 7 AWS services at ~60% lower cost than traditional hosting.

---

## GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=cxdima&show_icons=true&theme=nord&hide_border=true&bg_color=0b0f14&title_color=8FB3C9&icon_color=8FB3C9&text_color=c9d1d9" alt="GitHub stats" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=cxdima&layout=compact&theme=nord&hide_border=true&bg_color=0b0f14&title_color=8FB3C9&text_color=c9d1d9" alt="Top languages" height="165"/>
</p>

---

## Skills

### Languages

<p>
  <img src="https://skillicons.dev/icons?i=python,ts,js,java,cpp,bash,html,css&perline=16" alt="Languages"/>
</p>

<p>
  <img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge" />
  <img src="https://img.shields.io/badge/HCL_(Terraform)-623CE4?style=for-the-badge" />
</p>

### Frontend

<p>
  <img src="https://skillicons.dev/icons?i=angular,react,nextjs,tailwind,threejs,vite&perline=14" alt="Frontend"/>
</p>

<p>
  <img src="https://img.shields.io/badge/Nx_Monorepo-143055?style=for-the-badge&logo=nx&logoColor=white" />
  <img src="https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=black" />
  <img src="https://img.shields.io/badge/Leaflet-199900?style=for-the-badge&logo=leaflet&logoColor=white" />
  <img src="https://img.shields.io/badge/i18n_(6_locales)-455A64?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Accessibility_(axe)-1565C0?style=for-the-badge" />
</p>

### Backend / APIs

<p>
  <img src="https://skillicons.dev/icons?i=python,dynamodb,postman&perline=14" alt="Backend"/>
</p>

<p>
  <img src="https://img.shields.io/badge/REST_API_Design-005571?style=for-the-badge" />
  <img src="https://img.shields.io/badge/API_Gateway-FF4F8B?style=for-the-badge&logo=amazonapigateway&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white" />
  <img src="https://img.shields.io/badge/Lambda_Powertools-232F3E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
  <img src="https://img.shields.io/badge/Webhooks_(Stripe%2C_Telegram)-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />
  <img src="https://img.shields.io/badge/Step_Functions-E7157B?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Single--Table_DynamoDB-4053D6?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Rate_Limiting-B00020?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Multi--Tenant_Architecture-00695C?style=for-the-badge" />
</p>

### Cloud / DevOps / Infrastructure

<p>
  <img src="https://skillicons.dev/icons?i=aws,gcp,terraform,docker,githubactions,linux,cloudflare&perline=14" alt="Cloud"/>
</p>

<p>
  <img src="https://img.shields.io/badge/OpenTofu-FFDA18?style=for-the-badge&logo=opentofu&logoColor=black" />
  <img src="https://img.shields.io/badge/Infrastructure_as_Code-623CE4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/OIDC_CI%2FCD_(no_stored_keys)-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/CloudFront_%2B_S3-8C4FFF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Route_53_%2F_DNS-8C4FFF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Cognito-DD344C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SES_(DKIM%2FDMARC)-DD344C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/CloudWatch_Alarms-FF4F8B?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Cross--Region_Replication-0288D1?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Restore_Drills-2E7D32?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Alias--Based_Rollback-455A64?style=for-the-badge" />
  <img src="https://img.shields.io/badge/VPC_%2F_PrivateLink-37474F?style=for-the-badge" />
</p>

### Security Engineering

<p>
  <img src="https://img.shields.io/badge/STRIDE_Threat_Modeling-B71C1C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/MITRE_ATLAS-C62828?style=for-the-badge" />
  <img src="https://img.shields.io/badge/OWASP_LLM_Top_10-D32F2F?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Prompt_Injection_Defense-880E4F?style=for-the-badge" />
  <img src="https://img.shields.io/badge/KMS_Envelope_Encryption-283593?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Zero--Knowledge_Design-1A237E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Shamir_Secret_Sharing-3949AB?style=for-the-badge" />
  <img src="https://img.shields.io/badge/MFA_(TOTP%2C_Passkeys%2FWebAuthn)-1565C0?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Least--Privilege_IAM-37474F?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Tenant_Isolation-00695C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Secrets_Management-5D4037?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Incident_Response-AD1457?style=for-the-badge" />
  <img src="https://img.shields.io/badge/PIPEDA_%2F_HIPAA_Controls-4E342E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Supply_Chain_(SHA--pinned_actions)-263238?style=for-the-badge" />
</p>

### Testing / Quality / DevSecOps

<p>
  <img src="https://skillicons.dev/icons?i=jest,selenium,cypress,githubactions&perline=14" alt="Testing"/>
</p>

<p>
  <img src="https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Property--Based_Tests-6A1B9A?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Concurrency_Tests-4527A0?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Coverage_Gates_(80%25%2B)-2E7D32?style=for-the-badge" />
  <img src="https://img.shields.io/badge/bandit-1565C0?style=for-the-badge" />
  <img src="https://img.shields.io/badge/pip--audit-0277BD?style=for-the-badge" />
  <img src="https://img.shields.io/badge/checkov-7D3C98?style=for-the-badge" />
  <img src="https://img.shields.io/badge/gitleaks-B00020?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=white" />
  <img src="https://img.shields.io/badge/mypy_%2B_ruff-000000?style=for-the-badge" />
</p>

### Tooling

<p>
  <img src="https://skillicons.dev/icons?i=git,github,vscode,pycharm&perline=14" alt="Tooling"/>
</p>

<p>
  <img src="https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI_Codex-000000?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Analytics_4-E37400?style=for-the-badge&logo=googleanalytics&logoColor=white" />
</p>

---

<div align="center">
  <sub>Dutch · English · Russian · Ukrainian</sub>
</div>
