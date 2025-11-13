# Guillaume Fontz - AI Security & Product Portfolio

**Live Portfolio**: [fontzgui.github.io](https://fontzgui.github.io)

## About This Portfolio

This repository contains my professional portfolio showcasing **AI-first development with security-first architecture**. I built [DreamVelo](https://dreamvelo.com) to prove that AI-assisted development can be as secure as traditional development when architected correctly.

## Target Roles

- **AI Security Engineer** - Design security controls for customer-facing AI products
- **AI Product Manager** - Help teams leverage AI tools effectively
- **Technical Customer Success Engineer** - Bridge technical implementation ↔ business value

## What's Inside

### Portfolio Website (`/portfolio-site/`)

- **index.html** - Homepage with AI-first development framework and metrics
- **project.html** - Complete DreamVelo case study
- **about.html** - Background, competencies, and technical skills
- **contact.html** - Contact form and direct contact information

Built with:
- HTML5 + Tailwind CSS (responsive design)
- Security-first principles
- Mobile-first approach
- No build process required

### Code Samples (Coming Soon)

Production code samples from DreamVelo demonstrating:
- Prompt injection prevention (15+ patterns blocked)
- Zero-trust architecture implementation
- AI-powered compatibility scoring algorithm
- Firestore security rules with email verification
- Multi-factor authentication (TOTP)

## Key Metrics: DreamVelo Project

**Proven Results:**
- ✅ **Zero** security incidents in production
- ✅ **28** STRIDE threats identified & mitigated
- ✅ **10,000+** lines generated via AI-assisted development
- ✅ **6 months** solo development (concept → production)

**Value Delivered:**
- 50-80 hours saved per job search
- 40-60% interview rate (vs 5-10% industry average)
- $5k-$18k ROI per user

**Technical Achievement:**
- Multi-platform deployment (Web live, iOS submitted, Android complete)
- <$100/month cost at scale (serverless architecture)
- <2 min rollback capability
- Comprehensive security monitoring

## The 5-Step AI-Assisted Development Framework

1. **Research & Threat Modeling** - STRIDE analysis before any code
2. **Specify Security Requirements** - Exact requirements, test cases, edge cases
3. **Prompt Engineering** - Detailed prompts with line numbers, examples, validation criteria
4. **Validate with Adversarial Testing** - 20+ malicious test cases, security code review
5. **Deploy & Monitor** - Production deployment with comprehensive logging

**Key Insight:** AI accelerates implementation (~70% success rate first try, 4x speed advantage). Humans ensure correctness through architecture, security design, and validation.

## Security Implementation Highlights

**Threat Modeling:**
- 28 STRIDE threats identified for DreamVelo
- All threats have documented mitigations
- Zero incidents since launch

**Zero-Trust Architecture:**
- No API keys in frontend (Cloudflare Workers proxy)
- Authentication at every layer (Firebase JWT)
- Server-side secret management (AWS Secrets Manager)

**AI Security:**
- 15+ prompt injection patterns blocked before reaching AI
- Input validation, output sanitization
- Rate limiting (10 requests/month for free tier)
- Security event logging

**Code Quality:**
- Security code review performed (5 findings documented)
- Adversarial testing with malicious inputs
- Production monitoring with CloudWatch

## Technology Stack

**Frontend:**
- Alpine.js SPA on AWS S3 + CloudFront CDN
- Tailwind CSS for responsive design
- Lucide icons

**Security:**
- Cloudflare Workers (edge security, API proxy)
- Firebase Auth (TOTP MFA, JWT)
- AWS WAF (DDoS protection, rate limiting)

**Backend:**
- AWS Lambda (receipt validation, email forwarding)
- AWS Secrets Manager (API key storage)
- Google Gemini Pro 1.5 (AI analysis, <$0.01 per request)

**Data:**
- Firebase Firestore (user data, application tracking)
- JSearch API (job listings)

**Payments:**
- Stripe (web)
- Apple In-App Purchase (iOS)
- Google Play Billing (Android)

## Lessons Learned: The Playbook

### What Works ✅

- **Security-first design:** Threat modeling before coding prevents incidents
- **Detailed specifications:** AI needs exact requirements ("Block 15 patterns, log events, return false" not "Add security")
- **Iterative validation:** Test immediately, fix fast (~2.5 iterations average per feature)
- **Zero-trust architecture:** No secrets in frontend, authentication at every layer

### When Human Must Step In ⚠️

- **iOS App Store rejections:** 4 rejections. AI couldn't debug Apple's feedback. I researched docs, fixed IAP issues.
- **Registration bugs:** Email verification modal issues (Nov 5-12). Required manual debugging, Firestore rules analysis.
- **Architecture decisions:** AI can't choose between approaches. I decided: zero-trust, serverless, multi-platform strategy.
- **Security code review:** AI generates code, but I review for vulnerabilities. Found 5 issues in initial implementation.

## Contact

**Email:** [guillfontz@gmail.com](mailto:guillfontz@gmail.com)
**LinkedIn:** [linkedin.com/in/fontzguillaume](https://www.linkedin.com/in/fontzguillaume/)
**Location:** Atlanta, Georgia (Open to remote)

## Availability

**Seeking roles at:**
- Leading AI companies
- AI-first startups
- Security-focused product teams

**Full-time roles:**
- AI Security Engineer
- AI Product Manager
- Technical Customer Success Engineer

**Consulting projects:**
- AI security audits
- Prompt engineering training

**Speaking engagements:**
- AI-assisted development
- Security-first AI

---

**© 2025 Guillaume Fontz. Built with AI-first development principles.**
