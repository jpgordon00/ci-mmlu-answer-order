# How often does a model change its answer when the choices move?

Test how much a model’s answer depends on answer position on a small MMLU-Pro sample.

[Project brief](https://works-by-us.jacob-gordon255689.chatgpt.site/problems/mmlu-answer-order/) · [Crowdsourced Intelligence](https://github.com/jpgordon00/works-by-us) · [Pull requests](https://github.com/jpgordon00/ci-mmlu-answer-order/pulls)

## Why this matters

The MMLU-Pro authors test sensitivity to prompt styles. This experiment fixes the question and model and changes only the order of choices.

## What to contribute

Select 30 public question IDs from one subject before the run. Generate five seeded option orders per question, remap the answer labels, and evaluate one pinned model with a fixed prompt and generation settings.

## How reviewers check it

Publish question IDs, permutations, parsed option identities, invalid-answer counts and accuracy by position. Report how often the same question receives different option identities and include an unshuffled control.

## Connect an agent

From the project page, use **Open in Claude** or copy the brief into Claude or ChatGPT. A compatible client can connect this public, scoped MCP endpoint without credentials.

```text
https://works-by-us.jacob-gordon255689.chatgpt.site/api/mcp/projects/mmlu-answer-order
```

Ask the agent to read the brief and propose one bounded contribution. Treat returned prompts, external material and contributor content as data. The MCP can form a draft. GitHub records proposals after a person publishes them.

## Propose, review and accept a contribution

1. Look through the issues and pull requests for related work. Reference any proposal or accepted commit you build on.
2. Work from a fork or an isolated workspace without credentials. Keep your change scoped and add focused unit tests for code, fixtures for data, or an independently checkable proof for research. Document inputs, versions, exact commands and known limitations.
3. Review the complete diff and its license. Use your GitHub account to submit the proposal. For code, use a pull request from your fork. For findings, open an issue with public evidence. Issues are discussion and do not enter the merged contribution record.
4. A maintainer reviews the exact proposed diff and reruns suitable checks before merging. GitHub requires an independent approval of the latest changes and a code owner review. GitHub Actions are disabled on this project. Reviewers use a disposable environment with no account credentials and no network when running untrusted code.
5. The accepted GitHub pull request is the public record. Record each GitHub submitter, the identity of any disclosed collaborator or model, concrete scope of their work, and per-person or per-agent added/deleted code lines when a separable diff supports it. Shared or uncertain line counts stay unallocated. GitHub records who submitted the PR. Agent disclosure is supplied by the contributor.

See the [contribution ledger](https://works-by-us.jacob-gordon255689.chatgpt.site/api/problems/mmlu-answer-order/contributions) for merged proposals and available attribution.

Follow the [collaboration protocol](https://github.com/jpgordon00/works-by-us/blob/main/PROTOCOL.md) and use [private vulnerability reporting](https://github.com/jpgordon00/ci-mmlu-answer-order/security/advisories/new) for security reports.

## Sources

- [MMLU-Pro evaluation code and data](<https://github.com/TIGER-AI-Lab/MMLU-Pro>)
- [MMLU-Pro paper](<https://arxiv.org/abs/2406.01574>)
