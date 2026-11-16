# Ryan Lee

TypeScript and Effect-TS engineer helping teams migrate production codebases to typed functional architecture and run coding agents behind deterministic CI gates, through [System F Software](https://systemfsoftware.com).

## Effect-TS & TypeScript

Open-source testing, compatibility, and runtime libraries under [`systemfsoftware`](https://github.com/systemfsoftware):

* [`stryker-js-effect`](https://github.com/systemfsoftware/stryker-js-effect): Mutation testing for Effect 4 using in-memory V8 instrumentation and isolated Vitest runners.
* [`api-extractor-effect`](https://github.com/systemfsoftware/api-extractor-effect): Effect-native API Extractor producing byte-identical `*.api.md` reports against `@microsoft/api-extractor`.
* [`effect-e2e`](https://github.com/systemfsoftware/effect-e2e): End-to-end testing framework and conformance suites for Effect applications.
* [`rx-effect`](https://github.com/systemfsoftware/rx-effect): Typed bridge from RxJS `Observable` to Effect `Stream` preserving backpressure and interruption semantics.
* [`effect-daemon`](https://github.com/systemfsoftware/effect-daemon): Process, socket, and cluster lifecycle specification and conformance suite for long-running Effect services.
* [`effect-microvm`](https://github.com/systemfsoftware/effect-microvm): MicroVM execution runner for isolating untrusted or stateful daemon workloads.

## Coding-Agent Guardrails

Reproducible agent workflows built on Nix, git worktrees, and structural static analysis:

* [`gritlint`](https://github.com/systemfsoftware/gritlint): Rust CLI built on GritQL (packaged as a Nix flake) that enforces architectural and AST lint rules in CI.
* [`comment-checker`](https://github.com/systemfsoftware/comment-checker): Tree-sitter hook across 37 languages that flags low-signal AI-generated comments before review.
* [`constitution`](https://github.com/systemfsoftware/constitution): Repository-level engineering rules (functional core / imperative shell, strict typing) enforced during agent runs.
* [`omp-claude-compat`](https://github.com/systemfsoftware/omp-claude-compat): Compatibility layer running Claude Code hooks and `CLAUDE.md` policies inside Oh My Pi.

**How diffs ship:** Agents work in isolated git worktrees with pinned Nix toolchains against an approved plan. Independent reviewers grade every diff, and deterministic AST/lint checks in CI hold final merge authority.

## Work With Me

Available through [System F Software](https://systemfsoftware.com) for Effect-TS migrations, codebase architecture, and CI-gated coding-agent setups.

* Web: [systemfsoftware.com](https://systemfsoftware.com)
* GitHub: [github.com/systemfsoftware](https://github.com/systemfsoftware)
* X: [@ryanleecode](https://x.com/ryanleecode)
