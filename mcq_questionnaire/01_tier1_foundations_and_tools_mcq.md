# Assessment Module 01: Tier 1 — AI Foundations & Tool Setup
## AI for Coders: Developer Competency Assessment (20 Questions | Weight: 25%)

> **Target Audience**: Software Developers working on Lending Products (LOS, LMS, Credit Services).  
> **Curriculum Covered**: Modules 1.1 through 1.6 of Track A (`_outputs/02_track_a_developers.md`).  
> **Core Focus**: How LLMs work under the hood, tokenization, context windows, GitHub Copilot (Agent, Ask, Plan modes), Claude Code CLI, Google Antigravity IDE, and prompt engineering for code.

---

### Question 1.1 (Module 1.1 — LLM Foundations & Transformers)
**Scenario**: A developer working on a loan EMI interest calculation module asks an AI coding assistant to generate a reducing-balance interest schedule. The developer notices that across identical prompts, the assistant occasionally outputs `double` primitives instead of `BigDecimal`, or calculates slight rounding differences in the final cents/paise.  
**Core Question**: Which architectural property of transformer-based LLMs explains why an AI assistant cannot be treated as a deterministic mathematical execution engine?
- **A)** Transformers rely on self-attention and probabilistic next-token sampling from a learned probability distribution, rather than executing internal symbolic arithmetic.
- **B)** Transformers evaluate all numbers using 16-bit floating-point weights, causing IEEE 754 precision loss during model compilation.
- **C)** Context windows automatically truncate floating-point mantissas exceeding 8 decimal places to optimize token usage.
- **D)** Modern foundation models lack causal attention masking when processing code, causing token leakage that distorts math operations.

---

### Question 1.2 (Module 1.1 — Tokenization & Embeddings)
**Scenario**: While refactoring a loan file ingestion parser, a developer notices that Copilot Chat generates very different code completions when an input string has extra spaces around custom delimiters (for example, `LOAN_ID:1001` vs `LOAN_ID : 1001`).  
**Core Question**: How does subword tokenization (such as Byte-Pair Encoding) directly cause this sensitivity?
- **A)** Changing spaces alters how the characters are grouped into subword tokens, changing the token sequence and embedding vectors fed into the model.
- **B)** Subword tokenizers automatically convert all text with spaces into 8-bit ASCII representations, discarding non-standard tokens.
- **C)** Byte-Pair Encoding encrypts strings with variable hashes based on whitespace, leading to semantic fragmentation.
- **D)** Any string containing spaces is automatically replaced with an unknown token `[UNK]`.

---

### Question 1.3 (Module 1.1 — Context Window Mechanics)
**Scenario**: A developer loads a 4,500-line monolithic loan processing file into an LLM chat window with a 128k token context window and asks: *"Find all concurrency race conditions in this file."* The LLM reports zero race conditions, missing an obvious multi-threaded synchronization flaw located around line 2,200.  
**Core Question**: What well-documented LLM phenomenon explains why the model missed this bug?
- **A)** Catastrophic forgetting caused by high temperature sampling in enterprise chat configurations.
- **B)** The "Lost in the Middle" phenomenon, where retrieval and reasoning accuracy are significantly higher at the beginning and end of the context window than in the middle.
- **C)** Context quantization degradation, where tokens in the middle 50% of the window are downscaled to 4-bit integers.
- **D)** Enterprise firewalls selectively redacting concurrency keywords from prompt payloads.

---

### Question 1.4 (Module 1.2 — AI Capabilities & Hallucinations)
**Scenario**: While integrating a loan service with an external credit bureau API, a developer prompts an AI assistant to write the authentication client. The AI generates code calling `CreditBureauClient.authenticateWithMutualTlsAndToken()`. During build, the compiler fails because no such method exists in the official SDK.  
**Core Question**: What has occurred, and what is the required developer practice?
- **A)** Model hallucination / confabulation; developers must always verify AI-generated library calls against authoritative API docs or SDK definitions.
- **B)** Model inversion attack; the developer should revoke all local API tokens and alert the security team.
- **C)** Token collision; the developer should increase model temperature to 1.0 to find the right method signature.
- **D)** Model context leakage; the AI assistant copied an internal method from another customer's repository.

