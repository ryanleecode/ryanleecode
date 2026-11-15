<div align="center">

# Ryan Lee

**Building autonomous software factories with TypeScript, Effect, and Rust — orchestrated on [Kiro Crew](https://kiro.dev/docs/crew).**

<p>
  <a href="https://readme-typing-svg.demolab.com">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=16&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=720&lines=Outer-loop+conductors+owning+requirements+and+plan+approval;Makers+shipping+in+isolated+worktrees+via+Claude+Code+%26+OMP;Report-only+P0-P3+reviewers+and+deterministic+CI+gates;Every+failure+compounded+into+a+durable+rule+or+skill" alt="Typing SVG" />
  </a>
</p>

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Effect-000000?style=for-the-badge&logo=effect&logoColor=white" alt="Effect" />
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/Bun-000000?style=for-the-badge&logo=bun&logoColor=white" alt="Bun" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Nix-5277C3?style=for-the-badge&logo=nixos&logoColor=white" alt="Nix" />
  <img src="https://img.shields.io/badge/Kiro_Crew-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="Kiro Crew" />
  <img src="https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code" />
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Cloudflare" />
</p>

</div>

---

## 🏭 The Software Factory

I design and run multi-agent software engineering pipelines at **[System F Software](https://github.com/systemfsoftware)**. Human attention stays focused on intent, taste, and release, while specialized coding agents handle planning, isolated implementation, adversarial review, and rule compounding.

```mermaid
flowchart LR
    Owner["Owner (intent, taste, release)"] --> Conductor["Conductor on Kiro Crew (requirements, plan approval)"]
    Conductor --> Plan["Committed Plan"]
    Plan --> Makers["Makers in Isolated Worktrees (Claude Code / OMP)"]
    Makers --> PR["Pull Request"]
    PR --> Reviewers["Independent Reviewers (report-only, P0-P3)"]
    Reviewers --> CI["CI Gate"]
    CI --> Merge["Merge"]
    Merge --> Compound["Compound Step (failure becomes a rule)"]
    Compound --> Conductor
```

---

## ⚙️ Running on Kiro Crew

The factory runs on **[Kiro Crew](https://kiro.dev/docs/crew)**, AWS's open-source personal agent platform, orchestrating **Claude Code** and **Oh My Pi (OMP)** coding agents as makers and reviewers:

- **Specialized Conductors:** Dedicated conductors per product area alongside isolated ledger and security conductors.
- **Editorial & Visual Loop:** A Gemini copy desk, a design critic, and a page judge reviewing copy and rendered interfaces before release.
- **Execution & Skill Density:** Isolated workers backed by ~68 skills on the main conductor.
- **Hard Guardrails & Recovery:** Gate hooks that refuse unsafe actions and auto-nudge patrol loops that keep stalled sessions moving.
- **Durable Memory & Deployment:** Lessons that turn corrections into permanent rules, all deployed reproducibly with Nix `home-manager` from a pinned Git ref.

---

## 📦 Built in the Open

Public libraries, developer tools, and conformance suites published under [`systemfsoftware`](https://github.com/systemfsoftware):

| Repository | Description | Stars |
| :--- | :--- | :---: |
| [`stryker-js-effect`](https://github.com/systemfsoftware/stryker-js-effect) | Effect 4 mutation testing with in-memory V8 instrumentation, Vitest runner sandboxes, and NDJSON event streams. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/stryker-js-effect?style=flat-square) |
| [`api-extractor-effect`](https://github.com/systemfsoftware/api-extractor-effect) | Effect-native API Extractor producing byte-identical `*.api.md` reports against `@microsoft/api-extractor`. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/api-extractor-effect?style=flat-square) |
| [`are-the-types-wrong-effect`](https://github.com/systemfsoftware/are-the-types-wrong-effect) | Effect-native package export and TypeScript module resolution analyzer. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/are-the-types-wrong-effect?style=flat-square) |
| [`effect-e2e`](https://github.com/systemfsoftware/effect-e2e) | Effect-native end-to-end testing across core, web engine, CLI, and engine conformance suites. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-e2e?style=flat-square) |
| [`effect-daemon`](https://github.com/systemfsoftware/effect-daemon) | Daemon specification and conformance suite supporting process, socket, and cluster media. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-daemon?style=flat-square) |
| [`effect-microvm`](https://github.com/systemfsoftware/effect-microvm) | Microsandbox binding and daemon microVM medium for isolated execution. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-microvm?style=flat-square) |
| [`effect-readiness`](https://github.com/systemfsoftware/effect-readiness) | Readiness cells and their deterministic conformance surface. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-readiness?style=flat-square) |
| [`gritlint`](https://github.com/systemfsoftware/gritlint) | Conventions gate implemented as a Rust CLI on the GritQL engine, packaged as a Nix flake. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/gritlint?style=flat-square) |
| [`comment-checker`](https://github.com/systemfsoftware/comment-checker) | Offline Claude Code hook flagging unnecessary comments and AI slop via Tree-sitter across 37 languages. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/comment-checker?style=flat-square) |
| [`omp-claude-compat`](https://github.com/systemfsoftware/omp-claude-compat) | Claude Code settings hooks and `CLAUDE.md` `@`-references running natively in Oh My Pi agents. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/omp-claude-compat?style=flat-square) |
| [`constitution`](https://github.com/systemfsoftware/constitution) | Engineering constitution (functional core / imperative shell, types-first, mutation-tested) vendored across repos and enforced by AI coding agents. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/constitution?style=flat-square) |
| [`hex-schema`](https://github.com/systemfsoftware/hex-schema) | Hex-encoded byte schemas built for Effect Schema. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/hex-schema?style=flat-square) |
| [`rx-effect`](https://github.com/systemfsoftware/rx-effect) | RxJS `Observable` to typed Effect `Stream` bridge with backpressure and interruption semantics. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/rx-effect?style=flat-square) |
| [`effect-memfs`](https://github.com/systemfsoftware/effect-memfs) | In-memory filesystem implementation for Effect (fork of [`nounder/effect-memfs`](https://github.com/nounder/effect-memfs)). | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-memfs?style=flat-square) |
| [`discern`](https://github.com/systemfsoftware/discern) | Static analysis and code inspection tooling (fork of [`doeixd/discern`](https://github.com/doeixd/discern)). | ![Stars](https://img.shields.io/github/stars/systemfsoftware/discern?style=flat-square) |
| [`effect-endgame-starter-kit`](https://github.com/systemfsoftware/effect-endgame-starter-kit) | Opinionated project template pre-wired with Effect, strict typing, mutation testing, and agent guardrails. | ![Stars](https://img.shields.io/github/stars/systemfsoftware/effect-endgame-starter-kit?style=flat-square) |

---

## 🧠 How I Build

- **Plan before code:** An outer-loop conductor owns requirements and approves a committed plan in the repository before a single line of implementation is written.
- **Inspect the state, never the transcript:** Automated checks read only the produced repository state and artifacts, never how an agent arrived there.
- **Reviewers report, CI decides:** Independent reviewers audit the exact PR head in report-only mode (`P0`–`P3`), while deterministic CI remains the sole merge gate.
- **Taste belongs in review:** Aesthetic, architectural, and API design calls go to human or critic review, never to brittle lint rules.
- **State lives in Git and the issue tracker:** Ephemeral chat context is disposable; durable memory lives in committed plans, rules, and issues.
- **Done means verified in production:** A task is complete only after it is deployed and checked against the real system.

---

## 📰 Newsletter

Get the long-horizon prompt to build your own software factory at **[systemfsoftware.com](https://systemfsoftware.com)**.

---

## 🎮 Fun Fact

Ranked **Top 50 Grandmaster** in *StarCraft II* during the *Heart of the Swarm* era.

---

## 📡 Connect

<p>
  <a href="https://systemfsoftware.com">
    <img src="https://img.shields.io/badge/systemfsoftware.com-0F172A?style=for-the-badge&logo=safari&logoColor=white" alt="Website" />
  </a>
  <a href="https://x.com/ryanleecode">
    <img src="https://img.shields.io/badge/@ryanleecode-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" />
  </a>
  <a href="https://www.linkedin.com/in/drd">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:ryanleecode@gmail.com">
    <img src="https://img.shields.io/badge/ryanleecode@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>
