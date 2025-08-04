# List of agentic coding tools with free access to frontier models

> **TL;DR**: Compare agentic IDEs/CLIs by their free access to frontier models. Local models = unlimited free use, Gemini CLI = 3000 h/month, others have various limits.

Last verified: August 4, 2025 • PRs welcome • ⭐ Star if useful!

This list compares agentic coding systems (IDE and CLI) by how many hours of free access they provide to frontier models. Only agentic tools included.

---

## Methodology / assumptions

- Goal: compare agentic coding systems by how many hours of model usage their free tiers provide.
- Preset: 10 requests ≈ 1 AI-assisted coding hour (so 1,000 requests/day ≈ 100 hours/day).
- Token quotas: when vendors publish tokens (not requests), assume ~10k tokens ≈ 1 coding hour.
- If you spot an error or missing source link, please open an issue or a pull request.

---

## Local models (completely free)

Running open-weight frontier models locally provides unlimited coding assistance without API costs or usage limits. The best tools for local deployment include **[Cline](https://cline.bot/)** (VS Code extension with Plan/Act modes and MCP support), **[Aider](https://aider.chat/)** (command-line assistant with built-in Git integration), and **[Continue](https://www.continue.dev/)** (open-source VS Code extension supporting 200+ models). All work seamlessly with **[Ollama](https://ollama.com/)** to run frontier models like Qwen3-Coder, DeepSeek Coder V2, Codestral, and GLM-4.5.

**Note**: Frontier models require GPUs with substantial RAM/VRAM. See Simon Willison's article on [running GLM-4.5 AIR on his laptop to build Space Invaders](https://simonwillison.net/2025/Jul/29/space-invaders/) for a practical example.

---

## Free access to frontier models (most generous → least)

| Tool | Free Premium Hours | Models used (frontier vs fallback) | Model switching / available models | Notes |
|---|---:|---|---|---|
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | ≈100 h/day (1000 req/day) → ≈3000 h/month | Primary: Gemini 2.5 Pro; fallback: auto-switch to Gemini 2.5 Flash after Pro daily quota | Google models (Gemini family) via built-in auth; can also use [Google AI Studio](https://ai.google.dev/gemini-api/docs/pricing) or [Vertex AI](https://cloud.google.com/gemini/pricing) keys | Official limits for personal account: 60 req/min and 1000 req/day. Quotas for agent mode and CLI are combined. Alternative API keys: AI Studio free tier (100 RPD), Vertex AI free tier (express mode). [Rate limits documentation](https://ai.google.dev/gemini-api/docs/rate-limits) |
| [Warp](https://warp.dev/) | ≈15 h/month (150 AI requests/month) | Claude Sonnet 4, OpenAI o3, Gemini 2.5 Pro (frontier) | Multiple providers (Claude, OpenAI, Google) in terminal; model picker available | Free: 150 AI requests/month for frontier models; Pro $15/month (2,500 requests); Turbo $40/month (10,000 requests); Lightspeed $200/month (50,000 requests). Pay-as-you-go for overages. [Pricing details](https://www.warp.dev/pricing) |
| [Amazon Q Developer](https://aws.amazon.com/q/developer/) | ≈5 h/month (50 agent chats/month) | Anthropic Claude Sonnet 4 (frontier) | Claude family inside Q; cross-provider switching not supported | Perpetual Free Tier with 50 agentic chats/month; Pro tier unlimited chats at $19/month. [Pricing details](https://aws.amazon.com/q/developer/pricing/) |
| [Windsurf](https://windsurf.com/) | ≈2.5 h/month (25 prompt credits/month) | Free credits work with all frontier models (OpenAI, Anthropic, Google, xAI) | Multiple providers (OpenAI, Anthropic, Google, xAI) inside Windsurf | Free: 25 prompt credits/month for all frontier models; Pro $15/month (500 credits); Teams $30/user/month; Enterprise $60+/user/month. [Pricing details](https://windsurf.com/pricing) |
| [AWS Kiro](https://kiro.dev/) | Preview free with daily limits; pricing TBD | Claude Sonnet 4 / 3.7 | Claude family in preview; cross-provider not announced | Free during preview with waitlist. Initially planned tiered pricing (Free 50/Pro 1000/Pro+ 3000 interactions) but AWS removed pricing details, stating "updated pricing will be shared soon." [Introduction blog](https://kiro.dev/blog/introducing-kiro/) |

> Limits change fast. If you see a mistake, a newer quota/model, or want to add a new tool, open an issue or PR with a source. New tool contributions are welcomed!

---

## Tools with free tier but unclear frontier model usage limits

| Tool | Free Premium Hours | Models used (frontier vs fallback) | Model switching / available models | Notes |
|---|---:|---|---|---|
| [Cursor](https://cursor.com/) | Unknown ("limited agent requests") | Multiple frontier models available (e.g., Claude Sonnet/Opus, Gemini 2.5 Pro, GPT-4.x, o3) | Multiple providers; own keys supported; model picker in app | Hobby (free): limited agent requests and tab completions; Pro $20/month (extended agent limits); Ultra $200/month (20x usage); Teams $40/user/month. [Pricing details](https://cursor.com/en/pricing) |
| [Lovable](https://lovable.dev/) | ≈3 h/month (5 credits/day, 30/month cap) | Models not enumerated publicly | Vendor-hosted (no public model picker) | Free plan: 5 daily credits, max 30/month; Pro $25/month (100 credits), Teams $30/month (higher limits). [Messaging limits documentation](https://docs.lovable.dev/user-guides/messaging-limits) |
| [Bolt.new](https://bolt.new/) | ≈100 h/month (1M tokens/month) | Free-plan model not publicly specified | Unknown in app docs | Free plan: 1M tokens/month (resets monthly); paid plans from $20/month (10M tokens) to $200/month (120M tokens). [Token documentation](https://support.bolt.new/account-and-subscription/tokens) |
| [v0.dev](https://v0.dev/) | Model-dependent (Free includes $5 credits/month) | v0 models (routing varies) | v0 models (no cross-provider own-keys in app) | Credit-based billing: Free $5/month, Premium $20/month ($20 credits), Team $30/user/month ($30 credits). [Updated pricing blog](https://vercel.com/blog/improved-v0-pricing-5luSrdRUJsRvf1kXWoYGxh) |

> Know the official limits or models? Share a link in an issue or PR to update the table.

---

## Paid-only with generous usage quotas (no free frontier model access)

| Tool | Pricing | Models used (frontier vs fallback) | Model switching / available models | Notes |
|---|---:|---|---|---|
| [Claude Code](https://www.anthropic.com/claude-code) | Pro $20/month; Max $100/month or $200/month | Pro: Claude Sonnet 4; Max: Opus 4 + Sonnet 4 (Opus limited; falls back to Sonnet after quota) | Claude family | Weekly limits: Pro 40-80h Sonnet 4; Max $100 (140-280h Sonnet 4, 15-35h Opus 4); Max $200 (240-480h Sonnet 4, 24-40h Opus 4). [Pricing details](https://www.anthropic.com/pricing) |
| [GitHub Copilot](https://github.com/features/copilot/plans) | Pro $10/month; Pro+ $39/month; Business $19/user/month; Enterprise $39/user/month | Premium requests route to frontier models (varies by feature) | GitHub-managed models (no external own-keys for the agent) | Monthly frontier request limits: Pro (300), Pro+ (1500), Business (300/user), Enterprise (1000/user). Overage billing $0.04/request. [Plans details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot) |



