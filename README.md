# List of agentic coding tools with free access to frontier models

> **TL;DR**: Compare agentic IDEs/CLIs by their free access to frontier models. Local models = unlimited free use, Gemini CLI = 3000 h/month, others have various limits.

Last verified: August 4, 2025 • PRs welcome • ⭐ Star if useful!

This list compares agentic coding systems (IDE and CLI) by how many hours of free access they provide to frontier models. Only agentic tools included.

---

## Methodology / assumptions

- Goal: compare agentic coding systems by how many hours of model usage their free tiers provide.
- Preset: 60 requests ≈ 1 AI-assisted coding hour (based on real-world task simulation).
- Token quotas: when vendors publish tokens (not requests), assume ~10k tokens ≈ 1 coding hour.
- If you spot an error or missing source link, please open an issue or a pull request.

---

## Local models (completely free)

Running open-weight frontier models locally provides unlimited coding assistance without API costs or usage limits. The best tools for local deployment include **[Cline](https://cline.bot/)** (VS Code extension with Plan/Act modes and MCP support), **[Aider](https://aider.chat/)** (command-line assistant with built-in Git integration), and **[Continue](https://www.continue.dev/)** (open-source VS Code extension supporting 200+ models). All work seamlessly with **[Ollama](https://ollama.com/)** to run frontier models like Qwen3-Coder, DeepSeek Coder V2, Codestral, and GLM-4.5.

**Note**: Frontier models require GPUs with substantial RAM/VRAM. See Simon Willison's article on [running GLM-4.5 AIR on his laptop to build Space Invaders](https://simonwillison.net/2025/Jul/29/space-invaders/) for a practical example.

---

## Agentic coding tools

---
### [Gemini CLI](https://github.com/google-gemini/gemini-cli)

**Free Tier:**
*   **Pro-grade usage:** ~1.7h/day of Gemini 2.5 Pro (est.)
*   **Fallback usage:** ~15h/day of Gemini 2.5 Flash (est.)
*   **Notes:** Free tier provides ≈100 daily requests for the Pro model before falling back to Flash.

**Paid Tiers (via Google AI Studio / Vertex AI):**
*   **Pay-as-you-go:** Removes daily request limits and offers higher rate limits (e.g., 60 RPM). Pricing is per-token.
*   **Notes:** Requires a Google Cloud project with billing enabled to use alternative API keys.

**Links:** [Rate Limits](https://ai.google.dev/gemini-api/docs/rate-limits) | [Pricing](https://ai.google.dev/gemini-api/docs/pricing)
---

### [Warp](https://warp.dev/)

**Free Tier:**
*   **Pro-grade usage:** ~2.5h/month across all frontier models (est.)
*   **Notes:** Free tier provides 150 AI requests per month, which can be used with Claude Sonnet 4, OpenAI o3, or Gemini 2.5 Pro.

**Paid Tiers:**
*   **Pro ($15/mo):** ~42h/month (est., 2,500 requests)
*   **Turbo ($40/mo):** ~167h/month (est., 10,000 requests)
*   **Lightspeed ($200/mo):** ~833h/month (est., 50,000 requests)
*   **Notes:** Pay-as-you-go available for overages.

**Links:** [Pricing](https://www.warp.dev/pricing)
---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**Free Tier:**
*   **Pro-grade usage:** ~0.8h/month of Claude Sonnet 4 (est.)
*   **Notes:** Perpetual free tier includes 50 agentic chats per month.

**Paid Tiers:**
*   **Pro ($19/mo):** Unlimited chats.

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)
---

### [Windsurf](https://windsurf.com/)

**Free Tier:**
*   **Pro-grade usage:** ~0.4h/month across all frontier models (est.)
*   **Notes:** Free tier provides 25 prompt credits per month, which can be used with models from OpenAI, Anthropic, Google, and xAI.

**Paid Tiers:**
*   **Pro ($15/mo):** ~8.3h/month (est., 500 credits)
*   **Teams ($30/user/mo):** Higher limits.
*   **Enterprise ($60+/user/mo):** Higher limits.

**Links:** [Pricing](https://windsurf.com/pricing)
---

### [AWS Kiro](https://kiro.dev/)

**Free Tier:**
*   **Pro-grade usage:** Free during preview with daily limits (models: Claude Sonnet 4 / 3.7).

**Paid Tiers:**
*   Pricing is not yet available.
*   **Notes:** Previously announced tiers (Free 50/Pro 1000/Pro+ 3000 interactions) were removed.

**Links:** [Introduction Blog](https://kiro.dev/blog/introducing-kiro/)
---


> Limits change fast. If you see a mistake, a newer quota/model, or want to add a new tool, open an issue or PR with a source. New tool contributions are welcomed!

---

## Tools with unclear free tier limits

---
### [Cursor](https://cursor.com/)

**Free Tier:**
*   **Pro-grade usage:** Unknown ("limited agent requests").
*   **Notes:** Provides access to multiple frontier models (e.g., Claude Sonnet/Opus, Gemini 2.5 Pro, GPT-4.x, o3).

**Paid Tiers:**
*   **Pro ($20/mo):** Extended agent limits.
*   **Ultra ($200/mo):** 20x usage of Pro.
*   **Teams ($40/user/mo):** Custom limits.

**Links:** [Pricing](https://cursor.com/en/pricing)
---

### [Lovable](https://lovable.dev/)

**Free Tier:**
*   **Pro-grade usage:** ~0.5h/month (est.)
*   **Notes:** Free plan provides 5 daily credits with a cap of 30 per month. Models used are not publicly enumerated.

**Paid Tiers:**
*   **Pro ($25/mo):** ~1.7h/month (est., 100 credits)
*   **Teams ($30/mo):** Higher limits.

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)
---

### [Bolt.new](https://bolt.new/)

**Free Tier:**
*   **Pro-grade usage:** ~100h/month (est., 1M tokens).
*   **Notes:** The specific model used in the free plan is not publicly specified.

**Paid Tiers:**
*   **$20/mo:** ~1000h/month (est., 10M tokens).
*   **$200/mo:** ~12000h/month (est., 120M tokens).

**Links:** [Token Documentation](https://support.bolt.new/account-and-subscription/tokens)
---

### [v0.dev](https://v0.dev/)

**Free Tier:**
*   **Usage:** $5 in credits per month.
*   **Notes:** Credit usage is model-dependent. v0 uses its own models with varied routing.

**Paid Tiers:**
*   **Premium ($20/mo):** Includes $20 in credits.
*   **Team ($30/user/mo):** Includes $30 in credits per user.

**Links:** [Updated Pricing Blog](https://vercel.com/blog/improved-v0-pricing-5luSrdRUJsRvf1kXWoYGxh)
---


> Know the official limits or models? Share a link in an issue or PR to update the table.

---

## Paid-only tools

---
### [Claude Code](https://www.anthropic.com/claude-code)

**Free Tier:**
*   None

**Paid Tiers:**
*   **Pro ($20/mo):** 40-80h/week of Claude Sonnet 4.
*   **Max ($100/mo):** 140-280h/week of Sonnet 4, plus 15-35h/week of Opus 4.
*   **Max ($200/mo):** 240-480h/week of Sonnet 4, plus 24-40h/week of Opus 4.
*   **Notes:** Usage limits are weekly and based on Anthropic's own hour estimations.

**Links:** [Pricing](https://www.anthropic.com/pricing)
---

### [GitHub Copilot](https://github.com/features/copilot/plans)

**Free Tier:**
*   None

**Paid Tiers:**
*   **Pro ($10/mo):** ~5h/month (est., 300 requests).
*   **Pro+ ($39/mo):** ~25h/month (est., 1500 requests).
*   **Business ($19/user/mo):** ~5h/user/month (est., 300 requests/user).
*   **Enterprise ($39/user/mo):** ~17h/user/month (est., 1000 requests/user).
*   **Notes:** Overage billing is available at $0.04/request.

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot)
---

