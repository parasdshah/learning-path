# Assessment Module 02: Tier 2 — AI-Augmented Development Workflows
## AI for Coders: Developer Competency Assessment (20 Questions | Weight: 40%)

> **Target Audience**: Software Developers working on Lending Products (LOS, LMS, Credit Services).  
> **Curriculum Covered**: Modules 2.1 through 2.6 of Track A (`_outputs/02_track_a_developers.md`).  
> **Core Focus**: Agentic coding patterns (Plan→Execute→Verify), task decomposition, AI-assisted debugging (`/explain`→`/fix`), automated test generation, context management (`AGENTS.md`), version control workflows, and critical review of AI output.

---

### Question 2.1 (Module 2.1 — Agentic Plan-Execute-Verify Loop)
**Scenario**: A developer is tasked with refactoring a legacy loan repayment schedule generator to a modern event-driven service. The change involves 10 interdependent classes and database schema updates.  
**Core Question**: What is the most reliable agentic workflow pattern to complete this refactoring without introducing regressions?
- **A)** Send a single prompt asking the AI agent to rewrite the entire package in one pass.
- **B)** Follow the **Plan → Execute → Verify** loop: First, prompt the agent to analyze dependencies and output a step-by-step plan; second, execute changes in small, incremental steps; third, run automated test suites and compiler checks after every step before proceeding.
- **C)** Let the agent generate code directly into the main branch and rely on runtime logs in staging to find bugs.
- **D)** Manually write all implementations first and use AI only to add comments afterwards.

---

### Question 2.2 (Module 2.1 — Task Decomposition for Agentic Coding)
**Scenario**: A developer asks Copilot Agent Mode to implement a dual-approval loan underwriting workflow. In response, the agent attempts to generate a single 850-line monolithic controller containing database queries, business rules, notification dispatches, and REST endpoints.  
**Core Question**: How should an experienced developer decompose this task to guide the agent toward clean software architecture?
- **A)** Ask the agent to minify the 850-line file into a single line so it processes faster.
- **B)** Break the task into discrete, modular prompts: (1) Domain entity and state machine for Approval Status, (2) Repository layer with locking mechanisms, (3) Service layer with approval business logic, (4) Event notification listener, and (5) REST controller with DTO validation.
- **C)** Accept the monolithic controller because AI agents work best when all code is in one file.
- **D)** Run `/fix` repeatedly on the 850-line file until SonarQube stops flagging issues.

---

### Question 2.3 (Module 2.1 — Tool-Calling & Closed-Loop Verification in Agent Mode)
**Scenario**: A developer uses Copilot Agent Mode to resolve a NullPointerException in a loan delinquency calculation method.  
**Core Question**: What key capability distinguishes Agent Mode from standard conversational chat when validating code fixes?
- **A)** Agent Mode connects to human brainwaves to assess satisfaction.
- **B)** Agent Mode can use tool calls to execute terminal commands (e.g., `./gradlew test`), inspect stdout/stderr compiler and test feedback, and autonomously iterate on code edits until tests pass.
- **C)** Agent Mode automatically pays cloud hosting bills using corporate cards.
- **D)** Agent Mode eliminates the need for unit tests by mathematically proving code correctness.

---

### Question 2.4 (Module 2.1 — MCP External Tool Integration for Schemas)
**Scenario**: An engineering team maintains an internal schema registry managing 100+ microservice API contracts. A developer using an agentic IDE needs to generate client DTOs for a loan valuation service.  
**Core Question**: How does configuring a Model Context Protocol (MCP) server for the schema registry improve the agent's output?
- **A)** The agent directly queries the MCP server to fetch the live, accurate OpenAPI schema, ensuring generated DTOs match actual service contracts without hallucinations.
- **B)** The MCP server compiles REST endpoints into machine binary code to bypass the JVM.
- **C)** The MCP server overrides corporate network firewalls to deploy unapproved code to production.
- **D)** The MCP server guarantees that generated code will execute with zero network latency.

---

