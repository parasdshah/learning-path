# Assessment Module 01: Tier 1 — AI Foundations & Tool Setup
## Enterprise India Lending Developer Evaluation (20 Questions | Weight: 25%)

> **Scope**: Covers Modules 1.1 through 1.6 of Track A. Focuses on LLM probabilistic architectures, code generation risk boundaries, GitHub Copilot (Agent, Plan, Ask modes), Claude Code CLI, Google Antigravity IDE, and tool-level prompt engineering in Indian Lending Platforms (Loan Origination Systems [LOS], India Stack Integrations, CIBIL/Experian Bureau Parsing, and Credit Decisioning).

---

### Question 1.1 (Module 1.1 — LLM Foundations & Transformers)
**Indian Lending Context**: A software engineer is implementing an Equated Monthly Installment (EMI) calculation engine and Annual Percentage Rate (APR) disclosure generator for an unsecured personal loan product adhering to the **RBI Digital Lending Guidelines (DLG)** and mandatory **Key Fact Statement (KFS)** disclosures. When prompting an LLM assistant to generate the monthly reducing balance interest accrual algorithm in Indian Rupees (INR) across a 60-month loan tenure, the LLM occasionally emits `double` or `float` primitive types instead of `BigDecimal`, or introduces slight discrepancies in fractional paise rounding.  
**Core Question**: Which architectural reality of transformer-based LLMs explains why an AI assistant cannot be treated as a deterministic mathematical execution engine for Indian loan servicing?
- **A)** Transformers rely on self-attention mechanisms and probabilistic next-token generation calculated via softmax temperature distributions over token vocabularies, rather than executing internal symbolic arithmetic.
- **B)** Transformers store numbers in 16-bit floating-point (FP16) tensor weights, causing IEEE 754 precision loss during internal Python runtime calculations before text generation occurs.
- **C)** The LLM's context window automatically truncates floating-point mantissas exceeding 8 decimal places to conserve memory in enterprise cloud endpoints.
- **D)** Modern foundation models lack causal attention masking when processing programming languages, causing forward-looking token leakage that skews numerical outputs.

---

### Question 1.2 (Module 1.1 — Embeddings & Tokenization)
**Indian Lending Context**: A developer asks Copilot Chat to refactor an Indian credit bureau integration service that parses raw **TransUnion CIBIL** and **Experian India** Credit Information Reports (CIR). The parser processes specialized segment delimiters such as `T001` (Header), `ID01` (Income Tax PAN), `PT01` (Phone), and `TR01` (Trade-line with 36-month DPD strings like `000000030060XXX`). The developer observes that subtle changes in spacing or punctuation around segment tags result in wildly inconsistent parsing code completions.  
**Core Question**: How does subword tokenization (e.g., Byte-Pair Encoding) directly influence this behavior?
- **A)** The tokenizer encrypts CIBIL tags using SHA-256 hashes to prevent borrower privacy leaks, causing semantic fragmentation.
- **B)** Non-standard punctuation and alphanumeric strings like `TR01` or `ID01` are split into disparate, fragmented subword tokens depending on spacing, altering the embedding vectors passed to attention heads.
- **C)** Byte-Pair Encoding converts all characters into 8-bit ASCII representations, stripping specialized bureau delimiters from the model's receptive field.
- **D)** Indian credit tags exceed the maximum vocabulary size of 32,000 tokens, forcing the model to substitute unknown `[UNK]` tokens for critical bureau identifiers.

---

### Question 1.3 (Module 1.1 — Context Window Mechanics)
**Indian Lending Context**: While modernizing a 4,500-line monolithic Loan Origination System (LOS) orchestrator in a single source file, a developer loads the full file into an LLM chat window with a 128k token context window and asks: *"Identify all concurrency bugs and race conditions in the PAN de-duplication, credit limit allocation, and underwriting decision flow."* The LLM confidently reports zero bugs, completely overlooking a critical thread synchronization flaw sitting at line 2,240 where borrower Fixed Obligation to Income Ratio (**FOIR**) calculations overwrite shared state during simultaneous loan applications.  
**Core Question**: Which well-documented LLM phenomenon explains why the model overlooked this vulnerability?
- **A)** Catastrophic forgetting caused by high temperature sampling in enterprise chat configurations.
- **B)** The "Lost in the Middle" phenomenon, where transformer retrieval and attention accuracy degrade significantly for information positioned in the middle third of extensive context windows.
- **C)** Context quantization degradation, where tokens between 30% and 70% of the window are converted to 4-bit integers, corrupting AST parsing.
- **D)** The enterprise security firewall actively redacts multi-threaded concurrency primitives before prompting the external API.

