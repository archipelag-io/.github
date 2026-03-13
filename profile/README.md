<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://archipelag.io/img/archipelagio-brandmark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://archipelag.io/img/archipelagio-brandmark.png">
  <img alt="Archipelag.io" src="https://archipelag.io/img/archipelagio-brandmark.png" width="64">
</picture>

## Archipelag.io

Distributed compute, locally powered.

Archipelag.io is a network that connects people who need compute with people who have it. Your neighbor's idle GPU can serve your AI requests with lower latency than a data center three time zones away. We built the plumbing to make that work.

**Currently in [open beta](https://archipelag.io/blog/open-beta-announcement/) through June 2026.**

### How it works

Users submit AI inference jobs (LLM chat, image generation). The coordinator finds the nearest available host, dispatches the job, and streams results back. Hosts earn credits for their contributions. The architecture is workload-agnostic, but we're starting with AI because that's where the pain is sharpest.

### Repositories

| Repo | What it does |
|------|-------------|
| [website](https://github.com/archipelag-io/website) | Marketing site at [archipelag.io](https://archipelag.io) |
| [archipelag-python](https://github.com/archipelag-io/archipelag-python) | Python SDK |
| [archipelag-js](https://github.com/archipelag-io/archipelag-js) | JavaScript/TypeScript SDK with React hooks |
| [mobile-agent-android](https://github.com/archipelag-io/mobile-agent-android) | Android host agent |

More repositories (coordinator, node agent, docs, iOS agent, workload containers) are private during the beta and will open up over time.

### Get involved

- **Use AI** on the platform: [app.archipelag.io](https://app.archipelag.io)
- **Host with your GPU**: grab the [node agent](https://github.com/archipelag-io/node-agent/releases)
- **Build on the API**: read the [docs](https://docs.archipelag.io)
- **Report bugs or ideas**: [open an issue](https://github.com/archipelag-io/website/issues) or email [hello@archipelag.io](mailto:hello@archipelag.io)

### Links

[Website](https://archipelag.io) · [Docs](https://docs.archipelag.io) · [Blog](https://archipelag.io/blog) · [Twitter](https://twitter.com/archipelagio)
