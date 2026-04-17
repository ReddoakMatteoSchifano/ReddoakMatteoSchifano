# Matteo Schifano

Full-Stack Developer at **Reddoak**

Building modern web applications with TypeScript across the entire stack.

## Tech Stack

**Frontend** &mdash; React, Next.js, Tailwind CSS, Framer Motion
**Backend** &mdash; Node.js, REST APIs, Stripe
**Tools** &mdash; TypeScript, Git, Vercel, Google Cloud

## Currently

- Working on production web apps at Reddoak
- Exploring AI integration in developer workflows

## Developer Diary

I'm currently building **Yourang** — an AI-powered platform for voice agents, call center automation, and event reservation management. The stack is Python (FastAPI) on the backend and Next.js/React on the frontend, with real-time workflow orchestration, Stripe billing, and Twilio telephony integration. It's a complex product that touches AI, payments, scheduling, and multi-tenant SaaS — and I work across the full stack daily.

### Week of Apr 4–10, 2026

**Contact Lists Overhaul (Yourang)** — Tackled seven improvements to the contact lists module across the full stack. On the FastAPI side, extended the `GET /lists/{id}/contacts` endpoint with server-side sorting using the existing `-prefix` convention, then forwarded the params through the service and selector layers and covered the new behavior with integration tests. On the frontend, debugged a TanStack Table state desync where `table.setPageSize()` was never called, causing the rows-per-page selector to show a stale value silently. Also implemented auto-navigation into a newly created list, redesigned the page header with a subtitle hint, replaced raw `<textarea>` elements with the shared `Textarea` design-system component, and capped both tables to viewport height with internal scrolling. Added schema validation tests to keep the frontend API types in sync with the backend response contract.

**Codebase Refactor (Yourang)** — Removed the "actions" feature entirely from the codebase. Required careful tracing of all usages across routes, services, and frontend components to ensure no dead references or broken flows were left behind.

### Week of Mar 24–30, 2026

**Call Center & Campaigns** — Shipped the Predictive Dialer R1 with campaign management and orchestration. Built the campaign detail page with tabbed navigation, contact list popover, and route constants. Added label management for verified phone numbers with i18n support.

**Workflow Engine** — Implemented the If-Criteria node for conditional workflow branching with validation and i18n. Fixed parallel If-Criteria paths swallowing shared downstream nodes. Optimized criteria evaluation polling by passing friendly_id through the pipeline.

**Reservations** — Built copy-paste UX for schedule configuration and "Apply to all days" popover. Fixed handlePasteSchedule forcing target day open.

**Payments & Invoicing** — Integrated Stripe tax data into payment processing and Fattura in Cloud invoice generation with gross prices. Fixed promo code redemption and added cancellation selector on payment cancel.

**Infrastructure** — Switched default provider to Twilio with data migration. Removed Datadog RUM integration. Set up release workflow with proper token permissions. Added Claude agent definitions for development tasks.

**Side project: Ferie** — Added personal registry (anagrafica) with structured address fields, admin notifications, and permesso hours tracking with CSV export. Fixed lunch break subtraction in hours calculation.

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/matteo-vincenzo-schifano/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:matteo.vincenzo.schifano@gmail.com)
[![Website](https://img.shields.io/badge/matteoschifano.it-000000?style=flat&logo=safari&logoColor=white)](https://matteoschifano.it)