### Question 2.5 (Module 2.2 — Progressive Root Cause Analysis: `/explain` → `/fix`)
**Scenario**: During peak batch processing of monthly loan installment payments, a database connection pool exhaustion error crashes the service. A developer pastes a 100-line stack trace into Copilot Chat.  
**Core Question**: According to the official debugging workflow (Module 2.2), what is the best two-stage methodology to resolve this bug?
- **A)** Immediately invoke `/fix` with the prompt *"Fix connection pool now"* and accept whatever code diff is generated.
- **B)** First use `/explain` with the stack trace, connection pool configuration, and transaction lifecycle code to identify the root cause (e.g., unclosed connections in exception blocks); second, after validating the diagnosis, invoke `/fix` targeted specifically at releasing connections in a `finally` block or tuning pool parameters.
- **C)** Ignore the stack trace and ask the AI to rewrite the service in another programming language.
- **D)** Prompt Copilot to generate a cron script that restarts the application container every 15 minutes.

---

### Question 2.6 (Module 2.2 — AI-Assisted Diagnosis of Concurrency Race Conditions)
**Scenario**: In a digital loan credit-line service, two concurrent withdrawal requests for $800 arrive simultaneously for an account with $1,000 available credit. Both requests succeed, leaving the account overdrawn at $1,600 without triggering credit limit alerts.  
**Core Question**: What classic concurrency bug should an AI-assisted debugging workflow help identify in the repository layer?
- **A)** A Time-of-Check to Time-of-Use (TOCTOU) race condition caused by non-atomic read-then-write operations without pessimistic locking (`SELECT ... FOR UPDATE`) or optimistic versioning (`@Version`).
- **B)** Memory bus cache contention in the developer's laptop keyboard.
- **C)** Inadequate RAM allocation in the Docker host container.
- **D)** The SQL query optimizer converting lowercase table names to uppercase.

---

### Question 2.7 (Module 2.2 — Sanitizing Log Analysis Prompts)
**Scenario**: A developer encounters an unhandled exception in a loan application intake service. The production error log contains real applicant names, Social Security / Tax ID numbers, bank account details, and credit scores.  
**Core Question**: What pre-processing step is mandatory before pasting this log into an AI debugging tool?
- **A)** Gzip the log file before pasting to save token budget.
- **B)** Sanitize, redact, or mask all Personally Identifiable Information (PII), customer credentials, and sensitive account data before sending it to the AI tool.
- **C)** Add a prompt instruction: *"Please treat this customer data as strictly confidential."*
- **D)** Encrypt the chat prompt with PGP and post it to a public developer forum.

---

### Question 2.8 (Module 2.3 — Generating Tests for Idempotency)
**Scenario**: A developer is building a loan disbursement API endpoint that accepts an `Idempotency-Key` HTTP header. If a network timeout occurs, the client retries the request with the identical key.  
**Core Question**: When prompting an AI tool to generate comprehensive test cases for this endpoint, which test scenario is essential to verify?
- **A)** Verifying that the API returns HTTP 200 within 5 milliseconds when given invalid JSON.
- **B)** Simulating two identical concurrent requests with the same idempotency key, asserting that exactly one disbursement transaction is created, the second returns the cached original response, and no duplicate transfer occurs.
- **C)** Verifying that the idempotency key is logged in cleartext in console logs.
- **D)** Asserting that sending 1,000,000 keys crashes the in-memory cache.

---

### Question 2.9 (Module 2.3 — Financial Boundary Value & Edge-Case Test Generation)
**Scenario**: An engineer prompts Copilot: *"Generate unit tests for calculateLoanAmortization()."* The AI outputs three simple positive tests using $10,000 at 5% interest over 12 months.  
**Core Question**: When reviewing and refining the AI-generated test suite, which critical boundary conditions should the developer ensure are tested?
- **A)** Only test strings and booleans to confirm Java compilation.
- **B)** Zero interest rate (0% promotional loans), maximum facility amounts (`Long.MAX_VALUE`), fractional-cent rounding, early payoffs, and leap year day-count calculations.
- **C)** Testing whether removing comments makes the code run faster.
- **D)** Verifying that method parameter names match British English spelling conventions.

---

### Question 2.10 (Module 2.3 — Synthetic Test Data Generation)
**Scenario**: A QA engineer asks an AI coding assistant: *"Generate a SQL seed script with 50 realistic loan applicant records for integration testing."*  
**Core Question**: What engineering best practice must be followed when using AI to generate test datasets?
- **A)** The AI should scrape production databases to ensure real customer data realism.
- **B)** The AI should generate purely synthetic data using dummy names, fake identifiers (e.g., standard test SSN/PAN formats), and mock credit scores, with zero use of real customer data.
- **C)** The test records should use real employee phone numbers to test SMS alerting.
- **D)** AI-generated test data never requires review because it is generated in memory.

