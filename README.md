# PetMorph Public Repository

Public project documentation for **PetMorph**: AI pet-to-human portrait generation.

- Live app: https://petmorph.app/
- Product focus: upload a pet photo, choose a style, generate and download/share

## Why this repository is lightweight

PetMorph runs as an actively maintained production product.  
The full application source is private for security and operational reasons.

This public repository exists to provide:

- Product overview and architecture notes
- Public changelog
- Security reporting path
- Issue tracking for users and partners

## Product capabilities (public)

- Pet photo upload and guided generation flow
- Multiple style presets for pet-to-human transformation
- Credit-based usage model with pricing plans
- User dashboard for generation history and account actions
- SEO-focused and multilingual content surfaces

## High-level stack

- Frontend: Next.js + React + TypeScript
- Backend: Supabase (Auth, Postgres, Storage, RLS)
- Payments: Stripe and provider integrations
- AI generation pipeline: async job flow + storage lifecycle management
- Operations: CI workflows, scripts, and deployment checklists

See:

- `docs/public-architecture.md`
- `docs/public-roadmap.md`
- `CHANGELOG.md`

## Repository contents

- `README.md`: public project summary
- `CHANGELOG.md`: public updates and milestones
- `SECURITY.md`: responsible disclosure process
- `CONTRIBUTING.md`: contribution guidelines
- `docs/`: public technical and roadmap docs
- `.github/`: issue templates and basic docs checks

## Not included in this repository

- Production source code
- Infrastructure secrets and deployment credentials
- Internal runbooks with sensitive implementation details

## Feedback and support

- Bug report / feature request: open a GitHub Issue
- Product support: use the support/contact channel on https://petmorph.app/

## License

This repository is distributed under a proprietary license. See `LICENSE`.
