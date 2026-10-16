<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg">
  <img src="./assets/header-light.svg" alt="Garret Grant — Software Engineer. TypeScript, full-stack products, APIs, and AWS." width="1200">
</picture>

Software Engineer at Realtor.com focused on TypeScript, JavaScript, full-stack applications, APIs, and reliable production systems. I also build and operate revenue-generating web products, working across the frontend, backend, payments, and deployment.

<a href="https://www.linkedin.com/in/garret-d-grant/"><img src="./assets/linkedin.svg" alt="Connect with Garret on LinkedIn" height="32"></a>
<a href="mailto:garret.grant.swe@gmail.com"><img src="./assets/email.svg" alt="Email Garret" height="32"></a>

[Open PepPal](https://app.peppal.app/) · [Watch the product demo](https://app.peppal.app/#demo) · [Peptide Dosing Protocols](https://www.peptidedosingprotocols.com/)

<p>
  <img src="./assets/icons/TypeScript.svg" alt="TypeScript" width="44" height="44">
  <img src="./assets/icons/JavaScript.svg" alt="JavaScript" width="44" height="44">
  <img src="./assets/icons/React-Dark.svg" alt="React" width="44" height="44">
  <img src="./assets/icons/NextJS-Dark.svg" alt="Next.js" width="44" height="44">
  <img src="./assets/icons/NodeJS-Dark.svg" alt="Node.js" width="44" height="44">
  <img src="./assets/icons/NestJS-Dark.svg" alt="NestJS" width="44" height="44">
  <img src="./assets/icons/PostgreSQL-Dark.svg" alt="PostgreSQL" width="44" height="44">
  <img src="./assets/icons/Prisma.svg" alt="Prisma" width="44" height="44">
  <img src="./assets/icons/AWS-Dark.svg" alt="AWS" width="44" height="44">
  <img src="./assets/icons/Docker.svg" alt="Docker" width="44" height="44">
</p>

## What I work on

- **Production systems:** Key contributor to Realtor.com's CloudFront and Lambda@Edge router, with work spanning production changes, observability, and service migrations.
- **Developer tooling:** Led development of all five versions of the TypeScript/NestJS Starter App and developer-portal template, standardizing microservice creation and deployment across 48 repositories, including 19 production services used by 13 teams.
- **Full-stack products:** Built the PepPal React/TypeScript application and NestJS/PostgreSQL backend, alongside Next.js marketing websites for PepPal and Peptide Dosing Protocols.

## Selected products

### [PepPal](https://app.peppal.app/) · Full-stack application

A production application for saved calculations, calendar-based tracking, and subscription features.

<a href="https://app.peppal.app/#demo">
  <picture>
    <source media="(prefers-reduced-motion: reduce)" srcset="./assets/peppal-demo-poster.jpg">
    <img src="./assets/peppal-pro-demo.gif" alt="Animated PepPal product preview: schedule a saved calculation, switch calendar views, and mark an entry complete. Click to watch the full 26-second demo." width="760">
  </picture>
</a>
<a href="https://app.peppal.app/#demo">
  <img src="./assets/peppal-demo-cta.svg" alt="Watch the 26-second PepPal product demo: calculate, save, schedule, and track." width="760">
</a>

[Watch the demo](https://app.peppal.app/#demo) · [Open the app](https://app.peppal.app/) · [Marketing website](https://www.peppal.app/)

- React, TypeScript, and Vite frontend with a NestJS API and PostgreSQL/Prisma data layer.
- Stripe subscription checkout, customer billing portal, and webhook-driven subscription updates.
- Resend transactional email, Listmonk subscriber workflows, and a separate Next.js marketing website.
- Multistage Docker build for the backend and a Docker-hosted Listmonk service.

### [Peptide Dosing Protocols](https://www.peptidedosingprotocols.com/)

A revenue-generating Next.js website with supplier-directory integrations, product discovery, and email subscriber workflows.

## Engineering case study: billing and email reliability

Across the PepPal app and website, I implemented billing and email workflows with explicit failure handling:

- **Verify incoming events:** Validate Stripe webhook signatures against the raw request body before processing checkout and subscription events.
- **Handle event ordering:** Check stored Stripe event timestamps before applying subscription updates so older events can be ignored.
- **Reduce duplicate emails:** Use Resend idempotency keys, persisted send markers, and database claims for trial-ending reminders.
- **Retry selectively:** Retry Listmonk rate-limit responses using `Retry-After` or exponential backoff. Avoid automatically retrying other failures that could duplicate an already-queued email.

## Tools I use

- **Languages:** TypeScript, JavaScript, SQL, Go, Bash
- **Applications and APIs:** Node.js, React, Next.js, NestJS, REST, GraphQL, PostgreSQL, Prisma, Jest
- **Cloud and delivery:** AWS, Docker, Kubernetes, Helm, Argo CD, CircleCI
- **Integrations and observability:** Stripe, Resend, Listmonk, Auth0, CloudWatch, New Relic, Backstage

## Public code and earlier projects

- **[NestJS API Starter](https://github.com/garretdgrant/nestjs-api-starter):** A personal API starter with Swagger documentation, health checks, Jest tests, and a multistage Docker build.
- **[DiamondDoor](https://github.com/garretdgrant/diamond_door):** An earlier full-stack learning project inspired by Glassdoor, built with React, Redux, Ruby on Rails, and PostgreSQL.

Outside of software, I enjoy working out, hiking, and the occasional pick-up basketball game.

