# 🧱 Preferred Tech Stack (General Reference)

A running list of tools, libraries, and frameworks I use or would use across projects.

---

## Frontend (Web + Mobile UI)

- React Native + React (shared logic), logtail
- UI / Components: NativeWind UI, shadcn/ui, lucide-animated (icons)
- Animation & advanced lists: React Native Reanimated, Virtua (fast lists), xyflow (flow/graph UI)
- Drag & drop: @hello-pangea/dnd
- Rich text editing: Tiptap
- Forms: React Hook Form
- Motion / animations: **motion.dev**
- Command palette UI: CMDK
- Code highlighting / formatting: Ultracite
- Logo / brand assets: Logo.dev (company logo lookup by domain)
- Maps & geospatial: **Mapbox**

---

## State, Data, Validation & Backend

- Global state: Legend State
- Backend-as-a-service / realtime: Convex
- Runtime: **Bun**
- Server framework: **ElysiaJS** (Bun-native) + Hono (lightweight APIs)
- Validation & schemas: Zod
- Search engine: Typesense
- Queues / rate limits / caching: **Upstash (Redis / Kafka)**
- Background jobs / event workflows: **Inngest**
- Authentication / user management: Clerk
- Domains: Porkbun
- Hosting & deployment: Vercel (frontend/edge), Render (apps/containers)
- Infra tools: Docker, Caddy, Ngrok, Cloudflare
- Networking / mesh VPN: Tailscale

---

## Storage, Media & Files

- Object storage: **Cloudflare R2**
- Uploads & media handling: UploadThing
- Asset optimization (optional): ImageKit

---

## Services & Integrations

- Email: Resend
- Payments: Stripe
- Subscriptions / mobile monetization: RevenueCat
- Analytics / product metrics: PostHog
- Document OCR: **DocStrange by Nanonets**
- Document workflows / e-sign: Documenso
- Scheduling / bookings: Cal.com
- Automation / workflow glue: n8n
- Link management: Dub
- Browser automation / agent systems: Browserbase, Stagehand, Director
- Video / realtime calls: Daily.co

---

## Monitoring, Logs & Observability

- Error tracking: **Highlight.io** (over Sentry)
- Logging: Logtail (Betterstack) or Axiom
- Performance insights (edge, workers, etc.): Cloudflare Analytics

---

## Audio, Voice & AI

- FluidAudio — CoreML (transcription, TTS, VAD, diarization)
- Pipecat — streaming voice agent pipeline
- AI / Compute:
  - Cerebras — high-throughput open-weights compute
  - Gemini — best reasoning + multimodal model suite
- Vector DB / embeddings: LanceDB (optional)

---

## Testing & QA

- **Vitest** (unit tests)
- **Playwright** (browser, E2E tests)
- **bun test** (lightweight native test runner)

---

## DevOps & Hosting Layers

- Hosting: Vercel, Render
- CDN / DNS / security: Cloudflare
- Containers: Docker
- Local tunnels: Ngrok
- Reverse proxy & TLS: Caddy
- Networking: Tailscale

---
