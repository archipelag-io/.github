# Contributing to Archipelag.io

Thanks for your interest in contributing! Archipelag.io is currently in **open beta**, and we welcome contributions from the community.

## Ways to Contribute

- **Report bugs** — [Open an issue](https://github.com/archipelag-io/website/issues) on the relevant repository
- **Suggest features** — Use the feature request issue template
- **Improve documentation** — Fix typos, clarify explanations, add examples
- **Submit code** — Bug fixes, improvements, new features

## Getting Started

1. **Fork** the repository you want to contribute to
2. **Clone** your fork locally
3. **Create a branch** for your changes (`git checkout -b my-feature`)
4. **Make your changes** — follow the existing code style in the repo
5. **Test** your changes — run the test suite before submitting
6. **Commit** with a clear message (we prefer [Conventional Commits](https://www.conventionalcommits.org/))
7. **Push** to your fork and open a **Pull Request**

## Pull Request Guidelines

- Keep PRs focused — one feature or fix per PR
- Write a clear description of what changed and why
- Include a test plan (how to verify the changes work)
- Make sure CI passes before requesting review
- Be responsive to review feedback

## Development Setup

Each repository has its own setup instructions in its README. All repos use [mise](https://mise.jdx.dev/) as a task runner — check the `mise.toml` in each repo for available tasks.

## Code Style

Follow the conventions already established in each repository:

- **Elixir** — `mix format`, standard Elixir conventions
- **Rust** — `cargo fmt`, `clippy` with `-D warnings`
- **TypeScript** — ESLint + Prettier
- **Python** — ruff for linting and formatting

## Repository Visibility

Some repositories (coordinator, node agent, mobile agents, infrastructure) are private during the beta period. They will open up over time as the platform stabilizes.

## Code of Conduct

All contributors are expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before participating.

## Questions?

- Email: [hello@archipelag.io](mailto:hello@archipelag.io)
- Twitter: [@archipelagio](https://twitter.com/archipelagio)
- Website: [archipelag.io](https://archipelag.io)
