# Repository Guidelines

## Project Structure & Module Organization

This repository is a Czech Agent Skills catalog. Each skill lives directly at the repository root as `<slug>/SKILL.md`; do not add a `skills/` parent directory.

Core files:

- `README.md` - public Czech overview and skill list.
- `CONTRIBUTING.md` - Czech contribution guide surfaced by GitHub.
- `SECURITY.md` - security reporting guidance for public repository health.
- `docs/instalace.md` - Czech installation guide.
- `<slug>/SKILL.md` - one reusable agent skill.
- `LICENSE` - repository license.

Use lowercase ASCII slugs with hyphens and the `vf-` prefix, for example `vf-emailova-sekvence` or `vf-seo-audit`.

## Build, Test, and Development Commands

There is no build system. Use lightweight checks:

- `rg --files` - confirm the catalog shape.
- `git status --short` - review changed files.
- `skills-ref validate ./vf-copywriting` - validate one skill if `skills-ref` is installed.
- `markdownlint README.md CONTRIBUTING.md SECURITY.md AGENTS.md docs/instalace.md` - lint docs if available.

Do not add package managers or generated artifacts unless a future validation workflow requires them.

## Coding Style & Naming Conventions

Write public content and skill bodies in Czech. Keep contributor-only notes in English unless the surrounding file is Czech.

Each `SKILL.md` must contain valid YAML frontmatter with `name` and `description`. The `name` must exactly match the parent folder and include the `vf-` prefix. Descriptions should explain both what the skill does and when an agent should use it.

Keep instructions concise, practical, and useful for non-technical users. Prefer short workflows, concrete questions, and explicit output formats.

## Testing Guidelines

For every new or edited skill, manually check:

- folder name matches frontmatter `name`;
- description is specific enough for agent routing;
- Czech instructions do not rely on unavailable tools;
- examples do not invent customer quotes, references, or metrics.

If validation tooling is available, run it on every changed skill folder.

## Commit & Pull Request Guidelines

The history does not establish a detailed convention. Use clear imperative commits such as `Add Czech marketing skills` or `Update install guide`.

Pull requests should include a short summary, list changed skills, and mention manual validation performed. Link related issues when available.

For GitHub discoverability, keep `README.md` focused on what the project does, why it is useful, how to install it, and which search terms users might use to find it.

## Agent-Specific Instructions

Do not copy or directly translate third-party skill text. This catalog may use other repositories for topic inspiration, but the Czech instructions must be original. Avoid touching unrelated local files such as `.codex`.