---

### Question 2.11 (Module 2.3 — Reviewing AI-Generated Documentation)
**Scenario**: A developer uses Copilot Agent Mode to generate OpenAPI specifications and Javadoc for a loan repayment API.  
**Core Question**: What common deficiency in AI-generated documentation must the developer actively correct?
- **A)** AI models refusing to write descriptions longer than 10 words.
- **B)** Superficial descriptions that merely restate method names (e.g., `processPayment(): Processes the payment`) while omitting critical business constraints, error codes (HTTP 409 Conflict, 422 Unprocessable), and transaction boundaries.
- **C)** The AI automatically embedding bash scripts inside OpenAPI YAML files.
- **D)** The AI translating English documentation into Latin by default.

---

### Question 2.12 (Module 2.4 — The AGENTS.md Standard for Context Management)
**Scenario**: A repository contains multiple microservices. When developers use AI coding tools, the assistants frequently suggest outdated libraries and violate internal coding conventions.  
**Core Question**: According to the Linux Foundation `AGENTS.md` open standard (Module 2.4), how does adding an `AGENTS.md` file to the repository solve this problem?
- **A)** It automatically installs software updates on developer laptops without user input.
- **B)** It provides a standardized, vendor-neutral configuration file documenting repository architecture, approved libraries, build commands, and coding rules that compliant AI agents parse upon session startup.
- **C)** It encrypts the entire repository so only AI agents can read it.
- **D)** It legally transfers code copyright to the AI model vendor.

---

### Question 2.13 (Module 2.4 — Hierarchical Context in Monorepos)
**Scenario**: In a monorepo containing a Python machine learning credit scoring service and a Java Spring Boot loan ledger, the Python project requires Flake8 / Black style rules, while the Java project mandates Checkstyle and strict typing.  
**Core Question**: How does the `AGENTS.md` / `.agents/` standard support different rules across sub-projects in a single repository?
- **A)** Monorepos are unsupported; the project must be split into separate physical repositories.
- **B)** Through hierarchical context: subdirectories can maintain their own localized `AGENTS.md` or `.agents/rules/` that override or extend the root project configuration when the agent works in that directory.
- **C)** By running two separate AI models on alternating minutes.
- **D)** The AI agent randomly selects which rule set to follow on each prompt.

---

### Question 2.14 (Module 2.4 — Context Window Bloat & Token Degradation)
**Scenario**: A developer attempts to provide "complete context" by attaching all 50 source files in a package into a single prompt. The developer notices that the AI assistant begins hallucinating and ignores explicit instructions.  
**Core Question**: What context management best practice avoids this issue?
- **A)** Keep expanding the context window to 10 million tokens using third-party browser plugins.
- **B)** Provide lean, high-signal context: attach only the target file, relevant interface definitions, and immediate dependencies (using precise `#file` anchors), rather than dumping entire packages.
- **C)** Minify all source files into single-line strings before prompting.
- **D)** Delete test files so only production code occupies the context window.

---

### Question 2.15 (Module 2.5 — Developer Accountability for AI-Generated PR Summaries)
**Scenario**: After completing a bug fix in a loan interest calculation service, a developer uses GitHub Copilot to generate the Pull Request description.  
**Core Question**: What is the developer's responsibility regarding the AI-generated PR summary before submitting it for review?
- **A)** Submit the generated PR summary without reading it because AI summaries are vendor-certified.
- **B)** Review, verify, and edit the summary to ensure it accurately explains the root cause, references the correct issue ticket (Jira), documents backward compatibility, and lists the exact verification steps performed.
- **C)** Delete the entire summary and replace it with a single sentence: *"Fixed bug."*
- **D)** List the AI model as the co-author and legal owner of the change request.

---