---

### Question 1.4 (Module 1.2 — Capabilities, Limitations & Risk)
**Indian Lending Context**: An engineer is integrating an automated underwriting engine with a Credit Information Company (CIC) API (e.g., TransUnion CIBIL or Experian India). The engineer prompts an AI coding tool to write the bureau pull client. The AI generates code invoking a method `CibilConsumerClient.fetchScoreWithAadhaarXmlAndOtp()` from an official-looking SDK package. During build execution, the build fails because this method does not exist in the official CIBIL vendor SDK.  
**Core Question**: What risk phenomenon has occurred, and what is the required enterprise protocol?
- **A)** Model hallucination / confabulation; developers must verify all third-party API contracts against authoritative vendor specifications rather than assuming AI synthetic accuracy.
- **B)** Model inversion attack; the developer must revoke corporate OAuth credentials immediately and file an incident with CERT-In.
- **C)** Token collision; the developer should increase model temperature to 1.0 to force the model to explore alternate SDK signatures.
- **D)** Model context leakage; the AI provider accessed a competitor NBFC's proprietary SDK and leaked it across tenant boundaries.

---

### Question 1.5 (Module 1.2 — Non-Determinism in Financial Logic)
**Indian Lending Context**: A credit risk engineering team uses an AI code generator to write test cases for automated credit decisioning rules (evaluating CIBIL score cutoffs $\ge 750$, FOIR $\le 50\%$, and zero 90+ DPD write-offs in the last 24 months). Running the test generation prompt twice yields two completely different sets of edge cases—one omitting mandatory rejection logging required under RBI Fair Practices Code.  
**Core Question**: When utilizing AI tools for compliance-mandated Indian lending software development, how must engineering teams address model non-determinism?
- **A)** Re-run the prompt five times and take a majority voting consensus of the generated code snippets.
- **B)** Hardcode the LLM temperature to 0.0 in production IDEs and consider AI output as fully deterministic and self-verifying.
- **C)** Treat AI code generation strictly as a non-deterministic brainstorming/scaffolding aid, mandating deterministic verification through formal test specifications, static analysis, and SME peer review.
- **D)** Restrict AI code generation to borrower-facing mobile UI widgets and forbid its use on any credit policy or underwriting test code.

---

### Question 1.6 (Module 1.2 — Intellectual Property & Data Contamination)
**Indian Lending Context**: A quantitative developer working on a proprietary machine learning credit scorecard (predicting default probabilities for new-to-credit [NTC] borrowers using alternative device telemetry and utility payments) pastes proprietary feature engineering logic and risk weighting coefficients into a public consumer web chat AI tool to optimize execution performance.  
**Core Question**: Which enterprise policy and technical violation occurred under Indian lending regulatory standards?
- **A)** Violation of the Apache 2.0 dual-licensing requirement for algorithmic lending code.
- **B)** Data egress and intellectual property contamination violation; unapproved external transmission of proprietary source code risks model retraining on sensitive lending IP and breaches the **Digital Personal Data Protection (DPDP) Act 2023** and **RBI Cyber Security Framework**.
- **C)** Violation of compiler optimization standards; AI chat models strip SIMD vectorization annotations from risk models.
- **D)** Breaching the maximum daily quota of enterprise code submissions under RBI Master Direction on Information Technology Governance.

---

### Question 1.7 (Module 1.3 — GitHub Copilot: Agent Mode vs Ask Mode vs Plan Mode)
**Indian Lending Context**: You are assigned to refactor a loan disbursement orchestration service to support instant direct-to-account payouts complying with **RBI Digital Lending Guidelines (DLG)**. This requires integrating NPCI Penny-Drop IMPS account verification, generating the Key Fact Statement (KFS) PDF, creating an e-NACH mandate via NPCI API, and registering an e-Sign workflow with NeSL.  
**Core Question**: In GitHub Copilot's modern interface, which interaction mode is specifically designed for autonomous multi-step, multi-file execution across your project workspace?
- **A)** **Ask Mode**: Best for generating full-workspace edits via simple conversational prompts.
- **B)** **Plan Mode**: Used only to compile markdown documentation without inspecting file trees.
- **C)** **Agent Mode**: Leverages tool-calling loops to inspect directory structures, plan dependencies, edit multiple files autonomously, and run terminal build checks.
- **D)** **Edit Mode**: Standard single-line inline completions using keyboard tab triggers.

