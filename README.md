# Hi, I'm Ibrohim Fayzullayev

**Frontend Engineer — React · Next.js · TypeScript | Full-stack delivery with Go, PostgreSQL, Docker**

Tashkent, Uzbekistan (UTC+5) · Open to on-site and remote roles

[![Portfolio](https://img.shields.io/badge/fayzullayev.uz-000000?style=flat-square&logo=googlechrome&logoColor=white)](https://fayzullayev.uz)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ibrohim-fayzullayev)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/Ibrohim_Fayzullayev)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:ibrokhim.fayzullaev.dev@gmail.com)

---

I build React and Next.js products for fintech, and I can take a feature from the database to the screen. I have 4 years of commercial experience and currently work at **Radius Mobile**.

- **Radius CRM** — the company's core operations system for installment retail. One app runs the whole sale: application → credit scoring → order → payment → overdue → collection. It has 25+ screens across 12 business areas and serves 100+ concurrent staff.
- **Amanat Pay** — a BNPL platform. I am the sole frontend engineer: I built it from an empty repository to an investor-ready MVP in about 4 months, including CI/CD and deployment.

Both are private company code. The projects below are mine and fully public.

## Featured project — [fayzullayev.uz](https://fayzullayev.uz)

A production platform I designed, built and run on my own: a bilingual (Uzbek / English) site and blog, an admin CMS and a REST API. It runs as three services on one Linux VPS behind Caddy with automatic HTTPS.

| Repository | What it is | Stack |
|---|---|---|
| [portfolio](https://github.com/IbrohimFayzullayev/portfolio) | Public site and blog: SSR / ISR, hreflang, JSON-LD, dynamic OG images | Next.js, TypeScript, Tailwind, Vitest |
| [portfolio-dashboard](https://github.com/IbrohimFayzullayev/portfolio-dashboard) | Admin CMS and Telegram Mini App | Next.js, TypeScript, TanStack Query, Vitest |
| [portfolio-api](https://github.com/IbrohimFayzullayev/portfolio-api) | REST API and ops Telegram bot | Go, PostgreSQL, sqlc, Docker |

What is inside:

- **CI/CD:** GitHub Actions runs lint, type-check and tests before every build. Images are pushed to GHCR with commit-SHA tags. A deploy only passes after it verifies that the running container is the new image and is healthy.
- **200+ automated tests:** Go unit tests, Go integration tests against a real PostgreSQL in CI, and Vitest in both Next.js apps. A CI check also fails if generated database code drifts from the schema.
- **Security:** HttpOnly cookie sessions with Origin checks and login rate limiting. Client IPs are read only from the proxy's header, so rate limits cannot be bypassed with a spoofed header.
- **Operations:** a Go Telegram bot handles alerts and admin tasks. It delivers messages through an outbox table and checks health with flap dampening. It also warns before TLS certificates expire and groups server and browser errors. A separate cron watchdog monitors the bot, and an external heartbeat covers the case where the whole server goes down.
- **Backups:** nightly PostgreSQL dumps go to Cloudflare R2 with object lock, and restores are tested.

## Stack

**Frontend:** React · Next.js (App Router, SSR / SSG / ISR) · TypeScript · TanStack Query · Tailwind CSS · Feature-Sliced Design · Telegram Mini Apps

**Backend & data:** Go · PostgreSQL · REST APIs · Node.js · GraphQL

**DevOps & quality:** Docker · GitHub Actions · Linux · Caddy · Vitest · Go testing

---

📫 The fastest way to reach me is [Telegram](https://t.me/Ibrohim_Fayzullayev) or [email](mailto:ibrokhim.fayzullaev.dev@gmail.com).
