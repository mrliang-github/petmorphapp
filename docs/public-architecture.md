# Public Architecture Overview

This document describes the high-level architecture of the PetMorph product.

## 1. Product layers

- Web app layer: user-facing pages and dashboard
- API and orchestration layer: request validation, job orchestration, and state updates
- Data layer: user identity, credits, transactions, and generation metadata
- Storage layer: generated media and lifecycle cleanup
- Observability and operations layer: logs, error tracking, and CI checks

## 2. Core flow

1. User uploads a pet image and selects style options.
2. Server validates request and account state.
3. Generation job is dispatched to AI backend pipeline.
4. Output media is stored and linked to user generation history.
5. Credit transactions and status are persisted for auditability.
6. User accesses results in dashboard/gallery views.

## 3. Platform components (high-level)

- Frontend: Next.js + React + TypeScript
- Data/Auth/Storage: Supabase
- Payments: integrated checkout and webhook processing
- Security controls: auth checks, RLS policies, request guards
- Automation: scripts for data validation, i18n checks, and deployment verification

## 4. Public boundaries

This repository intentionally excludes:

- Private source modules and business logic internals
- Environment secrets and private infrastructure configuration
- Internal incident and operations playbooks