---

### Question 1.8 (Module 1.3 — GitHub Copilot: Custom Instruction Files)
**Indian Lending Context**: Your bank/NBFC mandates that all Java Spring Boot microservices across the lending platform must:
1. Use `java.math.BigDecimal` with explicit `RoundingMode.HALF_EVEN` for all loan principals, fees, and interest calculations in INR.
2. Annotate all loan disbursement and ledger mutations with `@Transactional(rollbackFor = Exception.class, isolation = Isolation.SERIALIZABLE)`.
3. Never log raw borrower Permanent Account Numbers (PAN), Aadhaar numbers (first 8 digits must be masked as `XXXX-XXXX-1234`), or Credit Bureau CIR scores.  
**Core Question**: Where should the team place project-wide instructions so that GitHub Copilot automatically incorporates these rules into all developer interactions in VS Code / JetBrains?
- **A)** In an environment variable named `COPILOT_SYSTEM_PROMPT` on each developer's laptop.
- **B)** In `.github/copilot-instructions.md` within the root of the repository.
- **C)** In a global snippet file located at `~/.config/github/copilot.json`.
- **D)** As comments at the very top of each developer's `pom.xml` or `build.gradle` file.

---

### Question 1.9 (Module 1.3 — Model Context Protocol (MCP) in Copilot)
**Indian Lending Context**: A developer needs GitHub Copilot to validate whether an incoming mortgage loan collateral schema matches the central repository schema of **CERSAI** (Central Registry of Securitisation Asset Reconstruction and Security Interest of India) before generating an entity mapping class.  
**Core Question**: How does Model Context Protocol (MCP) integration extend GitHub Copilot's capabilities in this scenario?
- **A)** MCP compiles the database SQL schema directly into Copilot's underlying model weights during weekly retraining cycles.
- **B)** MCP provides a standardized client-server protocol enabling Copilot to securely query external tools, databases, and enterprise servers to fetch real-time contextual schema information.
- **C)** MCP acts as a VPN tunnel encrypting Copilot's cloud traffic to bypass enterprise network inspection firewalls.
- **D)** MCP converts relational SQL databases into vector embeddings stored on GitHub's public cloud servers.

---

### Question 1.10 (Module 1.3 — GH-300 Certification & Enterprise Compliance)
**Indian Lending Context**: You are configuring GitHub Copilot for 500 developers working across retail personal loans, MSME lending, and two-wheeler vehicle financing. The compliance officer insists that Copilot must never suggest verbatim public code snippets that might subject the lender to GPL copyleft licensing claims.  
**Core Question**: Which GitHub Copilot administrative policy setting must be enforced at the enterprise organization level?
- **A)** Enable "Public Code Ingestion Filtering" and set "Suggestions matching public code" to **Blocked**.
- **B)** Set "Model Temperature" to `0.0` in the organization settings dashboard.
- **C)** Disable telemetry logging and enforce strict SSH key signing on all Copilot prompt payloads.
- **D)** Configure Copilot to run exclusively in local offline mode without internet connectivity.

---

### Question 1.11 (Module 1.4 — Claude Code CLI Architecture)
**Indian Lending Context**: A senior engineer is using Claude Code in a terminal environment to modernize a batch loan repayment reconciliation service that processes NPCI NACH return clearing files (interpreting rejection codes like `E01` for insufficient funds or `R01` for mandate cancelled). The developer executes `claude` in the project root.  
**Core Question**: What is the primary architectural differentiator of Claude Code compared to traditional IDE autocomplete extensions?
- **A)** Claude Code only generates Python scripts and cannot interact with compiled languages like Go or C#.
- **B)** Claude Code is an agentic, terminal-native tool that directly reads project files, executes bash/shell commands, runs test suites, checks git diffs, and iterates autonomously to solve tasks.
- **C)** Claude Code runs a local quantized 7B model entirely on the developer's laptop CPU without sending network requests.
- **D)** Claude Code replaces the operating system kernel with an AI-directed hypervisor to sandbox lending software.

---

