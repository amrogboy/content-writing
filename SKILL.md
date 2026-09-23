---
name: content-writing-skill
description: Write SEO- and LLM-optimized articles that follow Google's content guidelines and are structured for AI answer engines (ChatGPT, Google AI Overviews, Perplexity). Use this whenever the user asks to write a blog post, article, or web page, do keyword research, check for topic/keyword cannibalization before writing, audit E-E-A-T or schema on a page, build an FAQ section, or optimize existing content for search or AI visibility. Covers the full pipeline: cannibalization check, keyword research, outline, in-article images, internal linking, YAML frontmatter, E-E-A-T signals, schema checklist, and FAQ checklist.
compatibility: Works best with a keyword/SERP research tool (Google Search Console, Ahrefs, SEMrush, Google Trends, or similar) and an image-generation or stock-image connector (Canva, DALL-E, Midjourney, or similar) available. Falls back to manual instructions for both if no such tool is connected.
---

# Content Writing Skill

Writes content that ranks in Google, gets cited by AI answer engines (ChatGPT, AI Overviews, Perplexity), and holds up to an editorial quality bar — not generic AI-sounding filler. The workflow front-loads the decisions that are expensive to get wrong (should this even be written, what's the real angle) before any drafting happens.

## Why the order matters

Most bad content briefs happen because someone starts writing before checking whether the topic is worth writing about, or whether it competes with something that already exists. Do the scoping and cannibalization check first — it's much cheaper to redirect a topic before a draft exists than to discover the overlap after publishing and have two pages compete with each other in search.

## Step 1 — Scope the piece

Before researching keywords, establish:

1. **Topic/keyword** the user wants to target, and the **search intent** behind it (informational, commercial, transactional, navigational) — this determines format (guide vs. comparison vs. landing page vs. FAQ hub).
2. **Audience and funnel stage** — who's reading this and what do they already know.
3. **Site/domain** it's going on, if known — needed for the cannibalization check and internal linking in Step 2 and Step 5.
4. **Available data sources** — Search Console, Ahrefs/SEMrush, Google Trends, or similar, if connected. If none are connected, say so and proceed with judgment-based keyword research (Step 3 covers the manual fallback).

## Step 2 — Topic and keyword cannibalization check

Do this before researching keywords or outlining — it can change or kill the topic entirely.

1. If a site/domain is known and a search-data tool is connected, pull the site's existing indexed pages and check for:
   - An existing page already ranking for the same primary keyword or a close variant.
   - Multiple pages targeting overlapping intent (e.g., two "best X for Y" articles).
2. If no tool is connected, ask the user whether a similar page already exists on their site, or search the site (`site:domain.com keyword`) as a manual check.
3. **Verdict — pick one and say so explicitly before proceeding:**
   - **Clear to write** — no meaningful overlap.
   - **Write, but differentiate** — an existing page is adjacent but not identical; state exactly how this piece's angle, depth, or intent differs, and note it should be interlinked with (not competing against) the existing page.
   - **Don't write this — here's why, and an alternative** — a page already owns this keyword/intent well. Explain the overlap concretely (which page, which keyword) and propose 1-3 alternative angles or subtopics that would be additive instead of duplicative (e.g., a more specific long-tail variant, a different search intent, a follow-up/advanced topic, or a comparison the existing page doesn't cover).

Don't skip straight to writing when cannibalization is found — the recommendation not to write, or to redirect, is a legitimate and often the most valuable output of this step.

## Step 3 — Keyword research

1. If a keyword tool is connected (Search Console, Ahrefs, SEMrush, Google Trends), pull: search volume, difficulty/competition, related and question-based queries, and current trend direction for the primary keyword and 3-5 close variants.
2. If no tool is connected, do this manually: reason about likely search intent and phrasing from the topic itself, check what currently ranks by describing typical SERP patterns for that query type, and flag that volume/difficulty figures should be verified with a real tool before final commitment.
3. Settle on: one **primary keyword**, 2-4 **secondary keywords** to weave in naturally, and a shortlist of **question-based queries** (these become FAQ candidates in Step 8 and are often what AI Overviews / ChatGPT pull directly).
4. Don't keyword-stuff. The goal is covering the topic's real subtopics and questions completely, not hitting a density target — modern search and AI systems reward comprehensive, well-organized coverage over repeated phrases.

## Step 4 — Outline and structure

1. Build a heading structure (single H1, logical H2/H3 nesting) that mirrors how someone would actually explain this topic to a colleague — lead with the direct answer, then support it. This "answer-first" structure is what both featured snippets and AI answer engines tend to extract.
2. Map secondary keywords and question-based queries from Step 3 to the sections where they belong naturally — don't force one section to cover everything.
3. Plan internal links now, not after drafting (see Step 6) — decide which existing pages this piece should link to and which existing pages should link back to it, so the draft is written with those anchor points in mind.
4. Plan image placement now too (see Step 5) — decide roughly where a diagram, screenshot, or illustrative image adds real comprehension value, rather than dropping in decorative stock photos afterward.

## Step 5 — Write the draft

1. Write in the outlined structure. Open each major section with the direct answer or key point, then elaborate — don't bury the point at the end of a paragraph.
2. **E-E-A-T signals** — weave these in naturally, don't bolt them on at the end:
   - **Experience**: first-hand detail, specific examples, screenshots of actually doing the thing, not just describing it in the abstract.
   - **Expertise**: correct terminology, depth appropriate to the topic, and — if the site supports author bios — a byline naming a real author with relevant credentials.
   - **Authoritativeness**: cite credible external sources for claims that need it (data, statistics, regulations), and link to the site's own authoritative pages where relevant.
   - **Trustworthiness**: accurate, current information; clear disclosure of any commercial relationship; no unsupported claims.
3. **Write for people first, but structure for machines too** — clear, direct prose with genuinely useful information is what both Google's ranking systems and AI answer engines are trying to reward. Avoid the tells of low-effort AI-generated content: generic filler sentences, repetitive transitional phrases ("In today's fast-paced world...", "It's important to note that..."), padding to hit a word count, and vague claims with no specifics.
4. Keep paragraphs short (2-4 sentences) and use lists/tables where they genuinely aid scanability — not as a formatting reflex.

## Step 6 — In-article images

1. For each image slot planned in Step 4, decide whether it needs to be **generated** (illustrative/conceptual) or is better as a **real screenshot/photo** (product UI, real data, a real place) — don't generate a fake screenshot of software.
2. If an image-generation or design connector (Canva, DALL-E, Midjourney, or similar) is available, use it to produce the illustrative images; otherwise describe exactly what each image should show (composition, style, any text overlay) so the user or a designer can produce it.
3. Every image needs: descriptive alt text (not keyword-stuffed — describe what's actually in the image), a descriptive filename (not `IMG_1234.jpg`), and — if the page is image-heavy — inclusion in an image sitemap.
4. Don't place the first meaningful image so it becomes an unoptimized LCP (Largest Contentful Paint) element — flag that hero/above-the-fold images need proper sizing and modern formats (WebP/AVIF).

## Step 7 — Internal linking

1. Add the internal links planned in Step 4: links out to relevant existing pages (using descriptive, natural anchor text — never "click here"), and note which existing pages should be updated to link back to this new piece so it isn't an orphan.
2. Check link depth: this page should be reachable within 3-4 clicks from the homepage; if it won't be, flag that as a follow-up task for site navigation/hub pages, not something this piece alone can fix.
3. Confirm the new piece doesn't compete with the pages it's linking to (this should already be resolved from Step 2, but double-check once the draft's actual angle is final).

## Step 8 — YAML frontmatter and metadata

Populate frontmatter completely and correctly for the target CMS. At minimum:

```yaml
title: "..."           # unique, includes primary keyword naturally, appropriate length
description: "..."     # unique meta description, compelling, within length, includes primary keyword
slug: "..."             # clean, lowercase, hyphenated, matches primary keyword where natural
date: "..."
author: "..."           # real named author if the site supports E-E-A-T author bios
canonical: "..."        # self-referencing unless intentionally canonicalizing elsewhere
og_title / og_description / og_image / twitter_card
```

Validate the frontmatter is well-formed YAML (correct indentation, quoting on strings with special characters, no duplicate keys) before handing it off — a malformed frontmatter block can break the whole page build.

## Step 9 — Schema markup checklist

Check which of these genuinely apply and are accurate to the actual page content (never add schema for something not visibly present on the page — that's a policy violation risk, not just a missed opportunity):

- `Article` / `BlogPosting` — headline, author, datePublished, dateModified, image
- `BreadcrumbList` — matches the actual category hierarchy
- `FAQPage` — only if Step 10's FAQ section is genuinely on the page
- `HowTo` — only for genuine step-by-step instructional content
- `Product` / `Offer` / `AggregateRating` / `Review` — only for genuine product pages with real reviews visible
- `Organization` / `Person` (author) — for E-E-A-T and knowledge panel eligibility
- JSON-LD format (preferred over microdata)

## Step 10 — FAQ checklist

1. Pull 3-6 real questions from Step 3's question-based queries — these are the ones most likely to already be searched, and most likely to get pulled into AI Overviews or cited by ChatGPT/Perplexity when they answer a related question.
2. Write direct, complete answers (2-4 sentences) that would make sense read in isolation, since AI answer engines often extract just the answer without surrounding context.
3. Don't pad the FAQ with questions nobody would ask just to hit a count — a shorter, genuinely useful FAQ beats a padded one, both for readers and for schema-quality signals.
4. Match the on-page FAQ content exactly to the `FAQPage` schema from Step 9 — mismatched schema/visible-content is a Google policy violation.

## Step 11 — AI answer engine and index-level optimization pass

Before finalizing, check:

1. **Extractability**: is the core content in the raw server-rendered HTML, or only injected client-side by JavaScript? AI crawlers (GPTBot, ClaudeBot/anthropic-ai, PerplexityBot, Google-Extended) generally don't execute JS — if this is a client-rendered site, flag that as a technical dependency outside this skill's scope, not something the content itself can fix.
2. **`/llms.txt`**: if the site has one, check whether this new page should be referenced in it.
3. **AI crawler access**: note (don't assume) whether the site's robots.txt deliberately allows or blocks GPTBot/ClaudeBot/Google-Extended/PerplexityBot — this is a site-level decision, but content that's blocked from AI crawlers won't be cited by AI Overviews or ChatGPT regardless of quality.
4. **Answer-first structure** (from Step 4): re-confirm the direct answer to the core question appears early and cleanly — this is the single highest-leverage factor in whether AI Overviews and chat answer engines extract and cite the page.
5. **Indexability**: correct canonical tag, no accidental `noindex`, included in the sitemap once published.

## Step 12 — Final output

Deliver:

```
# [Working Title]

## Cannibalization verdict (Step 2)
[Clear to write / Write with differentiation / Don't write — alternative suggested]

## Target keywords
Primary: ...
Secondary: ...
Question-based (→ FAQ): ...

## Full draft
[The article, in the target CMS's format — markdown or otherwise]

## YAML frontmatter
[Complete block from Step 8]

## Schema to implement
[Checklist from Step 9, only the applicable ones, each with the specific fields to fill]

## FAQ section
[From Step 10, matching the schema above]

## Image briefs
[What each image should show, and whether it was generated or needs to be sourced]

## Internal linking notes
[Links added, and existing pages that should link back]

## Follow-ups outside this piece
[E.g., "site blocks GPTBot in robots.txt — flag to dev", "hub page needed so this isn't 4+ clicks from home"]
```

Keep the draft itself clean prose — the checklist/metadata sections around it are what make it easy to hand off to an editor, a CMS, or a developer without back-and-forth.