---

### Question 1.5 (Module 1.2 — Non-Determinism in Code Generation)
**Scenario**: A developer prompts an AI assistant to generate unit tests for a credit eligibility evaluation function. Running the identical prompt twice produces two different sets of test cases, one of which misses a critical boundary test.  
**Core Question**: How should software developers incorporate non-deterministic AI code generators into their daily workflow?
- **A)** Re-run prompts multiple times and pick the longest output using a majority vote approach.
- **B)** Set temperature to 0.0 and assume the code is completely bug-free and deterministic.
- **C)** Treat AI generation as an initial drafting and scaffolding tool, relying on deterministic unit tests, linters, and peer review for verification.
- **D)** Avoid using AI for any testing or backend code, limiting its usage strictly to CSS and HTML templates.

---

### Question 1.6 (Module 1.2 — Source Code Privacy & Telemetry)
**Scenario**: A developer working on a proprietary credit scoring algorithm pastes the core scoring calculation into a public, consumer-facing browser AI chatbot to ask for algorithmic optimizations.  
**Core Question**: What technical and security risk does this action present?
- **A)** Public consumer chat models may retain prompt inputs for future model training and telemetry, leading to data egress and exposure of proprietary source code.
- **B)** The web browser compiler will automatically compile the code into WebAssembly and publish it publicly.
- **C)** Consumer LLMs strip SIMD vectorization from code, making the resulting logic permanently slower.
- **D)** It violates the open-source Apache 2.0 dual-license clause for web chats.

---

### Question 1.7 (Module 1.3 — GitHub Copilot: Agent Mode vs Ask Mode vs Plan Mode)
**Scenario**: A developer needs to refactor a loan service across five files: creating two new DTOs, modifying a repository layer, updating a service class, and writing two integration tests.  
**Core Question**: In GitHub Copilot, which interaction mode is designed to autonomously plan, navigate the workspace file tree, edit multiple files, and run terminal build commands?
- **A)** **Ask Mode**: Designed for conversational questions and answers about code without making edits.
- **B)** **Plan Mode**: Used solely to draft markdown project plans without workspace file access.
- **C)** **Agent Mode**: Uses autonomous tool-calling loops to inspect files, edit across the workspace, and run terminal checks.
- **D)** **Edit Mode**: Designed only for inline single-line tab autocomplete suggestions.

---

### Question 1.8 (Module 1.3 — GitHub Copilot: Custom Instruction Files)
**Scenario**: A team wants GitHub Copilot to consistently follow repository-wide coding conventions (e.g., use `BigDecimal` for monetary amounts, use constructor injection for Spring beans, and enforce standard exception classes).  
**Core Question**: Where should the team place these instructions so that Copilot Chat automatically includes them in every developer query in the repository?
- **A)** In an environment variable named `COPILOT_SYSTEM_PROMPT` on each local machine.
- **B)** In a file named `.github/copilot-instructions.md` at the root of the repository.
- **C)** In `~/.config/github/copilot.json` in the user's home directory.
- **D)** In a markdown comment at the top of the root `build.gradle` or `pom.xml` file.

---

### Question 1.9 (Module 1.3 — Model Context Protocol: MCP)
**Scenario**: A developer using an agentic coding assistant wants the assistant to query their local database schema and fetch live API contracts from an internal documentation server before generating repository code.  
**Core Question**: How does Model Context Protocol (MCP) enable this capability?
- **A)** It retrains the underlying LLM weights locally with the database schema every night.
- **B)** It provides an open, standardized client-server protocol allowing AI assistants to securely connect to external tools, databases, and context servers.
- **C)** It encrypts the developer's network connection via a VPN to bypass corporate firewalls.
- **D)** It converts relational databases into local vector embeddings stored on public GitHub servers.

---

