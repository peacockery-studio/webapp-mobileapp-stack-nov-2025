# Peacockery Preferred Stack

Personal tech stack reference. Tools, libraries, and frameworks I use or would use across projects.

## Usage Tiers

- **Always Use** — Default choice, reach for it every time
- **Used** — Battle-tested, use when the need fits
- **Researched** — Vetted and approved, but not yet used in production

---

## Quick Setup Commands

### React Native (Expo)

```bash
# Initialize with React Native Reusables
bunx --bun @react-native-reusables/cli@latest init

# Or full Expo + EAS setup
bun install --global eas-cli && bunx create-expo-app mobile && cd mobile && eas init
```

### React (Web)

```bash
bun init  # Select: React TS → shadcn + Tailwind
```

### Linting/Formatting (Ultracite + Biome)

```bash
bunx ultracite
# Always: full install, all AI configs (Claude, VSCode), all hooks (pre-commit, husky)
# Replaces ESLint and Prettier entirely
```

### Backend (Bun + Elysia)

```bash
bun init
bun add elysia @elysiajs/swagger @elysiajs/cors
```

---

## The Stack

### Frontend — Web

| Tool | Tier | Notes |
|------|------|-------|
| React + shadcn/ui + Tailwind | Always Use | `bun init` with React TS template |
| motion.dev (Framer Motion) | Always Use | Web animations |
| CMDK | Used | Command palette UI |
| xyflow | Used | Flow/graph UI — currently building with it |
| Tiptap | Researched | Rich text editor |
| @hello-pangea/dnd | Researched | Drag & drop (react-beautiful-dnd fork) |
| React Hook Form | Researched | |
| Virtua | Researched | Fast virtualized lists |
| lucide-animated | Researched | Animated icons |
| Logo.dev | Researched | Company logo lookup by domain |

### Frontend — Mobile (React Native)

| Tool | Tier | Notes |
|------|------|-------|
| Expo | Always Use | Everything goes through Expo + EAS |
| React Native Reusables (RNR) | Always Use | Primary mobile UI components |
| Reanimated 4 | Used | Comes with RNR |
| NativeWind UI | Fallback | Paid, nice for polished apps. RNR uses NativeWind under the hood |

### State & Data

| Tool | Tier | Notes |
|------|------|-------|
| Zustand | Always Use | Global state (familiar, go-to) |
| Zod | Always Use | Validation & schemas everywhere |
| Supabase | Used | Primary for heavier data needs |
| Convex | Used | Real-time/lightweight apps (chat, etc.) |
| Legend State | Researched | Fastest, but Zustand is the habit |

### Backend & Runtime

| Tool | Tier | Notes |
|------|------|-------|
| Bun | Always Use | Runtime for everything |
| ElysiaJS | Always Use | Bun-native server framework — with Swagger, CORS modules |
| Typesense | Used | Search engine — "factually insane" |
| Upstash Redis | Used (light) | Caching. Haven't used Kafka |
| Inngest | Researched | Background jobs / event workflows |

### Auth & Domains

| Tool | Tier | Notes |
|------|------|-------|
| Clerk | Always Use | Auth, every time |
| Porkbun | Always Use | Domain registrar |
| Cloudflare | Always Use | DNS, tunnels, and a lot of infra |

### Hosting & DevOps

| Tool | Tier | Notes |
|------|------|-------|
| Docker + Caddy + Cloudflare | Used | Self-hosting setup — want to do more |
| Vercel | Used | Easy deployments |
| Tailscale | Used | Mesh VPN / networking |
| Cloudflare Tunnels | Used | Replaced Ngrok |
| Render | Used (light) | Good, just don't reach for it often |

### Storage & Media

| Tool | Tier | Notes |
|------|------|-------|
| Cloudflare R2 | Always Use | Object storage for everything |
| UploadThing | Used (light) | Works, but R2 is primary |
| ImageKit | Researched | Asset optimization |

### Services & Integrations

| Tool | Tier | Notes |
|------|------|-------|
| Resend | Always Use | Email |
| n8n | Used | Automation / workflow glue — amazing |
| Browserbase + Stagehand v3 | Used | Browser automation — insane, very cool |
| Pipecat + Pipecat Cloud | Used | Voice agent pipelines — love it, certified |
| Stripe | Go-to pick | Payments (not much payment work yet) |
| RevenueCat | Go-to pick | Mobile subscriptions (researched only) |
| Daily.co | Researched | Video/realtime calls |
| Cal.com | Researched | Scheduling — certified |
| Dub | Researched | Link management |
| Documenso | Researched | E-sign / doc workflows |

### AI & ML

| Tool | Tier | Notes |
|------|------|-------|
| Gemini (2.5 Flash, Flash Lite, 3 preview) | Always Use | #1 for everything, including OCR |
| Cerebras | Used | First fallback — when you need crazy fast |
| FluidAudio | Used | CoreML transcription, TTS, VAD, diarization — amazing, current project |
| RapidOCR | Fallback | Local OCR option |
| Milvus | Would use | Vector DB (over LanceDB) |
| LanceDB | Researched | |

### Monitoring & Observability

| Tool | Tier | Notes |
|------|------|-------|
| Highlight.io | Researched | Error tracking (over Sentry) |
| Sentry | Researched | |
| Logtail / Axiom | Researched | Logging |
| Cloudflare Analytics | Researched | |

### Testing

| Tool | Tier | Notes |
|------|------|-------|
| Vitest | Used | Unit tests |
| Playwright | Used | E2E — through Stagehand v3 |
| bun test | Used | Lightweight native runner |

### Code Quality

| Tool | Tier | Notes |
|------|------|-------|
| Ultracite + Biome | Always Use | Replaces ESLint/Prettier. Full install with all hooks |

### Maps & Geo

| Tool | Tier | Notes |
|------|------|-------|
| Google Maps SDK / Places | Used | Go-to for 90% of cases, good free tier |
| Mapbox | Researched | Extra customization if needed |
