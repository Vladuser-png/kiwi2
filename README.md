# Kiwi

> Marketplace of ready-made design resources — landing pages, websites, fonts, illustrations, icons.  
> **One subscription. Any tool. Instant download.**

---

## Repo Index

| Folder | What lives here | Status |
|--------|----------------|--------|
| [`research/`](./research/) | Competitor analysis, user insights, reference screens | 🟡 In progress |
| [`wireframes/`](./wireframes/) | Low-fi flows and layout sketches | 🟢 Core MVP + D3/E3 done |
| [`concept/`](./concept/) | Visual direction, moodboard, style exploration | ⬜ Not started |
| [`tokens/`](./tokens/) | Color, typography, spacing, radius design tokens | ⬜ Not started |
| [`components/`](./components/) | UI component specs and states | ⬜ Not started |
| [`design-system/`](./design-system/) | Full component library + usage guidelines | ⬜ Not started |
| [`handoff/`](./handoff/) | Dev-ready specs, assets, annotations | ⬜ Not started |

---

## Структура · Ключові IA-документи

| Файл | Зміст |
|------|-------|
| [`sitemap.md`](./sitemap.md) | Інвентар сутностей · Ієрархія екранів A–E + SIROTA · Навігація і глибина · Матриця трасування Jobs × Screens |
| [`flows.md`](./flows.md) | 4 user flows у Mermaid (Main Job · RJ-1 · RJ-2 · RJ-3) |
| [`ia.html`](./ia.html) | IA living document: дерево sitemap + flows + матриця покриття |
| [`research/jtbd.md`](./research/jtbd.md) | JTBD framework · 10 jobs · матриця Jobs × Персони |
| [`research/personas.md`](./research/personas.md) | 3 персони (1 валідована ✅ · 2 гіпотези ⚠️) |
| [`research/research.html`](./research/research.html) | Research hub (11 розділів) |

---

## Product in one line
Kiwi cuts designer search time by offering a curated, tool-agnostic library of polished UI resources — accessible via flat subscription or one-time purchase.

## MVP scope
- Catalog: **Landing Pages + Websites**
- Keyword search + filters (price · date · color · tags · tool)
- Auth, subscription & one-time payments (Stripe)
- Author uploads + admin moderation

## Stack
`Next.js 14` · `Supabase` · `Stripe` · `Cloudinary` · `Vercel`

## Wireframes

`wireframes/*.html` — 15 low-fi HTML pages, grayscale/semantic-HTML only (contract: [`wireframes/_conventions.md`](./wireframes/_conventions.md)).

- **Coverage:** 7 Core-MVP screens ([`wireframes/_screens.md`](./wireframes/_screens.md): A1, B1, C1, D1, D2, E1, E2) + D3 (one-time purchase) and E3 (account) from `_screens.md §Розширення`. Every real state (empty/error/loading/success) from the state matrix is its own page — nothing invented beyond what `flows.md` models.
- **Navigation:** every page carries the same left-hand `<nav class="wf-nav-tree">` (section → screen → state) and real `<a href>` links along the Main Job flow — no dead ends.
- **Out of scope on purpose:** RJ-3 (E1/E2 form error, C1 empty state) — already flagged in `_screens.md` as deferred, not a gap. S1–S4 (orphan screens) — sitemap.md recommends deleting/backlog, so no wireframes exist for them.
- Audit + fixed defects log → [`wireframes/_critique.md`](./wireframes/_critique.md).

## Links
- Full brief → [`CLAUDE.md`](./CLAUDE.md)
- Research → [`research/research.md`](./research/research.md)