### Question 1.10 (Module 1.3 — Public Code Matching Policy)
**Scenario**: An engineering lead is configuring organization-wide settings for GitHub Copilot. To avoid any risk of introducing code covered by restrictive open-source licenses (such as GPL copyleft), the lead configures the enterprise policy.  
**Core Question**: Which administrative setting in GitHub Copilot enforces this protection?
- **A)** Setting "Suggestions matching public code" to **Blocked**.
- **B)** Setting "Model Temperature" to `0.0` in the organization dashboard.
- **C)** Requiring GPG key signing on all Copilot chat messages.
- **D)** Forcing Copilot to run in an offline, air-gapped container on each developer's laptop.

---

### Question 1.11 (Module 1.4 — Claude Code CLI Architecture)
**Scenario**: A developer installs Anthropic's Claude Code CLI tool to work on a loan reconciliation service in their terminal.  
**Core Question**: What is the key architectural differentiator of Claude Code compared to traditional IDE autocomplete extensions?
- **A)** Claude Code only supports Python and cannot work with compiled languages like Java, Go, or C#.
- **B)** Claude Code is an agentic, terminal-native tool that directly reads project files, executes terminal commands, runs tests, inspects git diffs, and iterates autonomously.
- **C)** Claude Code runs a local quantized 7B model entirely on the developer's laptop CPU.
- **D)** Claude Code replaces the host operating system with an AI sandbox.

---

### Question 1.12 (Module 1.4 — CLAUDE.md Memory & Project Configuration)
**Scenario**: When running Claude Code in a project, a developer wants the CLI to always know the standard build commands (`./gradlew test`), coding style guidelines, and forbidden practices without repeating them in every prompt.  
**Core Question**: How should these project rules be configured for Claude Code?
- **A)** Create a `CLAUDE.md` file in the root of the project repository containing the commands and rules.
- **B)** Pass them as command-line flags on every run: `claude --build="./gradlew test"`.
- **C)** Upload them to the public Anthropic web console under "Custom GPTs".
- **D)** Set them in the global git configuration via `git config --global claude.rules`.

---

### Question 1.13 (Module 1.4 — Claude Code Permission Safety)
**Scenario**: While using Claude Code to clean up an old build script, the tool suggests running terminal commands like `rm -rf` and `git clean -fdx`.  
**Core Question**: Why is the `--dangerously-skip-permissions` flag considered high risk in developer environments?
- **A)** It slows down CLI processing by checking each command against an online CVE database.
- **B)** It bypasses the interactive confirmation prompt, granting the agent unmonitored capability to run destructive terminal commands or delete uncommitted files without human review.
- **C)** It reduces the context window from 200k to 8k tokens.
- **D)** It invalidates the commercial software license of the CLI tool.

---

### Question 1.14 (Module 1.5 — Google Antigravity IDE: Architecture & Model Selection)
**Scenario**: A developer begins using Google Antigravity IDE for daily coding tasks. A teammate asks whether Antigravity is just a wrapper around Claude that requires an Anthropic account.  
**Core Question**: Based on the Track A curriculum (Module 1.5), what is the correct architecture of Google Antigravity?
- **A)** It is an Anthropic-exclusive editor built solely to run Claude Code models.
- **B)** It is Google's agentic IDE designed to execute Google Gemini models alongside other foundation models, featuring native agentic workflows, artifacts, and workspace context integration without requiring a Claude subscription.
- **C)** It is a cloud-only terminal emulator built exclusively for mainframe languages.
- **D)** It is a command-line package manager for installing AI libraries.

---

### Question 1.15 (Module 1.5 — Antigravity IDE: Task Management)
**Scenario**: While working in Google Antigravity, a developer launches a long-running integration test suite in the background. The agent needs to inspect the test output once finished.  
**Core Question**: How does Antigravity's task execution model handle waiting for background tasks?
- **A)** The agent runs a tight CPU busy-waiting loop, calling `status` every 200 milliseconds until the process exits.
- **B)** The agent uses reactive event wakeups; background tasks notify the agent upon completion, avoiding wasteful CPU polling while preserving context.
- **C)** Antigravity automatically terminates any background task that takes longer than 5 seconds.
- **D)** Antigravity converts background tasks into cron jobs scheduled on the operating system.

