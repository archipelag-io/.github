<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://archipelag.io/img/archipelagio-brandmark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://archipelag.io/img/archipelagio-brandmark.png">
    <img alt="Archipelag.io" src="https://archipelag.io/img/archipelagio-brandmark.png" width="120" />
  </picture>
</p>

<h3 align="center">Distributed Compute, Locally Powered</h3>

<p align="center">
  A network where people who need compute get it from people who have it.<br/>
  Your neighbor's idle GPU, not a data center three time zones away.
</p>

<p align="center">
  <a href="https://archipelag.io">Website</a> &middot;
  <a href="https://app.archipelag.io">App</a> &middot;
  <a href="https://docs.archipelag.io">Docs</a> &middot;
  <a href="https://archipelag.io/blog">Blog</a> &middot;
  <a href="https://twitter.com/archipelagio">Twitter</a>
</p>

---

### What is Archipelag.io?

Archipelag.io connects people who need AI compute with people who have idle GPUs sitting around. Users submit inference jobs (LLM chat, image generation), the coordinator finds the nearest available host, dispatches the work, and streams results back. Hosts earn credits for their contributions.

The architecture is workload-agnostic, but we're starting with AI inference because that's where the pain is sharpest.

**Currently in [open beta](https://archipelag.io/blog/open-beta-announcement/) through June 2026.** All credits and earnings are virtual during the beta.

### Architecture

```
User (browser / SDK / API)
         │
         ▼
Coordinator (Elixir/Phoenix)
  Placement · Dispatch · Billing · Karma
         │
         ▼
    NATS JetStream
         │
         ▼
  Node Agent (Rust)
  Docker · WASM · GPU
         │
         ▼
  Workload Container
  vLLM · ComfyUI · llama.cpp
         │
         ▼
NATS → Coordinator → WebSocket → User
```

### Open Source Repositories

| Repo | Description |
|------|-------------|
| [`website`](https://github.com/archipelag-io/website) | Marketing site at [archipelag.io](https://archipelag.io) |
| [`archipelag-python`](https://github.com/archipelag-io/archipelag-python) | Official Python SDK |
| [`archipelag-js`](https://github.com/archipelag-io/archipelag-js) | JavaScript/TypeScript SDK with React hooks |

More repositories (coordinator, node agent, docs, workload containers, mobile agents) are private during the beta and will open up over time.

### Get involved

- **Use AI** on the platform: [app.archipelag.io](https://app.archipelag.io)
- **Host with your GPU**: grab the [node agent](https://github.com/archipelag-io/node-agent/releases)
- **Build on the API**: read the [docs](https://docs.archipelag.io)
- **Report bugs or ideas**: [open an issue](https://github.com/archipelag-io/website/issues) or email [hello@archipelag.io](mailto:hello@archipelag.io)

### Built with

Elixir &middot; Phoenix LiveView &middot; Rust &middot; NATS JetStream &middot; PostgreSQL &middot; Docker &middot; WASM &middot; Tailwind CSS

---

<p align="center">
  <sub>Named after an archipelago, a network of independent islands working together. Each host is an island, the coordinator is the current that connects them.</sub>
</p>
