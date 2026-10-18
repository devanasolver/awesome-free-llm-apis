# Awesome Free LLM APIs

A curated list of LLM APIs with **permanent free tiers** (ongoing, no-expiry API access), plus freemium options, one-time trial credits, and a paid cost comparison.

**Verified on October 18, 2026** against each provider's official pricing/docs pages (linked per entry). Prices and limits change often - re-check the source before building on any of these. No API keys are (or should ever be) published in this list.

> **Watch out:** GitHub Models, a staple of older "free LLM API" lists, was **fully retired on July 30, 2026** - playground, catalog, inference API and BYOK are all gone. Migration path: Microsoft Foundry. [Source](https://github.blog/changelog/2026-07-30-github-models-is-now-retired/)

## Contents

- [Permanent free tiers](#permanent-free-tiers)
- [Freemium (free keys with restrictions)](#freemium-free-keys-with-restrictions)
- [Trial credits (one-time, not permanent)](#trial-credits-one-time-not-permanent)
- [Paid cost comparison](#paid-cost-comparison)

---

## Permanent free tiers

These give you an API key and ongoing free usage that renews (daily/monthly limits) with no credit card required unless noted.

| Provider | What you get for free | Limits (as verified) | Get a key |
| --- | --- | --- | --- |
| **Google Gemini API** (AI Studio) | Current Gemini models "free of charge" on the free tier (e.g. Gemini 3.8 Flash). Note: free-tier content may be used to improve Google products; flagship Gemini 4 Argon is **not** on the free tier. | Per-model RPM/TPM/RPD limits; RPD resets midnight Pacific. Exact limits shown on the AI Studio limits page. | [aistudio.google.com](https://aistudio.google.com/) · [Pricing](https://ai.google.dev/gemini-api/docs/pricing) · [Rate limits](https://ai.google.dev/gemini-api/docs/rate-limits) |
| **GroqCloud** | Fast inference for open models (GPT OSS 120B/20B, Qwen3.8-27B, Llama Guard, Whisper). | Free plan, per-model limits, e.g. GPT OSS 120B: 30 RPM / 1K RPD / 200K TPD. | [console.groq.com](https://console.groq.com/) · [Rate limits](https://console.groq.com/docs/rate-limits) · [Models & prices](https://console.groq.com/docs/models) |
| **OpenRouter** (`:free` models) | One API key for many models; every model with a `:free` variant costs $0; `openrouter/free` router picks a free model automatically. | 50 free-model requests/day; raised to 1,000/day after you have purchased at least $10 of credits. 5.5% fee ($0.80 min) applies when buying credits, not to free usage. | [openrouter.ai/keys](https://openrouter.ai/keys) · [FAQ](https://openrouter.ai/docs/faq) |
| **Mistral Studio** (free mode) | API keys enabled by default with no credit card; includes monthly free usage across Mistral models. | Lowest rate limits (evaluation/prototyping): RPS, tokens/min and tokens/month caps shown on the Admin Panel Limits page. | [console.mistral.ai](https://console.mistral.ai/) · [Quickstart](https://docs.mistral.ai/getting-started/quickstarts/studio/activate-and-generate-api-key) · [Usage & limits](https://docs.mistral.ai/admin/billing-usage/usage-limits) |
| **SambaNova Cloud** | Free tier (no payment method linked) on production models: Llama-3.3-70B, GPT OSS 120B, DeepSeek-V3.1. | 20 RPM, daily request cap, 200K tokens/day per model (TPD applies to free tier only). | [cloud.sambanova.ai](https://cloud.sambanova.ai/) · [Rate limits](https://docs.sambanova.ai/docs/en/models/rate-limits) · [Plans](https://cloud.sambanova.ai/plans) |
| **Cloudflare Workers AI** | ~30 open models (Llama, Qwen, GLM, DeepSeek distill, embeddings) via REST API. | 10,000 Neurons/day free on the Workers Free plan; resets 00:00 UTC. Above that needs Workers Paid ($0.011 / 1K Neurons). Some frontier models require a paid billing method. | [dash.cloudflare.com](https://dash.cloudflare.com/) · [Pricing](https://developers.cloudflare.com/workers-ai/platform/pricing/) |

## Freemium (free keys with restrictions)

| Provider | Free offer | Restriction | Source |
| --- | --- | --- | --- |
| **Cohere** | Trial API key created automatically at signup; API calls on it are free. | Rate limited; **not permitted for production or commercial use**. Production keys are pay-as-you-go. | [cohere.com/pricing](https://cohere.com/pricing) |
| **Hugging Face Inference Providers** | One API for 200+ models across providers (routed or BYOK). | Free accounts get **no** included monthly credits; PRO ($9/mo) includes $2/mo inference credits, otherwise buy credits. Not a free tier anymore. | [hf.co/docs/inference-providers/pricing](https://huggingface.co/docs/inference-providers/pricing) |

## Trial credits (one-time, NOT permanent)

Do not mistake these for free tiers - they expire or require payment up front.

| Provider | Offer | Catch | Source |
| --- | --- | --- | --- |
| **Cerebras** | $5 free credits | Requires a verified payment method; credits expire 30 days after grant; access pauses when exhausted. Cerebras explicitly states it has no permanently free tier. | [cerebras.ai/pricing](https://www.cerebras.ai/pricing) · [Rate limits FAQ](https://inference-docs.cerebras.ai/support/rate-limits) |
| **Together AI** | None | No free trial; platform access requires a minimum $5-$15 prepaid credit purchase. | [docs.together.ai](https://docs.together.ai/docs/billing-credits) |
| **xAI (Grok)** | None for the API | Playground is free to test; API usage is billed per token from $0 cumulative spend (Tier 0). | [x.ai/api](https://x.ai/api) · [docs.x.ai rate limits](https://docs.x.ai/developers/rate-limits) |
| **DeepInfra** | None | Pay-as-you-go only. | [deepinfra.com/pricing](https://deepinfra.com/pricing) |
| **Fireworks AI** | None (general) | Prepaid credits with a payment method; occasional per-model promos. | [fireworks.ai/pricing](https://fireworks.ai/pricing) |
| **GitHub Models** | None | **Retired 2026-07-30.** | [changelog](https://github.blog/changelog/2026-07-30-github-models-is-now-retired/) |

## Paid cost comparison

USD per 1M tokens (input / output), standard tier, as verified October 18, 2026. Sorted roughly flagship -> budget. "Intro" prices are time-limited promos the provider has already announced will rise.

| Provider | Model | Input | Output | Notes | Source |
| --- | --- | --- | --- | --- | --- |
| OpenAI | GPT-5.2 | $1.75 | $14.00 | Batch/flex cheaper; no free tier | [platform.openai.com/docs/pricing](https://platform.openai.com/docs/pricing) |
| OpenAI | GPT-5 mini | $0.25 | $2.00 | Budget option | same |
| OpenAI | GPT-5 nano | $0.05 | $0.40 | Cheapest OpenAI model | same |
| Anthropic | Claude Opus 5 | $5.00 | $25.00 | No free API tier | [docs.claude.com pricing](https://docs.claude.com/en/docs/about-claude/pricing) |
| Anthropic | Claude Sonnet 5 | $2.00 | $10.00 | Intro price made permanent | same |
| Anthropic | Claude Haiku 4.5 | $1.00 | $5.00 | | same |
| Google | Gemini 4 Argon | $2.00 | $10.00 | Intro through Nov 30, 2026, then $4/$20 | [ai.google.dev pricing](https://ai.google.dev/gemini-api/docs/pricing) |
| Google | Gemini 3.8 Flash | $0.75 | $3.75 | Intro through Dec 31, 2026, then $1.50/$7.50; **also on permanent free tier** | same |
| xAI | Grok 4.7 | $2.00 | $6.00 | $4/$12 above 200K prompt tokens | [docs.x.ai pricing](https://docs.x.ai/developers/pricing) |
| xAI | Grok 4.3 | $1.25 | $2.50 | 1M context | same |
| Mistral | Mistral Large | $0.50 | $1.50 | Batch -50%, cached input up to -90% | [mistral.ai/pricing](https://mistral.ai/pricing) |
| DeepSeek | deepseek-flash (V4.1 Flash) | $0.30 | $1.20 | Off-peak half price ($0.15/$0.60); 1M context | [api-docs.deepseek.com](https://api-docs.deepseek.com/quick_start/pricing) |
| DeepSeek | deepseek-v4-pro | $1.32 | $3.96 | Off-peak $0.66/$1.98 | same |
| Groq | GPT OSS 120B | $0.15 | $0.60 | ~500 tok/s; free tier also available | [console.groq.com/docs/models](https://console.groq.com/docs/models) |
| Groq | Qwen3.8-27B | $0.80 | $4.00 | ~450 tok/s | same |
| SambaNova | GPT OSS 120B | $0.22 | $0.59 | Developer tier (20M tokens/day cap) | [cloud.sambanova.ai/pricing](https://cloud.sambanova.ai/pricing) |
| SambaNova | Llama 3.3 70B | $0.60 | $1.20 | | same |
| DeepInfra | DeepSeek-V4-Flash | $0.09 | $0.18 | Very cheap hosted DeepSeek | [deepinfra.com/pricing](https://deepinfra.com/pricing) |
| DeepInfra | DeepSeek-V3.2 | $0.26 | $0.38 | | same |
| Together | Gemma 4 31B | $0.39 | $0.97 | Min $5 top-up to start | [together.ai/pricing](https://www.together.ai/pricing) |
| Cohere | (token models) | - | - | Per-token pricing not published on the public pricing page; trial keys are free but non-commercial | [cohere.com/pricing](https://cohere.com/pricing) |

## Methodology

- Every entry was checked on **October 18, 2026** against the provider's own pricing/docs page (linked in each row).
- "Permanent free" means an ongoing allowance that renews without payment; expiring credits and free playgrounds are listed separately.
- Prices exclude caching, batch, and regional variants unless noted. Always confirm on the source page before committing to a provider.

## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/) - use it however you like.
