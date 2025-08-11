# ChADA1 v2 - No Clerk Authentication

This repository contains the cleaned version of the ChADA1 (Chat Analysis Dashboard) application with Clerk authentication completely removed.

## Changes Made
- ✅ Removed all Clerk dependencies from package.json
- ✅ Removed Clerk environment variables from Docker configuration  
- ✅ Cleaned layout.tsx of ClerkProvider wrapper
- ✅ Removed sign-in/sign-up pages with Clerk components
- ✅ Updated Docker configuration for production deployment

## Deployment
The GitHub Actions workflow automatically builds and pushes the Docker image to:
- `mambamental3mil/chada1-frontend:v2-no-clerk`
- `mambamental3mil/chada1-frontend:latest-no-clerk`

## NAS Deployment
Your Portainer stack has been updated to use the new v2-no-clerk image.

To trigger a new build, push changes to this repository or run the workflow manually.

## Application Structure
This is a Next.js 15.4.5 application with:
- TypeScript
- Prisma ORM
- Tailwind CSS
- Custom mock authentication for development
- PostgreSQL database support