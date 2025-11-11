# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by [DevOps Engineer](octoacme-roles-and-personas.md))
- Release notes drafted (reviewed by [Customer Support Lead](octoacme-roles-and-personas.md))
- Rollback / mitigation plan documented (prepared by DevOps Engineer)
- Smoke tests prepared
- Support documentation and knowledge base updated (coordinated with Customer Support Lead)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable) (coordinated by DevOps Engineer)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred, managed by DevOps Engineer)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support
- [ ] Customer Support Lead notified and support documentation available
- [ ] Monitor system health and error rates (DevOps Engineer tracks)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call ([DevOps Engineer](octoacme-roles-and-personas.md) leads)
  - Rollback to last known-good release if necessary (DevOps Engineer executes)
  - [Customer Support Lead](octoacme-roles-and-personas.md) coordinates customer communication
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