---

### Question 1.16 (Module 1.5 — Antigravity Artifacts)
**Scenario**: A developer asks the agent in Google Antigravity to plan a complex refactoring of a payment routing module before touching any source code.  
**Core Question**: What mechanism in Google Antigravity allows the agent and developer to collaborate on structured, reviewable plans?
- **A)** Writing plans directly into the git commit message history.
- **B)** Creating interactive Markdown Artifacts in the brain directory, allowing the user to review, edit, and approve implementation plans before code edits are applied.
- **C)** Sending automated email summaries to the development team.
- **D)** Storing plans as compiled binary files in the `.git` directory.

---

### Question 1.17 (Module 1.6 — Prompt Engineering: Core Components for Code)
**Scenario**: A developer writes a vague prompt: *"Write a method to calculate loan interest."* The output lacks error handling, uses inappropriate variable types, and misses framework conventions.  
**Core Question**: According to the official prompt engineering guide (Module 1.6), what core elements should be included to get production-grade code?
- **A)** Persona/Role, Technical Context (framework & language version), Explicit Constraints (types, error handling, edge cases), and Desired Output Format.
- **B)** Only a request to "write clean and bug-free code" with multiple exclamation marks.
- **C)** Repeating the request in five different programming languages in the same prompt.
- **D)** Converting all method requirements into binary hexadecimal representations.

---

### Question 1.18 (Module 1.6 — Few-Shot Prompting for Specialized Formats)
**Scenario**: A developer needs an AI assistant to write a parser for an uncommon proprietary loan application text format with irregular column widths. Zero-shot prompting repeatedly results in hallucinated fields and incorrect parsing offsets.  
**Core Question**: What prompt engineering technique is best suited to teach the model this specific format?
- **A)** **Zero-shot prompting**: Removing all hints to prevent confusing the model's pre-trained weights.
- **B)** **Few-shot prompting**: Providing 2–3 concrete examples showing raw input text paired with the expected parsed output structure in the prompt.
- **C)** **Chain-of-thought compression**: Stripping all spaces and line breaks from the prompt.
- **D)** **Temperature maximization**: Setting temperature to 1.5 to increase output creativity.

---

### Question 1.19 (Module 1.6 — Negative Constraints vs Positive Instruction)
**Scenario**: A developer prompts an AI assistant: *"Do NOT use java.util.Date. Do NOT use Calendar. Do NOT use SimpleDateFormat."* Despite this, the AI still outputs code importing `java.util.Date`.  
**Core Question**: Why did the negative prompt fail, and how should it be corrected?
- **A)** LLMs have a hardcoded bias towards 1990s Java libraries that can never be overridden.
- **B)** Negative constraints often increase attention on the forbidden tokens; the recommended technique is **positive instruction** specifying the exact replacement to use (e.g., *"Use `java.time.LocalDate` and `DateTimeFormatter`"*).
- **C)** The prompt was missing quotation marks around the forbidden package names.
- **D)** Modern LLMs ignore all sentences containing negative words like "NOT" or "DON'T".

---

### Question 1.20 (Module 1.6 — Grounding Context with `#file` References)
**Scenario**: A developer is writing a new loan calculation service that depends on an existing `CreditScoringPolicy` class. When prompting Copilot Chat, the model invents a fake interface for the policy class.  
**Core Question**: What is the most effective way for the developer to provide the necessary context to Copilot Chat in VS Code?
- **A)** Open `CreditScoringPolicy.java` in an active editor tab or reference it directly in the chat prompt using `#file:CreditScoringPolicy.java`.
- **B)** Re-install the GitHub Copilot extension and restart the editor.
- **C)** Copy-paste the entire compiled `.class` binary bytecode file into the prompt.
- **D)** Push the code to a public repository so Copilot's base model can train on it.

---
*(End of Module 01 — Refer to Document 04 for Master Answer Key & Distractor Rationales)*
