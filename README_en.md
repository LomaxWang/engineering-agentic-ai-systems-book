<p align="center">
  <font size="5"><strong>📖 Engineering Agentic AI Systems</strong></font><br>
  <em>From LLMs to Production-Grade Agents</em>
</p>

<p align="center">
  <a href="https://github.com/datascale-ai/engineering-agentic-ai-systems-book/actions/workflows/validate.yml"><img src="https://github.com/datascale-ai/engineering-agentic-ai-systems-book/actions/workflows/validate.yml/badge.svg" alt="Build status"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

**| [中文](README.md) | English |**

> **Read online:** <https://datascale-ai.github.io/engineering-agentic-ai-systems-book/>

## Overview

Large language models give software new ways to interact, but an agentic system that perceives its environment, calls tools, maintains state, verifies outcomes, and completes tasks is much more than a model API. This book follows the path from model interaction through planning, memory, collaboration, runtimes, evaluation, governance, and engineering practice to explain how to build reliable, observable, testable, and deployable agents for the real world.

The book is planned as a Springer Handbook for researchers, graduate students, AI engineers, system architects, and technical leaders. Its proposed outline covers Parts I–VIII and Chapters 1–35. The team manuscript scaffold also retains Part IX (Chapters 36–39) as an engineering-practice extension with a reference implementation, runnable code, testing, and deployment exercises. The public scaffold therefore contains nine parts and 39 chapters.

The book covers:

- 🧠 **Models and reasoning:** instruction hierarchies, context engineering, structured outputs, model selection, and reasoning contracts
- 🧩 **Core agent capabilities:** task decomposition, plan revision, tool discovery, action execution, trace verification, and recovery
- 🗂️ **Memory and knowledge:** working memory, long-term memory, personalization, retrieval augmentation, and knowledge-driven agents
- 🤝 **Multi-agent systems:** role design, communication, coordination, collective reasoning, negotiation, and environment interaction
- ⚙️ **Runtime infrastructure:** orchestration, sessions, events, state machines, streaming, multimodality, and real-time coordination
- 🛡️ **Evaluation and production governance:** benchmarks, capacity planning, reliability, security, alignment, monitoring, and governance
- 🏗️ **Applications and capstone projects:** software engineering, knowledge work, education, healthcare, finance, and enterprise adoption
- 🧪 **Runnable engineering practice:** reference implementations, reproducible environments, layered tests, regression evaluation, fault injection, and continuous delivery

## Book structure

The parts are organized around the dependencies involved in building agentic systems, from foundational capabilities to production deployment. Parts I–VIII and Chapters 1–35 follow the Springer proposal outline. Part IX is a team-retained engineering-practice extension that provides a runnable path from reference implementation and layered testing to continuous delivery.

![Book structure](docs/images/book-structure-zh.png)

*The complete path from model interaction, planning, and action to runtimes, governance, and runnable engineering practice.*

```text
Model interaction and reasoning
        ↓
Planning, tool use, and action verification
        ↓
Memory, knowledge, and multi-agent collaboration
        ↓
Runtimes, event streams, and multimodal interaction
        ↓
Evaluation, reliability, security, and production governance
        ↓
Application capstones and runnable engineering practice
```

Readers can follow the book sequentially or choose a path: the foundations establish shared concepts; the capability chapters explain how agents complete tasks; the systems chapters address operation at scale; and the engineering-practice chapters turn the concepts into code, tests, and deployment workflows.

## Table of contents

```text
📖 Nine parts, 39 chapters, and 8 appendices
│
├── Part I: Foundations of Agentic AI Systems (Chapters 1–4)
├── Part II: Model Interaction and Reasoning Foundations (Chapters 5–8)
├── Part III: Core Agent Capabilities (Chapters 9–13)
├── Part IV: Memory, Knowledge, and Agent Learning (Chapters 14–17)
├── Part V: Multi-Agent and Environment Interaction Systems (Chapters 18–21)
├── Part VI: Runtime Engineering and Interaction Infrastructure (Chapters 22–25)
├── Part VII: Evaluation, Trustworthiness, and Production Governance (Chapters 26–30)
├── Part VIII: Applications, Capstone Projects, and Future Directions (Chapters 31–35)
├── Part IX: Engineering Practice, Runnable Code, and Testing (Chapters 36–39)
└── Appendices A–H: terminology, metrics, interfaces, deployment, security, failures, and references
```

## Key features

### From model capability to system capability

The book treats model invocation as one component of an agentic system. It examines task boundaries, state management, tool permissions, execution traces, verification evidence, and human intervention. Each layer addresses its inputs and outputs, failure modes, design trade-offs, and observability signals.

### From a single agent to production systems

The material spans single-agent loops and multi-agent organizations, synchronous calls and streaming runtimes, and experimental demos and production systems with capacity planning, recovery, security auditing, and continuous delivery.

### From concepts to verifiable practice

Chapters use consistent elements such as cases, architecture diagrams, interface tables, experiment cards, review questions, and exercises. Part IX provides a reference implementation and testing path so readers can validate designs and feed results back into evaluation and governance.

### An engineering perspective throughout

| Theme | Questions addressed |
| --- | --- |
| Model interaction | How can model outputs be made stable, parseable, and routable? |
| Task execution | How can tasks be decomposed, tools called, and outcomes verified? |
| State and memory | How can useful information be retained within a limited context? |
| Multi-agent systems | How should roles, communication, coordination, and conflict be managed? |
| Runtimes | How should sessions, events, traffic, interruptions, and real-time behavior be handled? |
| Evaluation and governance | How can reliability, safety, observability, and accountability be demonstrated? |
| Engineering practice | How can environments be reproduced, tests written, failures injected, and delivery sustained? |

## Read online and preview locally

The book website is built with MkDocs Material and provides Chinese and English navigation. The published version is available on GitHub Pages:

**[Open the online book →](https://datascale-ai.github.io/engineering-agentic-ai-systems-book/)**

Local preview requires Python 3.11+ and uv:

```bash
uv sync --extra test
uv run mkdocs serve
```

Open the local URL printed in the terminal. Build the production site with strict checks:

```bash
uv run pytest
uv run mkdocs build --clean --strict
```

## Who this book is for

- Graduate students and researchers in agentic AI, LLMs, and applied AI
- AI application, platform, MLOps, and backend engineers
- Technical leaders responsible for architecture, reliability, security, and production governance
- Product managers and engineering managers who need to understand agent-system design trade-offs
- Instructors and organizations selecting a systems-focused textbook for courses or team training

## Contributing

Contributions to the manuscript, example code, and documentation site are welcome through Issues and Pull Requests.

1. Open an Issue to describe chapter suggestions, factual errors, broken links, or problems with engineering examples. Discuss major structural changes before implementing them.
2. Put Chinese manuscript content under `docs/zh/`, English translations under the corresponding paths in `docs/en/`, and runnable examples and engineering assets under `examples/`.
3. Cite the source, version, and license for figures, code, datasets, and external references. Do not submit third-party material without permission or local planning documents.
4. Before submitting, run `uv run pytest` and `uv run mkdocs build --clean --strict`. Describe the scope and verification results in the Pull Request.
5. Make the Pull Request title and description identify the affected part or chapter. Call out changes to navigation, shared interfaces, or figure numbering.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