### Question 1.12 (Module 1.4 — CLAUDE.md Memory & Project Configuration)
**Indian Lending Context**: In an MSME GSTN invoice-discounting loan origination repository, the engineering team has strict standards for building and running tests:
- Build: `./gradlew clean build -x test`
- Verification: `./gradlew test --tests *GstnInvoiceDiscountingIntegrationTest`
- Coding Rule: Never commit `.env` files or borrower test credentials.  
**Core Question**: How should these project-specific commands and guardrails be documented so Claude Code reads them automatically at the start of every session?
- **A)** Add them to a text file named `CLAUDE.md` in the root of the project directory.
- **B)** Pass them as command-line arguments: `claude --rules="./gradlew test" --no-secrets`.
- **C)** Upload them to the public Anthropic Web Console under "Custom GPT Instructions".
- **D)** Add them to the Git global configuration under `git config --global claude.instructions`.

---

### Question 1.13 (Module 1.4 — Claude Code Permission Safety in Indian Lending)
**Indian Lending Context**: An engineer is running Claude Code to refactor an escrow settlement service complying with RBI DLG rules (ensuring disbursement flows directly from the Regulated Entity's escrow bank to the borrower). Claude Code suggests running a command: `git clean -fdx` and `rm -rf /var/lending/escrow_cache/`.  
**Core Question**: Why is the `--dangerously-skip-permissions` flag strictly prohibited in enterprise Indian lending development environments?
- **A)** It slows down CLI processing by forcing Claude to verify each command against a remote CERT-In database.
- **B)** It bypasses the interactive confirmation prompt, granting the agent unmonitored capability to run destructive terminal commands, delete uncommitted code, or alter system state.
- **C)** It triggers an automatic downgrade of Claude's model context window from 200k to 8k tokens.
- **D)** It invalidates the institution's commercial license agreement with Anthropic.

---

### Question 1.14 (Module 1.5 — Google Antigravity IDE: Architecture & Model Selection)
**Indian Lending Context**: A developer switches to Google Antigravity IDE to develop an early warning default prediction model and collections optimizer for retail loans. A colleague claims: *"Antigravity is just an Anthropic Claude wrapper and requires a Claude Pro subscription."*  
**Core Question**: According to the official Track A curriculum, what is the correct architecture of Google Antigravity?
- **A)** The colleague is correct; Antigravity is a VS Code fork developed exclusively by Anthropic for Claude Code.
- **B)** Antigravity is Google's agentic IDE designed to execute Google Gemini models alongside other foundation models, featuring native agentic workflows, sidecars, and workspace context integration without requiring a Claude subscription.
- **C)** Antigravity is a cloud-only mainframe emulator built specifically for legacy COBOL banking systems.
- **D)** Antigravity is an open-source Linux package manager that automatically installs AI CLI tools.

---

### Question 1.15 (Module 1.5 — Antigravity IDE Context & Task Management)
**Indian Lending Context**: While refactoring a loan portfolio stress-testing engine in Google Antigravity, a long-running Maven integration test suite is simulating 50,000 delinquent loan default paths across Indian credit cycles in the background. The developer needs the IDE agent to pause, wait for test results, and then inspect the resulting stress-test report artifact.  
**Core Question**: In Antigravity's reactive task execution model, how does the agent interact with background tasks?
- **A)** The agent must enter a continuous busy-wait loop, querying `get_status` every 500 milliseconds until the process exits.
- **B)** The agent relies on reactive event wakeups; background tasks notify the agent upon completion, avoiding wasteful CPU polling loops while maintaining state.
- **C)** The agent terminates the background task immediately and re-runs the tests in synchronous single-threaded mode.
- **D)** The agent delegates the task to the operating system cron daemon and closes the workspace.

---

### Question 1.16 (Module 1.5 — Antigravity Artifacts & Transparency)
**Indian Lending Context**: A team lead requires all developers using Antigravity on core Loan Origination Systems (LOS) to document architectural refactoring plans before applying code edits to credit underwriting rule classes.  
**Core Question**: How does Google Antigravity facilitate structured, reviewable plans prior to automated execution?
- **A)** By forcing developers to write physical memos and scan them into the project repository.
- **B)** Through the creation of interactive Markdown Artifacts in the brain directory, allowing humans and agents to inspect, verify, and approve step-by-step execution plans before code modification.
- **C)** By automatically submitting PRs to GitHub without local workspace changes.
- **D)** By encrypting prompt history into binary log files readable only by Google Cloud support.

---

