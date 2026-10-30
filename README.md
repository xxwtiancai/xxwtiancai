<h1 align="center">Xiongwei Xiao</h1>

<p align="center">
  <strong>Building agent applications and the systems behind them.</strong>
</p>

<p align="center">
  <a href="#user-content-about">About</a> &nbsp;·&nbsp;
  <a href="#user-content-focus">Focus</a> &nbsp;·&nbsp;
  <a href="#user-content-open-source">Open source</a> &nbsp;·&nbsp;
  <a href="#user-content-projects">Projects</a> &nbsp;·&nbsp;
  <a href="#user-content-contact">Contact</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/xxwtiancai/xxwtiancai/main/assets/agent-harness-overview-v1.png" alt="Conceptual Agent Harness architecture showing the agent loop, model, context and memory, policy checks, tools and sandbox, observations, traces, and evaluation" width="900">
</p>

## About

I build **AI agent applications** and contribute to the systems behind them: **sandboxed execution**, agent SDKs, tool use, and context management. My open-source work includes improvements to credential handling in [OpenSandbox](https://github.com/opensandbox-group/OpenSandbox) and proposed sandbox workspace protections in [Google ADK](https://github.com/google/adk-python/pull/7700). I am interested in the engineering details that make agents dependable in real workflows.

My longer-term interest is in agents that can build on previous experience. I am exploring **agent memory** and **recursive self-improvement (RSI)**: how to preserve useful context, turn feedback into better behavior, and test whether an improvement holds up. Previously, I worked on video coding and visual computing.

## Focus

- **Agent applications** · Current work  
  Building useful workflows around models, tools, and actions.
- **Sandbox & execution** · Open-source work  
  Credential handling, workspace boundaries, and controlled agent execution.
- **Agent memory** · Exploring  
  What should agents remember, retrieve, and carry forward across tasks?
- **Recursive self-improvement** · Exploring  
  How can feedback improve an agent's harness, and how do we verify the gains?

## Open source

Selected contributions to the tools and infrastructure behind AI agents.

| Project | Contribution | Stars |
| :--- | :--- | ---: |
| **[Strands Agents Harness SDK](https://github.com/strands-agents/harness-sdk)** | Preserve structured output during history offloading.<br><sub>Merged · [#5429](https://github.com/strands-agents/harness-sdk/pull/5429)</sub> | [★ 8,998](https://github.com/strands-agents/harness-sdk/stargazers) |
| **[OpenSandbox](https://github.com/opensandbox-group/OpenSandbox)** | Harden C# and Kotlin SDK credential handling.<br><sub>Merged · [#2183](https://github.com/opensandbox-group/OpenSandbox/pull/2183) · [#2372](https://github.com/opensandbox-group/OpenSandbox/pull/2372) · [#2375](https://github.com/opensandbox-group/OpenSandbox/pull/2375)</sub> | [★ 16,278](https://github.com/opensandbox-group/OpenSandbox/stargazers) |
| **[MOMO CODE](https://github.com/momozi1996/momo-code)** | Keep graph execution slots busy as tasks finish.<br><sub>Merged · [#12](https://github.com/momozi1996/momo-code/pull/12)</sub> | [★ 1,107](https://github.com/momozi1996/momo-code/stargazers) |
| **[Google ADK](https://github.com/google/adk-python)** | Contain relative paths within sandbox workspaces.<br><sub>Open PR · [#7700](https://github.com/google/adk-python/pull/7700)</sub> | [★ 22,047](https://github.com/google/adk-python/stargazers) |
| **[OpenHands SDK](https://github.com/OpenHands/software-agent-sdk)** | Expose MCP resources and prompts in the SDK.<br><sub>Open PR · [#6196](https://github.com/OpenHands/software-agent-sdk/pull/6196)</sub> | [★ 1,322](https://github.com/OpenHands/software-agent-sdk/stargazers) |
| **[Qwen Code](https://github.com/QwenLM/qwen-code)** | Share compression cache for equivalent model selections.<br><sub>Open PR · [#15318](https://github.com/QwenLM/qwen-code/pull/15318)</sub> | [★ 28,821](https://github.com/QwenLM/qwen-code/stargazers) |

<sub>Repository stars and PR status checked on October 30, 2026.</sub>

[Browse my pull requests →](https://github.com/pulls?q=is%3Apr+author%3Axxwtiancai+-user%3Axxwtiancai)

## Projects

### [ActionAnything](https://github.com/xxwtiancai/action-anything)

An action execution layer for an agent harness: normalize and validate proposals, apply policy and required approval, execute permitted actions, and record redacted traces. Model calls and deployment isolation stay with the host application.

<p align="center">
  <img src="https://raw.githubusercontent.com/xxwtiancai/xxwtiancai/main/assets/actionanything-harness-v1.png" alt="ActionAnything: host application to normalization and validation, policy and approval, executor, and result; policy outcomes and execution feed a redacted trace" width="900">
</p>

[Code & documentation →](https://github.com/xxwtiancai/action-anything)

### [nanoRSI](https://github.com/xxwtiancai/nanoRSI)

An auditable loop for improving a harness around a frozen model. Candidate changes are proposed, probed, contrasted, and composed from execution evidence; scoring happens only after freeze.

<p align="center">
  <img src="https://raw.githubusercontent.com/xxwtiancai/xxwtiancai/main/assets/nanorsi-harness-v1.png" alt="nanoRSI: frozen model and editable harness; propose, probe, contrast, and compose during evolution; freeze before judging; evidence recorded in a ledger" width="900">
</p>

[Code & documentation →](https://github.com/xxwtiancai/nanoRSI)

## Contact

For conversations about agent applications, sandboxes, memory, or self-improvement:

[**xiongweixiao@foxmail.com**](mailto:xiongweixiao@foxmail.com) &nbsp;·&nbsp; [**xiongweixiaoxxw@gmail.com**](mailto:xiongweixiaoxxw@gmail.com)
