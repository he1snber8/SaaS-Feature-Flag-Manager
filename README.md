# Bitasmbl-SaaS-Feature-Flag-Manager-0109d8-9b15c1dd694d

## Description
Build a production-ready SaaS app for managing feature flags across projects. The Java backend exposes secure REST APIs for tenant, project, and flag management, while the Next.js frontend provides a modern dashboard. Focus is on production readiness: auth, validation, error handling, logging, environment configs, and basic deployability.

## Tech Stack
- Java
- Next.js

## Requirements
- Implement tenant-aware feature flag listing where each API call only returns flags belonging to the authenticated tenant.
- Add a production build script and minimal README deployment section for both backend and frontend.

## Installation
bash
git clone https://github.com/he1snber8/SaaS-Feature-Flag-Manager.git
cd SaaS-Feature-Flag-Manager

Backend (Java): use standard Java build tooling.
Frontend (Next.js):
bash
cd frontend
npm install


## Usage
Backend: run the Java application with production environment configs.
Frontend:
bash
cd frontend
npm run dev


## Implementation Steps
1. Add auth ensuring all API calls identify the authenticated tenant.
2. Implement tenant, project, and flag REST endpoints in Java.
3. Enforce tenant-aware filtering on all feature flag listing APIs.
4. Add validation, error handling, and logging across backend APIs.
5. Configure environment-based settings for backend and frontend.
6. Implement Next.js dashboard pages for managing tenants, projects, and flags.
7. Add production build script for backend using the chosen Java build tool.
8. Add `npm run build` for Next.js production builds.
9. Document minimal deployment commands for backend and frontend.

## API Endpoints
- `GET /flags` – list feature flags for the authenticated tenant only.