### Question 1.17 (Module 1.6 — Prompt Engineering: System Constraints & Roles)
**Indian Lending Context**: A junior developer writes this prompt in Copilot Chat:  
*"Write a function to disburse an approved digital personal loan to a borrower's bank account."*  
The generated code simply decrements a balance variable and transfers money to a third-party Loan Service Provider (LSP) pool account without verifying RBI Digital Lending Guidelines (DLG) direct disbursement rules, Penny-Drop account validation, or generating a Sanction Letter.  
**Core Question**: Applying the official GitHub Prompt Engineering framework, how should this prompt be structured to produce enterprise-grade Indian lending code?
- **A)** Add: *"Please write it very nicely and make sure there are no bugs."*
- **B)** Structure the prompt with **Role** (Senior Indian FinTech Lending Engineer), **Context** (Spring Boot with JPA), **Explicit Constraints** (ACID `@Transactional`, optimistic locking on `LoanApplication` entity verifying status is `SANCTIONED`, direct disbursement from Lender's Escrow to borrower's verified bank account via IMPS per RBI DLG, mandatory Penny-Drop validation check, KFS reference number generation), and **Expected Output Format**.
- **C)** Repeat the word *"CRITICAL"* five times in capital letters at the beginning of the prompt.
- **D)** Ask the model to generate the code in Python first, then translate it to Java.

---

### Question 1.18 (Module 1.6 — Few-Shot Prompting for Complex Indian Bureau Formats)
**Indian Lending Context**: You need an AI assistant to generate a parser for raw TransUnion CIBIL 36-month payment history DPD (Days Past Due) strings embedded in trade-line records (e.g., `000000030060090XXXXXX`, where `000` = on time, `030` = 30 days overdue, `XXX` = no data reported). The LLM repeatedly outputs naive substring splits that misalign historical months.  
**Core Question**: Which prompt engineering technique is most effective for guiding the LLM to adhere strictly to CIBIL's 3-character monthly DPD block structure?
- **A)** **Zero-shot prompting**: Providing no examples to avoid biasing the model's pre-trained weights.
- **B)** **Few-shot prompting**: Providing 2–3 paired input-output examples in the prompt demonstrating the exact raw 36-character DPD string, the start date tag, and the resulting parsed list of monthly repayment status objects.
- **C)** **Chain-of-thought compression**: Removing all whitespace and delimiters from the prompt to fit more tokens.
- **D)** **Prompt chaining across different LLMs**: Running the prompt sequentially across 4 different AI vendors.

---

### Question 1.19 (Module 1.6 — Negative Constraints vs Positive Instruction)
**Indian Lending Context**: A developer attempts to prevent Copilot from using legacy, deprecated crypto libraries when encrypting borrower Aadhaar offline e-KYC XML data by prompting: *"Do NOT use any deprecated DES or 3DES algorithms. Do NOT use MD5. Do NOT use Apache Commons Crypto."*  
Copilot nevertheless generates code using `org.apache.commons.crypto.cipher.CryptoCipher` with 3DES.  
**Core Question**: Why did the negative constraint fail, and how does proper prompt engineering correct it?
- **A)** LLMs have a hardcoded bias towards 3DES due to 1990s training data that cannot be overridden by prompts.
- **B)** Negative constraints often trigger attention on the forbidden tokens (DES, MD5, Apache Commons); the effective technique is **positive instruction** specifying the exact permitted library and algorithm (e.g., *"Use `javax.crypto.Cipher` with `AES/GCM/NoPadding` and 256-bit keys per UIDAI security standards"*).
- **C)** The prompt contained too few exclamation marks to trigger the safety alignment filter.
- **D)** Copilot Chat ignores all sentences containing the word "NOT".

---

### Question 1.20 (Module 1.6 — Context Provisioning & Anchor Files)
**Indian Lending Context**: You are implementing an Automated Underwriting Rule Engine that must call an existing internal `CibilScoreEvaluator` and `FoirCalculator` (Fixed Obligation to Income Ratio). When prompting Copilot Chat in your IDE, the model invents fake method signatures for both classes.  
**Core Question**: Which developer action provides the necessary local context to ground Copilot Chat in VS Code?
- **A)** Open `CibilScoreEvaluator.java` and `FoirCalculator.java` in active editor tabs, or use `#file:CibilScoreEvaluator.java` in Copilot Chat to anchor the interface definitions in the prompt context.
- **B)** Restart VS Code and re-install the GitHub Copilot extension.
- **C)** Copy-paste the entire binary `.class` file into the chat window.
- **D)** Push the code to a public GitHub repository so Copilot's base model can index it overnight.

---
*(End of Module 01 — Refer to Document 04 for Master Answer Key & Distractor Rationales)*