### Question 2.16 (Module 2.5 — Conventional Commits with AI)
**Scenario**: An AI assistant suggests the following commit message after a developer fixes an underwriting eligibility check:  
`commit -m "fixed stuff in underwriting and updated a few files"`  
**Core Question**: Why is this commit message poor practice, and what should the developer instruct the AI to generate instead?
- **A)** Commit messages must be encrypted with PGP before pushing to Git.
- **B)** It lacks clarity and auditability; the developer should require **Conventional Commits** format with clear scope and rationale (e.g., `fix(underwriting): enforce max debt-to-income threshold of 45% [JIRA-4021]`).
- **C)** Commit messages must always contain the full source code diff in the subject line.
- **D)** Commit messages are acceptable as long as the build succeeds.

---

### Question 2.17 (Module 2.5 — Reviewing AI Git Diffs for Hidden Regressions)
**Scenario**: While reviewing an AI-generated Git diff for a credit qualification method, a reviewer spots this change:
```diff
- if (debtToIncomeRatio.compareTo(maxAllowedDti) > 0) {
-     throw new IneligibleBorrowerException("DTI exceeds maximum threshold");
- }
+ // Relaxed check for promotion
+ if (debtToIncomeRatio.compareTo(maxAllowedDti.add(promotionalDtiBuffer)) >= 0) {
+     throw new IneligibleBorrowerException("DTI exceeds maximum threshold");
+ }
```
The developer who submitted the PR had accepted the bulk AI completion without noticing this alteration.  
**Core Question**: What critical flaw occurred during this development workflow?
- **A)** The diff used tabs instead of spaces, causing compilation failure.
- **B)** The AI introduced an unapproved business logic change and altered a strict inequality (`>`) to greater-than-or-equal (`>=`); the developer failed to review the AI diff line-by-line before committing.
- **C)** Java exceptions cannot be thrown inside `if` statements.
- **D)** The method should have used Python dictionary lookups instead of Java `BigDecimal`.

---

### Question 2.18 (Module 2.6 — Critical Code Review: IEEE 754 Floating-Point Hazards)
**Scenario**: An AI coding assistant generates the following calculation for loan monthly payments:
```java
public double calculateMonthlyPayment(double principal, double annualRate, int tenureMonths) {
    double monthlyRate = annualRate / 12.0;
    return (principal * monthlyRate) / (1 - Math.pow(1 + monthlyRate, -tenureMonths));
}
```
**Core Question**: During code review, why must an engineer reject this code for financial calculations?
- **A)** The method lacks Javadoc annotations, causing a Maven build failure.
- **B)** Primitive `double` types introduce binary floating-point rounding errors (e.g., `0.1 + 0.2 != 0.3`), resulting in cumulative rounding discrepancies; financial systems mandate `BigDecimal` with explicit rounding modes.
- **C)** Java math libraries cannot calculate exponential powers greater than 12.
- **D)** The formula should use integer divisions instead of floating-point divisions.

---

### Question 2.19 (Module 2.6 — AI Package Hallucination & Supply Chain Risks)
**Scenario**: When asked to implement a specialized validation utility for loan account numbers, an AI tool suggests:
```javascript
const loanValidator = require('enterprise-loan-num-validator');
```
A developer runs `npm install enterprise-loan-num-validator`. The package installs successfully, but two days later, sensitive environment variables begin leaking to an unknown external server.  
**Core Question**: What software supply chain attack vector took advantage of the AI tool's output?
- **A)** SQL Injection via HTTP headers.
- **B)** **AI Package Hallucination / Slopsquatting**: An attacker identified common package names hallucinated by LLMs, registered a malicious package under that name on npm, and waited for developers to blindly install it.
- **C)** Man-in-the-middle attack on the developer's wireless keyboard.
- **D)** Cross-Site Scripting (XSS) inside the terminal command prompt.

---

### Question 2.20 (Module 2.6 — The Four-Pillar AI Code Review Framework)
**Scenario**: A team establishes a standard review checklist for evaluating all AI-generated pull requests before merging into main branches.  
**Core Question**: According to the official curriculum (Module 2.6), what are the four critical dimensions every engineer must evaluate?
- **A)** Speed of generation, Token count, Model temperature, and Prompt length.
- **B)** Correctness, Security, Performance, and Maintainability.
- **C)** Lines of code, Number of comments, Author seniority, and IDE theme.
- **D)** Cloud hosting cost, GPU utilization, RAM usage, and Network bandwidth.

---
*(End of Module 02 — Refer to Document 04 for Master Answer Key & Distractor Rationales)*
