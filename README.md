# Content Writing Skill

A structured content writing skill for Claude and ChatGPT that produces SEO- and LLM-optimized articles following Google's content guidelines, built for both traditional search and AI answer engines (ChatGPT, Google AI Overviews, Perplexity).

## What it does

Point it at a topic or keyword and it runs a full editorial pipeline before and during drafting:

- **Topic/keyword cannibalization check** — run before any writing starts, so it can catch overlap with existing content and suggest an alternative angle or recommend not writing the piece at all
- **Keyword research** — primary/secondary keywords and question-based queries, using a connected SEO tool (Search Console, Ahrefs, SEMrush, Google Trends) when available, with a manual fallback when not
- **Outline and answer-first structure** — planned for both human readers and AI answer-engine extraction
- **Draft writing** with E-E-A-T (Experience, Expertise, Authoritativeness, Trustworthiness) signals woven in, and explicit guardrails against generic AI-slop filler
- **In-article images** — briefs for generated or sourced images, alt text, filenames, LCP considerations; uses an image-generation or design connector (Canva, DALL-E, Midjourney, etc.) when available
- **Internal linking** plan
- **YAML frontmatter** template and validation
- **Schema markup checklist** (Article, FAQPage, HowTo, Product, etc. — only what's genuinely applicable)
- **FAQ checklist** built from real question-based queries, matched to FAQPage schema
- **AI answer engine optimization pass** — extractability, `llms.txt`, AI crawler access (GPTBot/ClaudeBot/PerplexityBot), answer-first re-check
- **Structured final output** — draft plus every checklist, ready to hand to an editor, CMS, or developer

## Installation

Drop the `content-writing-skill/` folder into your Claude Skills directory (or wherever your agent host loads skills from), or point your agent's skill-loading config at this repo.

## Compatibility

No hard dependencies — the skill works standalone. It becomes more precise if you have:
- An SEO/keyword research tool connected (Google Search Console, Ahrefs, SEMrush, Google Trends)
- An image-generation or design connector (Canva, DALL-E, Midjourney, or similar)

Both are optional; the skill falls back to manual, judgment-based guidance for keyword research and image briefs when neither is available.

## License

MIT — see [LICENSE](LICENSE).
