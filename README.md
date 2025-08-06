**Last updated: August 6, 2025** • PRs/issues welcome

**Disclaimer:** No affiliation with any vendor. All trademarks belong to their owners. Information is for research; accuracy not guaranteed; limits/pricing change frequently.

# The "Free" in Agentic AI Coding: A Ranked Comparison of Pro-Grade LLM Access

## Intro

This document compares free tiers for agentic AI coding tools, **focusing on access to pro-grade LLMs (e.g., Claude Sonnet 4, Gemini 2.5 Pro, o3)**. While "free" means no monetary cost, this guide highlights the nuances of what's available, including details on vendor limits, estimated coding hours, and model flexibility. The list is for informational purposes, with community contributions encouraged for accuracy, and is ranked from most to least generous.

---

**1.** [Local Models](#local-models-completely-free) _(completely free)_  

**2.** [Free Access to Pro-Grade Models](#free-access-to-pro-grade-models) _(ordered from most generous to least)_

**3.** [Paid Pro-Grade Tiers](#paid-pro-grade-tiers) _(ordered by most hours of coding for the buck)_

**4.** [Free Basic Model Access](#free-access-to-basic-models) _(unspecified/basic models)_  

---

## 1. Local models (completely free)

Running open-weight frontier models locally provides unlimited coding assistance without API costs or usage limits. The best tools for local deployment include **[Cline](https://cline.bot/)** (VS Code extension with Plan/Act modes and MCP support), **[Aider](https://aider.chat/)** (command-line assistant with built-in Git integration), and **[Continue](https://www.continue.dev/)** (open-source VS Code extension supporting 200+ models). All work seamlessly with **[Ollama](https://ollama.com/)** to run frontier models like Devstral (24B parameters, optimized for agentic coding), Qwen3-Coder, DeepSeek Coder V2, Codestral, and GLM-4.5.

**Note**: Frontier models require GPUs with substantial RAM/VRAM. See Simon Willison's article on [running GLM-4.5 AIR on his laptop to build Space Invaders](https://simonwillison.net/2025/Jul/29/space-invaders/) for a practical example.

---

## 2. Free Access to Pro-Grade Models

### [Gemini CLI](https://github.com/google-gemini/gemini-cli)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 100 requests/day for Gemini 2.5 Pro
- **Estimate:** ~1.7h/day (~50h/month) [1]
- **Fallback:** 1,500 requests/day for Gemini 2.5 Flash (~25h/day, ~750h/month) [1]
- **Credit card:** Not required
- **Model flexibility:** Google models only
- **Quota exhaustion:** Switches to paid rates after free quota
- Terms apply when registered with individual Google account

**Links:** [Rate Limits](https://ai.google.dev/gemini-api/docs/rate-limits) | [Pricing](https://ai.google.dev/gemini-api/docs/pricing)

---

### [Warp](https://warp.dev/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 150 requests/month
- **Estimate:** ~2.5h/month across Claude Sonnet 4, OpenAI o3, Gemini 2.5 Pro [1]
- **Credit card:** Not specified
- **Model flexibility:** Multiple providers (Claude, OpenAI, Gemini)
- **Quota exhaustion:** Pay-as-you-go overages available
- No credit card required for basic signup

**Links:** [Pricing](https://www.warp.dev/pricing)

---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 50 agentic chats/month
- **Estimate:** ~0.8h/month of Claude Sonnet 4 [3]
- **Credit card:** Required
- **Model flexibility:** Latest Claude models (AWS-hosted)
- **Quota exhaustion:** Must upgrade to Pro for continued access
- **Note:** Each agentic chat is a multi-turn conversation with context preservation
- Perpetual free tier

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)

---

### [Windsurf](https://windsurf.com/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 25 credits/month
- **Estimate:** ~0.4h/month across OpenAI, Anthropic, Google, xAI models [3]
- **Credit card:** Required
- **Model flexibility:** Multiple providers (OpenAI, Claude, Gemini, xAI)
- **Quota exhaustion:** Can purchase add-on credits to continue
- **Note:** Each credit = one prompt interaction (regardless of AI actions taken)

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [AWS Kiro](https://kiro.dev/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** Daily limits (undisclosed)
- **Estimate:** Unknown
- **Credit card:** Not required (preview period)
- **Model flexibility:** Claude models only (AWS-hosted)
- **Quota exhaustion:** Unknown (preview period)
- Claude Sonnet 4 / 3.7 available during preview

**Links:** [Introduction Blog](https://kiro.dev/blog/introducing-kiro/)

---

### [GitHub Copilot](https://github.com/features/copilot/plans)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** 50 chats + 2,000 completions/month
- **Estimate:** ~0.8h/month of agent interactions [1]
- **Credit card:** Not required
- **Model flexibility:** Multiple providers (GPT-4o, Claude 3.5 Sonnet, Gemini 2.0 Flash)
- **Quota exhaustion:** Limited to basic features after quota
- **Models:** GPT-4o, Claude 3.5 Sonnet, Gemini 2.0 Flash
- **Note:** Agent Mode with autonomous multi-step coding, tool calling, iterative refinement

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot) | [Agent Mode](https://code.visualstudio.com/blogs/2025/02/24/introducing-copilot-agent-mode)

---

### [OpenAI Codex CLI](https://github.com/openai/codex)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** Free for all ChatGPT users with usage limits during peak times
- **Estimate:** Variable based on demand (Plus: $5 API credits, Pro: $50 API credits monthly)
- **Credit card:** Not required for basic access
- **Model flexibility:** OpenAI models only
- **Quota exhaustion:** Rate limiting during high demand, paid subscribers get priority
- **Models:** codex-1 (o3-optimized), codex-mini-latest
- **Note:** Autonomous multi-task execution in secure cloud sandboxes

**Links:** [GitHub Repo](https://github.com/openai/codex) | [Help Center](https://help.openai.com/en/articles/11381614-codex-cli-and-sign-in-with-chatgpt)

---

### [Cursor](https://cursor.com/)

**Free Access to Pro-Grade Models:**
- **Vendor limit:** "Limited agent requests" (undisclosed)
- **Estimate:** Unknown
- **Credit card:** Required
- **Model flexibility:** Multiple providers (Claude, OpenAI, Gemini)
- **Quota exhaustion:** Asked to upgrade or switch to unlimited model
- Access to Claude Sonnet/Opus, Gemini 2.5 Pro, GPT-4.x, o3

**Links:** [Pricing](https://cursor.com/en/pricing)

---

> Limits change fast. If you see a mistake, a newer quota/model, or want to add a new tool, open an issue or PR with a source. New tool contributions are welcomed!

---

## 3. Paid Tiers with Pro-Grade Models

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
- **Pro ($15/mo):** ~42h/month [1]
- **Turbo ($40/mo):** ~167h/month [1]
- **Lightspeed ($200/mo):** ~833h/month [1]
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
- **Pro ($10/mo):** ~5h/month [1]
- **Pro+ ($39/mo):** ~25h/month [1]
- **Business ($19/user/mo):** ~5h/user/month [1]
- **Enterprise ($39/user/mo):** ~17h/user/month [1]
- Overage billing available at $0.04/request

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot)

---

### [Windsurf](https://windsurf.com/)

**Paid Tiers:**
- **Vendor limits:** 500 credits (Pro), higher limits (Teams/Enterprise)
- **Pro ($15/mo):** ~8.3h/month [3]
- **Teams ($30/user/mo):** Higher limits (undisclosed)
- **Enterprise ($60+/user/mo):** Higher limits (undisclosed)

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [Lovable](https://lovable.dev/)

**Paid Tiers:**
- **Vendor limits:** 100 credits (Pro), higher limits (Teams)
- **Pro ($25/mo):** ~1.7h/month [3]
- **Teams ($30/mo):** Higher limits (undisclosed)

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**Paid Tiers:**
- **Vendor limits:** 10M tokens ($20/mo), 120M tokens ($200/mo)
- **$20/mo:** ~1,000h/month [2]
- **$200/mo:** ~12,000h/month [2]

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

## 4. Free Access to Basic Models

### [Lovable](https://lovable.dev/)

**Free Access to Unspecified Models:**
- **Vendor limit:** 5 credits/day, 30/month cap
- **Estimate:** ~0.5h/month [3]
- Models not publicly enumerated
- Credit card required

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**Free Access to Unspecified Models:**
- **Vendor limit:** 1M tokens/month
- **Estimate:** ~100h/month [2]
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

---

## Methodology / Assumptions

- **Goal**: Compare agentic coding systems by their access to frontier models.
- **[1] Requests to hours**: 60 requests ≈ 1 AI-assisted coding hour (based on real-world task simulation).
- **[2] Tokens to hours**: ~10k tokens ≈ 1 coding hour (when vendors publish tokens, not requests).
- **[3] Chats/Credits to hours**: Multi-turn agentic chats and prompt credits are assumed equivalent to single requests for estimation purposes.
- If you spot an error or missing source link, please open an issue or a pull request.

