Last updated: August 7, 2025 • PRs/issues welcome • ⭐ Star to come back later

## UPD August 7: Current list of AI tools providing access to the GPT-5 models family:
- [Cursor](https://cursor.com/) — GPT-5 offered with free credits for paying users during launch week

The list is being updating... 
Please submit an issue or PR if you know of others.

# How much free‑tier access do AI coding tools provide to pro‑grade LLMs (e.g., GPT‑5, Claude Sonnet 4, Gemini 2.5 Pro)

## Intro

Many tools advertise “free” AI coding, but most only let you use the top “frontier” or “pro-grade” models for a short time before switching you to more basic ones. Because each tool describes its limits differently (requests, credits, tokens), it’s tricky to compare which is actually the most generous.

This list compares those free tiers, ranks them from most to least generous, and includes links to the vendor docs so you can check the fine print yourself.

---

**1.** [Free Access to Pro-Grade Models](#free-access-to-pro-grade-models) _(ordered from most generous to least)_

**2.** [Paid Pro-Grade Tiers](#paid-pro-grade-tiers) _(ordered by most hours of coding for the buck)_

**3.** [Free Basic Model Access](#free-access-to-basic-models) _(unspecified/basic models)_

**4.** [Local Models](#local-models) _(free inference, requires GPU investment)_  

---

## 1. Free Access to Pro-Grade Models

### [Gemini CLI](https://github.com/google-gemini/gemini-cli)

**~1.7h/day (~50h/month) of Gemini 2.5 Pro coding**
- 100 requests/day limit
- Fallback: ~25h/day with Gemini 2.5 Flash (1,500 requests/day)
- No credit card required
- Google models only
- Switches to paid rates after free quota

**Links:** [Rate Limits](https://ai.google.dev/gemini-api/docs/rate-limits) | [Pricing](https://ai.google.dev/gemini-api/docs/pricing)

---

### [Cerebras](https://cloud.cerebras.ai/)

**~1.7h/day (~50h/month) of Qwen3-Coder/Llama 3.1 coding**
- 100 requests/day free tier
- Models: Qwen3-Coder-480B (matches Claude Sonnet 4 performance), Llama 3.1 70B, Qwen3-32B, Qwen3-235B
- OpenAI-compatible API (works with Cursor, Continue.dev, Cline, etc.)
- Ultra-fast inference: 2,000 tokens/second (40x faster than typical providers)
- No credit card required
- Note: Cerebras provides API access only, not software - integrate with existing IDEs/CLIs

**Links:** [Pricing](https://www.cerebras.ai/pricing) | [API Docs](https://inference-docs.cerebras.ai/) | [Cline Integration](https://inference-docs.cerebras.ai/integrations/cline)

---

### [Warp](https://warp.dev/)

**~2.5h/month across Claude Sonnet 4, OpenAI GPT-5, Gemini 2.5 Pro**
- 150 requests/month limit
- Multiple providers (Claude, OpenAI, Gemini)
- No credit card required for basic signup
- Pay-as-you-go overages available

**Links:** [Pricing](https://www.warp.dev/pricing)

---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**~0.8h/month of Claude Sonnet 4 coding**
- 50 agentic chats/month limit (multi-turn conversations)
- Latest Claude models (AWS-hosted)
- Credit card required
- Must upgrade to Pro for continued access
- Perpetual free tier

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)

---

### [Windsurf](https://windsurf.com/)

**~0.4h/month across OpenAI, Anthropic, Google, xAI models**
- 25 credits/month limit (each credit = one prompt interaction)
- Multiple providers (OpenAI, Claude, Gemini, xAI)
- Credit card required
- Can purchase add-on credits to continue

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [GitHub Copilot](https://github.com/features/copilot/plans)

**~0.8h/month of agent interactions (GPT-4o, Claude 3.5 Sonnet, Gemini 2.0 Flash)**
- 50 chats + 2,000 completions/month limit
- Agent Mode with autonomous multi-step coding
- Multiple providers (GPT-4o, Claude 3.5 Sonnet, Gemini 2.0 Flash)
- No credit card required
- Limited to basic features after quota

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot) | [Agent Mode](https://code.visualstudio.com/blogs/2025/02/24/introducing-copilot-agent-mode)

---

### [Cursor](https://cursor.com/)

**Unknown duration with basic models**
- **GPT-5 offered with free credits for paying users during launch week**
- "Limited agent requests" (undisclosed)
- Multiple providers (OpenAI, Claude, Gemini)
- Credit card required
- Asked to upgrade or switch to unlimited model after quota

**Links:** [Pricing](https://cursor.com/en/pricing)

---

### [OpenAI Codex CLI](https://github.com/openai/codex)

**Variable duration based on demand (codex-1, codex-mini-latest)**
- Free for all ChatGPT users with peak-time limits
- Autonomous multi-task execution in secure cloud sandboxes
- OpenAI models only
- No credit card required for basic access
- Rate limiting during high demand, paid subscribers get priority

**Links:** [GitHub Repo](https://github.com/openai/codex) | [Help Center](https://help.openai.com/en/articles/11381614-codex-cli-and-sign-in-with-chatgpt)

---


---

### [AWS Kiro](https://kiro.dev/)

**Unknown duration of Claude Sonnet 4 / 3.7 coding**
- Daily limits (undisclosed)
- Claude models only (AWS-hosted)
- No credit card required (preview period)
- Quota exhaustion unknown (preview period)

**Links:** [Introduction Blog](https://kiro.dev/blog/introducing-kiro/)

---

> Limits change fast. If you see a mistake, a newer quota/model, or want to add a new tool, open an issue or PR with a source. New tool contributions are welcomed!

---

## 2. Paid Tiers with Pro-Grade Models

### [Claude Code](https://www.anthropic.com/claude-code)

**Pro ($20/mo):** 160-320h/month Sonnet 4
**Max ($100/mo):** 620-1,260h/month (Sonnet 4 + Opus 4)
**Max ($200/mo):** 1,056-2,208h/month (Sonnet 4 + Opus 4)
- Usage limits reset weekly

**Links:** [Pricing](https://www.anthropic.com/pricing)

---

### [Warp](https://warp.dev/)

**Pro ($15/mo):** ~42h/month
**Turbo ($40/mo):** ~167h/month
**Lightspeed ($200/mo):** ~833h/month
- Pay-as-you-go available for overages

**Links:** [Pricing](https://www.warp.dev/pricing)

---

### [Amazon Q Developer](https://aws.amazon.com/q/developer/)

**Pro ($19/mo):** Unlimited usage

**Links:** [Pricing](https://aws.amazon.com/q/developer/pricing/)

---

### [GitHub Copilot](https://github.com/features/copilot/plans)

**Pro ($10/mo):** ~5h/month
**Pro+ ($39/mo):** ~25h/month
**Business ($19/user/mo):** ~5h/user/month
**Enterprise ($39/user/mo):** ~17h/user/month
- Overage billing available at $0.04/request

**Links:** [Plans Details](https://docs.github.com/en/copilot/get-started/plans-for-github-copilot)

---

### [Windsurf](https://windsurf.com/)

**Pro ($15/mo):** ~8.3h/month
**Teams ($30/user/mo):** Higher limits (undisclosed)
**Enterprise ($60+/user/mo):** Higher limits (undisclosed)

**Links:** [Pricing](https://windsurf.com/pricing)

---

### [Cerebras](https://cloud.cerebras.ai/)

**Code Pro ($50/mo):** ~800h/month of Qwen3-Coder at 2,000 tokens/sec
**Code Max ($200/mo):** Unlimited usage for heavy workflows
- 24M tokens/day on Pro tier
- Models: Qwen3-Coder-480B (SOTA open-source), Llama 3.1 70B
- OpenAI-compatible API for all major IDEs
- Custom ASIC hardware (not GPU) for ultra-fast inference

**Links:** [Pricing](https://www.cerebras.ai/pricing) | [Blog](https://www.cerebras.ai/blog/introducing-cerebras-code)

---

### [Lovable](https://lovable.dev/)

**Pro ($25/mo):** ~1.7h/month
**Teams ($30/mo):** Higher limits (undisclosed)

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**$20/mo:** ~1,000h/month
**$200/mo:** ~12,000h/month

**Links:** [Token Documentation](https://support.bolt.new/account-and-subscription/tokens)

---

### [Cursor](https://cursor.com/)

**GPT-5 offered with free credits for paying users during launch week**


**Pro ($20/mo):** Unknown estimate
**Ultra ($200/mo):** Unknown estimate
**Teams ($40/user/mo):** Unknown estimate

**Links:** [Pricing](https://cursor.com/en/pricing)

---

> Know better pricing or limits? Share a link in an issue or PR to help keep this updated.

---

## 3. Free Access to Basic Models

### [Lovable](https://lovable.dev/)

**~0.5h/month with unspecified models**
- 5 credits/day, 30/month cap
- Models not publicly enumerated
- Credit card required

**Links:** [Messaging Limits](https://docs.lovable.dev/user-guides/messaging-limits)

---

### [Bolt.new](https://bolt.new/)

**~100h/month with unspecified models**
- 1M tokens/month limit
- Specific model not publicly specified
- Credit card required

**Links:** [Token Documentation](https://support.bolt.new/account-and-subscription/tokens)

---

### [v0.dev](https://v0.dev/)

**Variable duration with proprietary models (not frontier)**
- $5 in credits/month limit
- Uses proprietary models with varied routing
- Credit card required

**Links:** [Updated Pricing Blog](https://vercel.com/blog/improved-v0-pricing-5luSrdRUJsRvf1kXWoYGxh)

---

> Know the official limits or models? Share a link in an issue or PR to update the information.

---

## 4. Local Models

Running open-weight frontier models locally provides unlimited coding assistance without API costs or usage limits. Popular tools for local deployment include **[Cline](https://cline.bot/)** (VS Code extension with Plan/Act modes and MCP support), **[Aider](https://aider.chat/)** (command-line assistant with built-in Git integration), and **[Continue](https://www.continue.dev/)** (open-source VS Code extension supporting 200+ models). All work seamlessly with **[Ollama](https://ollama.com/)** to run frontier models like Devstral (24B parameters, optimized for agentic coding), Qwen3-Coder, DeepSeek Coder V2, Codestral, and GLM-4.5.

**Note**: Frontier models require GPUs with substantial RAM/VRAM. See Simon Willison's article on [running GLM-4.5 AIR on his laptop to build Space Invaders](https://simonwillison.net/2025/Jul/29/space-invaders/) for a practical example.

---

## Methodology / Assumptions

- **Goal**: Compare agentic coding systems by their access to frontier models.
- **What qualifies a model as "pro-grade"?** For this comparison, models must achieve ≥60% on SWE-bench Verified, demonstrating real-world software engineering capability. Current qualifying models: GPT-5 (74.9%), Claude Opus 4.1 (74.5%), Claude Sonnet 4 (72.7%), GPT-5 mini (71.0%), Qwen3-Coder-480B (69.6%), and Gemini 2.5 Pro (63.2%).
- **[1] Requests to hours**: 60 requests ≈ 1 AI-assisted coding hour (based on real-world task simulation).
- **[2] Tokens to hours**: ~10k tokens ≈ 1 coding hour (when vendors publish tokens, not requests).
- **[3] Chats/Credits to hours**: Multi-turn agentic chats and prompt credits are assumed equivalent to single requests for estimation purposes.
- If you spot an error or missing source link, please open an issue or a pull request.

---

## Pro-Grade Models Benchmark Comparison

Only models achieving >60% on SWE-bench Verified qualify as pro-grade for real-world coding tasks.

| Model | Provider | SWE-bench Verified | Context Window | Notes |
|-------|----------|-------------------|----------------|-------|
| GPT-5 | OpenAI | 74.9% | 256K | Adaptive reasoning system, 6x fewer hallucinations than o3 |
| Claude Opus 4.1 | Anthropic | 74.5% | 200K (64K thinking) | Extended thinking capability, multi-file refactoring |
| Claude Sonnet 4 | Anthropic | 72.7% (80.2% w/ parallel) | 200K | Best performance with test-time compute |
| GPT-5 mini | OpenAI | 71.0% | 256K | Cost-effective variant of GPT-5 |
| Qwen3-Coder-480B | Alibaba | 69.6% (interactive) / 67.0% (single) | 256K native / 1M extended | Best open-source, matches Claude Sonnet 4 |
| Gemini 2.5 Pro | Google | 63.2% | 2M | Excellent multi-language support, largest context window |

---

**Disclaimer:** No affiliation with any vendor. All trademarks belong to their owners. Information is for research; accuracy not guaranteed; limits/pricing change frequently.

