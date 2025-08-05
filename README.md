# List of agentic coding tools with free access to frontier models

> **TL;DR**: Compare agentic IDEs/CLIs by their free access to frontier models. Local models = unlimited free use, Gemini CLI = 3000 h/month, others have various limits.

Last verified: August 4, 2025 • PRs welcome • ⭐ Star if useful!

This list compares agentic coding systems (IDE and CLI) organized by their access to frontier models: free pro-grade access, paid pro-grade tiers, and basic model access.

---

## Methodology / assumptions

- Goal: compare agentic coding systems by their access to frontier models.
- Preset: 60 requests ≈ 1 AI-assisted coding hour (based on real-world task simulation).
- Token quotas: when vendors publish tokens (not requests), assume ~10k tokens ≈ 1 coding hour.
- If you spot an error or missing source link, please open an issue or a pull request.

---

## Local models (completely free)

Running open-weight frontier models locally provides unlimited coding assistance without API costs or usage limits. The best tools for local deployment include **[Cline](https://cline.bot/)** (VS Code extension with Plan/Act modes and MCP support), **[Aider](https://aider.chat/)** (command-line assistant with built-in Git integration), and **[Continue](https://www.continue.dev/)** (open-source VS Code extension supporting 200+ models). All work seamlessly with **[Ollama](https://ollama.com/)** to run frontier models like Qwen3-Coder, DeepSeek Coder V2, Codestral, and GLM-4.5.

**Note**: Frontier models require GPUs with substantial RAM/VRAM. See Simon Willison's article on [running GLM-4.5 AIR on his laptop to build Space Invaders](https://simonwillison.net/2025/Jul/29/space-invaders/) for a practical example.

---

## Free Access to Pro-Grade Models

### [Gemini CLI](https://github.com/google-gemini/gemini-cli)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 100 requests/day for Gemini 2.5 Pro
- **Estimate:** ~1.7h/day (~50h/month)
- **Fallback:** 1,500 requests/day for Gemini 2.5 Flash (~25h/day, ~750h/month)
- Terms apply when registered with individual Google account
- No credit card required

**Links:** [Rate Limits](https://ai.google.dev/gemini-api/docs/rate-limits) | [Pricing](https://ai.google.dev/gemini-api/docs/pricing)

---

### [Warp](https://warp.dev/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 150 requests/month
- **Estimate:** ~2.5h/month across Claude Sonnet 4, OpenAI o3, Gemini 2.5 Pro
- No credit card required

**Links:** [Pricing](https://www.warp.dev/pricing)

---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 50 agentic chats/month
- **Estimate:** ~0.8h/month of Claude Sonnet 4
- Perpetual free tier
- Credit card required

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)

---

### [Windsurf](https://windsurf.com/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 25 credits/month
- **Estimate:** ~0.4h/month across OpenAI, Anthropic, Google, xAI models
- Credit card required

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [AWS Kiro](https://kiro.dev/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** Daily limits (undisclosed)
- **Estimate:** Unknown
- Claude Sonnet 4 / 3.7 (preview period)
- No credit card required during preview

**Links:** [Introduction Blog](https://kiro.dev/blog/introducing-kiro/)

---

### [Cursor](https://cursor.com/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** "Limited agent requests" (undisclosed)
- **Estimate:** Unknown
- Access to Claude Sonnet/Opus, Gemini 2.5 Pro, GPT-4.x, o3
- Credit card required

**Links:** [Pricing](https://cursor.com/en/pricing)

---

> Limits change fast. If you see a mistake, a newer quota/model, or want to add a new tool, open an issue or PR with a source. New tool contributions are welcomed!

---

## Paid Tiers with Pro-Grade Models

### [Claude Code](https://www.anthropic.com/claude-code)

**Paid Access Only:**
- **Vendor limits:** 40-80h/week Sonnet 4 (Pro), 140-280h/week Sonnet 4 + 15-35h/week Opus 4 (Max $100), 240-480h/week Sonnet 4 + 24-40h/week Opus 4 (Max $200)
- **Pro ($20/mo):** 160-320h/month
- **Max ($100/mo):** 620-1,260h/month total
- **Max ($200/mo):** 1,056-2,208h/month total
- Usage limits reset weekly

**Links:** [Pricing](https://www.anthropic.com/pricing)

---

### [Warp](https://warp.dev/)

**Paid Tiers:**
- **Vendor limits:** 2,500 requests (Pro), 10,000 requests (Turbo), 50,000 requests (Lightspeed)
- **Pro ($15/mo):** ~42h/month
- **Turbo ($40/mo):** ~167h/month
- **Lightspeed ($200/mo):** ~833h/month
- Pay-as-you-go available for overages

**Links:** [Pricing](https://www.warp.dev/pricing)

---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**Paid Tiers:**
- **Vendor limits:** Unlimited chats
- **Pro ($19/mo):** Unlimited usage

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)

---

### [GitHub Copilot](https://github.com/features/copilot/plans)

**Paid Access Only:**
- **Vendor limits:** 300 requests (Pro/Business), 1,500 requests (Pro+), 1,000 requests (Enterprise)
- **Pro ($10/mo):** ~5h/month
- **Pro+ ($39/mo):** ~25h/month
- **Business ($19/user/mo):** ~5h/user/month
- **Enterprise ($39/user/mo):** ~17h/user/month
- Overage billing available at $0.04/request

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot)

---

### [Windsurf](https://windsurf.com/)

**Paid Tiers:**
- **Vendor limits:** 500 credits (Pro), higher limits (Teams/Enterprise)
- **Pro ($15/mo):** ~8.3h/month
- **Teams ($30/user/mo):** Higher limits (undisclosed)
- **Enterprise ($60+/user/mo):** Higher limits (undisclosed)

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [Lovable](https://lovable.dev/)

**Paid Tiers:**
- **Vendor limits:** 100 credits (Pro), higher limits (Teams)
- **Pro ($25/mo):** ~1.7h/month
- **Teams ($30/mo):** Higher limits (undisclosed)

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**Paid Tiers:**
- **Vendor limits:** 10M tokens ($20/mo), 120M tokens ($200/mo)
- **$20/mo:** ~1,000h/month
- **$200/mo:** ~12,000h/month

**Links:** [Token Documentation](https://support.bolt.new/account-and-subscription/tokens)

---

### [Cursor](https://cursor.com/)

**Paid Tiers:**
- **Vendor limits:** Extended agent limits (Pro), 20x usage of Pro (Ultra), custom limits (Teams)
- **Pro ($20/mo):** Unknown estimate
- **Ultra ($200/mo):** Unknown estimate
- **Teams ($40/user/mo):** Unknown estimate

**Links:** [Pricing](https://cursor.com/en/pricing)

---

> Know better pricing or limits? Share a link in an issue or PR to help keep this updated.

---

## Free Access to Basic Models

### [Lovable](https://lovable.dev/)

**Free Access to Unspecified Models:**
- **Vendor limit:** 5 credits/day, 30/month cap
- **Estimate:** ~0.5h/month
- Models not publicly enumerated
- Credit card required

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**Free Access to Unspecified Models:**
- **Vendor limit:** 1M tokens/month
- **Estimate:** ~100h/month
- Specific model not publicly specified
- Credit card required

**Links:** [Token Documentation](https://support.bolt.new/account-and-subscription/tokens)

---

### [v0.dev](https://v0.dev/)

**Free Access to Unspecified Models:**
- **Vendor limit:** $5 in credits/month
- **Estimate:** Varies by model routing
- Uses proprietary models with varied routing, not frontier models
- Credit card required

**Links:** [Updated Pricing Blog](https://vercel.com/blog/improved-v0-pricing-5luSrdRUJsRvf1kXWoYGxh)

---

> Know the official limits or models? Share a link in an issue or PR to update the information.

