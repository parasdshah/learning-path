# Assessment Module 02: Tier 2 — AI-Augmented Development Workflows
## Enterprise India Lending Developer Evaluation (20 Questions | Weight: 40%)

> **Scope**: Covers Modules 2.1 through 2.6 of Track A. Focuses on Agentic Coding Patterns (Plan→Execute→Verify loops), AI-Assisted Debugging (`/explain`→`/fix`), Test Generation for Indian Lending Criticality, Context Management (`AGENTS.md`, `.agents/`), Version Control Auditability, and Critical Code Review (Vetting AI Hallucinations & Security in Indian LOS and Credit Rating Software).

---

### Question 2.1 (Module 2.1 — Agentic Plan-Execute-Verify Loop)
**Indian Lending Context**: A lead software engineer needs to migrate a legacy batch loan interest accrual and repayment engine (using reducing balance interest in INR) to an event-driven microservice handling instant **UPI AutoPay** and **e-NACH** installment settlements. The migration touches 12 interdependent domain services, loan schedule tables, and strict RBI regulatory reporting pipelines.  
**Core Question**: What is the most reliable agentic workflow pattern to execute this complex migration without introducing financial calculation regressions?
- **A)** Instruct an AI agent in one prompt: *"Rewrite the entire lending calculation engine to reactive Spring Boot immediately."*
- **B)** Follow the **Plan → Execute → Verify** loop: First, have the agent analyze current calculation dependencies and output a verifiable migration plan; second, execute refactoring in isolated, incremental sub-tasks; third, run automated amortization test suites and compiler checks after every step before proceeding.
- **C)** Let the AI agent generate code directly into the production branch and rely on customer delinquency complaints to catch errors.
- **D)** Manually write all interfaces first, then use inline tab completion only for getters and setters.

---

### Question 2.2 (Module 2.1 — Task Decomposition in Indian Lending Systems)
**Indian Lending Context**: You are implementing a dual-authorization ("maker-checker") underwriting workflow for commercial and MSME credit lines exceeding ₹5,00,00,000 (5 Crore). When prompting Copilot Agent Mode, the agent generates a single 850-line monolithic controller handling credit officer authentication, CERSAI collateral queries, GSTN GSTR-3B tax verification, database mutations, and adverse action notification dispatch.  
**Core Question**: As an SME, how should you decompose this task to guide the agent toward clean lending system architecture?
- **A)** Ask the agent to minify the 850-line file so that it fits into memory.
- **B)** Decompose into discrete architectural milestones: (1) Domain entity and state machine for Commercial Loan Approval Status, (2) Idempotent database repository layer with optimistic locking, (3) Maker-Checker credit delegation authority business logic, (4) Event-driven GSTN/CERSAI appraisal listener, and (5) REST API controller with DTO validation.
- **C)** Accept the monolithic controller because agentic AI prefers single-file architectures to avoid imports.
- **D)** Run `/fix` repeatedly on the 850-line file until it passes SonarQube checks.

---

### Question 2.3 (Module 2.1 — Tool-Calling & Environment Feedback in Agent Mode)
**Indian Lending Context**: A developer utilizes Copilot Agent Mode to fix an intermittent NullPointerException in a batch loan delinquency classification engine (transitioning delinquent accounts across SMA-0, SMA-1, SMA-2, and NPA buckets per **RBI Prudential Norms on Income Recognition and Asset Classification [IRAC]**). The agent edits a calculation method and claims the bug is resolved.  
**Core Question**: In true agentic workflows, what critical capability differentiates Agent Mode from standard chat when validating fixes?
- **A)** Agent Mode connects to developer brainwaves to determine satisfaction.
- **B)** Agent Mode can execute terminal commands (e.g., `./gradlew test --tests IracDelinquencyClassificationTest`), inspect the stdout/stderr compiler and test execution feedback, and self-correct code edits iteratively if tests fail.
- **C)** Agent Mode automatically disburses funds to test borrower accounts via corporate credit cards.
- **D)** Agent Mode replaces the need for continuous integration (CI) servers by running permanent background daemons.

---

### Question 2.4 (Module 2.1 — MCP External Tool Integration for Account Aggregator Awareness)
**Indian Lending Context**: Your bank/NBFC integrates with the **Account Aggregator (AA)** ecosystem (ReBIT specifications / Sahamati network) to fetch real-time financial information (bank statements) from Financial Information Providers (FIPs). A developer using an agentic IDE needs to build a client for the `AccountAggregatorConsentManagerV2` service.  
**Core Question**: How does configuring a Model Context Protocol (MCP) server for the enterprise schema registry optimize the agent's output?
- **A)** The agent directly calls the MCP tool to query real-time OpenAPI/JSON schemas conforming to ReBIT AA specifications, ensuring generated consent request/response DTOs match live endpoints exactly, eliminating contract hallucinations.
- **B)** The MCP server automatically overrides internal lending firewalls to deploy unapproved services to production.
- **C)** The MCP server translates REST payloads into binary machine code bypassing Java bytecode compilation.
- **D)** The agent no longer needs to write error handling because MCP guarantees 100% network uptime.

---

### Question 2.5 (Module 2.2 — Progressive Root Cause Analysis: `/explain` → `/fix`)
**Indian Lending Context**: In a high-volume retail lending platform, database connection pool exhaustion occurs on the 5th of every month when 300,000 monthly auto-debit installments are presented via **NPCI e-NACH / UPI AutoPay**. A developer pastes a 120-line stack trace into Copilot Chat.  
**Core Question**: What is the most effective two-stage debugging methodology recommended in the GitHub Copilot debugging framework?
- **A)** Immediately invoke `/fix` with the prompt *"Fix connection pool now"* and apply whatever diff is generated.
- **B)** First invoke `/explain` with the stack trace, connection pool configuration, and batch repayment transaction lifecycle code to identify the root cause (e.g., unclosed connections in installment exception branches or missing pagination during NACH response processing); second, after validating the diagnosis, invoke `/fix` targeted specifically at releasing connections in a `finally` block or tuning pool parameters.
- **C)** Ignore the stack trace and ask the AI to rewrite the batch billing service in Go.
- **D)** Prompt Copilot to generate a script that kills and restarts the application container every 10 minutes.

---

### Question 2.6 (Module 2.2 — Diagnosing Silent Concurrency Bugs in Revolving Credit Lines)
**Indian Lending Context**: A borrower has an approved digital revolving credit line (BNPL / Instant Credit) of ₹1,00,000 with a current drawn balance of ₹90,000 (available credit = ₹10,000). Two concurrent drawdown requests of ₹8,000 each arrive simultaneously from different e-commerce checkout sessions. Both requests succeed, leaving the account at ₹1,06,000 drawn and violating the borrower's credit limit without triggering risk alerts.  
**Core Question**: What subtle concurrency bug should an AI-assisted debugging workflow help uncover in the database access layer?
- **A)** CPU cache line bouncing in the Kubernetes worker node.
- **B)** A Time-of-Check to Time-of-Use (TOCTOU) race condition caused by non-atomic read-then-write operations without pessimistic row-level locking (`SELECT ... FOR UPDATE`) or optimistic versioning (`@Version`) on the credit line balance entity.
- **C)** Inadequate RAM allocation in the JVM heap space causing garbage collection pauses.
- **D)** The database driver converting SQL queries to uppercase strings.

---

### Question 2.7 (Module 2.7 — Sanitizing Log Analysis Prompts in Indian Lending)
**Indian Lending Context**: An unhandled exception occurs in a digital loan origination application during PAN and CKYC verification. The production error log contains:  
`[ERROR] Underwriting failed for Applicant PAN: ABCDE1234F, Aadhaar: 1234-5678-9012, AnnualIncome: ₹12,00,000, CIBIL: 780, Employer: TCS, BankAcc: 987654321012. StackTrace: ...`  
The developer wants to feed this log into an AI debugging tool.  
**Core Question**: What pre-processing step is legally and procedurally mandatory under the **Digital Personal Data Protection (DPDP) Act 2023**, UIDAI regulations, and RBI Cyber Security directions?
- **A)** Compress the log file with gzip before pasting it to save tokens.
- **B)** Sanitize, redact, and mask all Personally Identifiable Information (PII) — including PAN, Aadhaar number (must be completely masked or truncated to last 4 digits), applicant names, bank account numbers, credit scores, and income figures — before injecting the log into any AI context.
- **C)** Add a prompt instruction: *"Please keep this borrower data confidential."*
- **D)** Encrypt the chat prompt with PGP and upload it to the AI vendor's public forum.

---

### Question 2.8 (Module 2.3 — Generating Idempotent Loan Disbursement Tests)
**Indian Lending Context**: An engineer is building an instant personal loan disbursement API that executes via **NPCI IMPS** directly from the lender's escrow account to the borrower's bank account, accepting an `X-Disbursement-Idempotency-Key` HTTP header. If a network timeout occurs while transferring ₹50,000, the client retries the request with the identical key.  
**Core Question**: When instructing an AI tool to generate comprehensive test cases for this endpoint, which test scenario is vital for lending reliability?
- **A)** Verifying that the API returns HTTP 200 within 10 milliseconds when called with invalid JSON.
- **B)** Simulating two identical concurrent requests with the same idempotency key, asserting that exactly one IMPS disbursement instruction is posted to the core banking ledger, the second returns the cached original response, and no duplicate funds are transmitted.
- **C)** Asserting that the idempotency key is stored in cleartext in the application log file.
- **D)** Verifying that generating 1,000,000 unique keys crashes the in-memory Redis cluster.

---

### Question 2.9 (Module 2.3 — Financial Boundary Value & Edge-Case Test Generation)
**Indian Lending Context**: An engineer prompts Copilot: *"Generate unit tests for the calculateLoanAmortization() function."*  
The AI generates three basic positive tests with loan amounts ₹1,00,000, ₹5,00,000, and ₹10,00,000 at 12% reducing balance interest over 12 months.  
**Core Question**: As an SME reviewing this AI output, which critical Indian lending boundary conditions must you ensure are included in the test suite?
- **A)** Only test strings and boolean types to verify Java compilation.
- **B)** Zero interest promotional loans (0% subvention schemes), broken-period interest calculation between loan disbursement and the first EMI date, maximum facility values (₹50,00,00,000+), early full prepayment (asserting zero foreclosure penalty for floating-rate individual loans per RBI Fair Practices Code), and leap year day-count variations.
- **C)** Testing whether the function runs faster when comments are removed.
- **D)** Validating that the method name conforms to British English spelling conventions.

---

### Question 2.10 (Module 2.3 — Synthetic vs Production Test Data Generation)
**Indian Lending Context**: A QA engineer asks an AI coding assistant: *"Generate a SQL seed script with 50 realistic borrower loan applications for testing the automated underwriting rule engine."*  
**Core Question**: What data governance practice must be adhered to when using AI to generate Indian lending test datasets?
- **A)** The AI must scrape production loan origination databases to ensure high realism.
- **B)** The AI must generate purely synthetic data using fictitious Indian names, validly formatted dummy PANs with test patterns, synthetic CIBIL scores (300–900), and mock addresses, with zero reliance on actual applicant PII.
- **C)** The test records must include actual loan officers' personal cell phone numbers to test SMS alerting.
- **D)** Test datasets generated by AI do not require masking because they reside on local developer workstations.

---

### Question 2.11 (Module 2.3 — Automated Documentation & OpenAPI Contracts)
**Indian Lending Context**: A team is refactoring an Indian loan servicing API. The developer uses Copilot Agent Mode to generate OpenAPI 3.0 (Swagger) specifications and Javadoc for the repayment schedule endpoints.  
**Core Question**: What common AI documentation flaw must the developer actively inspect and correct?
- **A)** The AI refusing to write comments longer than 10 words.
- **B)** Superficial docstrings that merely restate method names (e.g., `makeRepayment(): Makes a repayment`) while omitting crucial lending business rules, error codes (HTTP 409 Conflict for concurrent repayment, 422 for invalid tenure), NACH bounce charges, KFS parameter disclosures, and day-count convention assumptions.
- **C)** The AI embedding executable bash scripts inside OpenAPI YAML descriptions.
- **D)** The AI translating English documentation into ancient Latin automatically.

---

### Question 2.12 (Module 2.4 — Managing Context with AGENTS.md Standard)
**Indian Lending Context**: An enterprise Indian lending repository contains 18 microservices spanning loan origination, CIBIL bureau pull, Account Aggregator consent, collateral valuation, and collections. When developers use AI assistants, the models frequently hallucinate obsolete library versions and violate team conventions.  
**Core Question**: According to the Linux Foundation `AGENTS.md` open standard, how does placing an `AGENTS.md` file in the repository root resolve this issue?
- **A)** It automatically installs software updates on developer laptops without user consent.
- **B)** It provides a vendor-neutral, standardized configuration file containing repository architecture overviews, coding standards, approved dependencies, build commands, and security boundaries that any compliant AI agent (Copilot, Claude Code, Antigravity, Cursor) parses upon session initialization.
- **C)** It encrypts the entire codebase so only AI agents can read it.
- **D)** It acts as a legal copyright waiver transferring all source code ownership to the AI foundation.

---

### Question 2.13 (Module 2.4 — Hierarchical Context: Root vs Subdirectory `.agents/`)
**Indian Lending Context**: In an Indian lending monorepo containing a Python FastAPI credit risk rating scorecard (using scikit-learn / XGBoost for default probability) and a Java Spring Boot loan servicing ledger, the Python service requires Flake8 / Black standards while the Java service mandates Checkstyle and strict financial precision rules.  
**Core Question**: How does the `AGENTS.md` / `.agents/` standard support conflicting sub-project rules in a monorepo?
- **A)** Monorepos are unsupported; the project must be split into separate physical repositories immediately.
- **B)** Through hierarchical context resolution: child directories can maintain their own localized `AGENTS.md` or `.agents/rules/` that override or extend the root project configuration when the agent operates within those specific subdirectories.
- **C)** By running two separate AI vendor models simultaneously in alternating minutes.
- **D)** The AI agent randomly selects which rule set to follow on each prompt.

---

### Question 2.14 (Module 2.4 — Context Window Bloat & Token Degradation)
**Indian Lending Context**: A developer attempts to give an AI agent maximum context by attaching every `.java` file in a 60-file loan origination and underwriting package using `@workspace` or multi-file prompts. The developer notices that the agent begins giving vague, hallucinated answers and ignores explicit lending constraints.  
**Core Question**: What context management best practice prevents this failure mode?
- **A)** Increase the context window to 10 million tokens by subscribing to consumer chat plugins.
- **B)** Curate high-signal, lean context: supply only the target file, relevant interface definitions, and immediate dependencies (e.g., using precise symbol references or `#file` anchors), rather than dumping entire packages into the prompt.
- **C)** Convert all Java source files into single-line minified text before feeding them to the AI.
- **D)** Delete unit test files so that only production code occupies the context window.

---

### Question 2.15 (Module 2.5 — AI-Generated Pull Request Summaries & Auditing)
**Indian Lending Context**: A developer completes a hotfix for an interest calculation bug affecting the **Key Fact Statement (KFS)** Annual Percentage Rate (APR) generation. The institution's release governance process is audited by financial regulators (**RBI IT Examination**). The developer uses Copilot to generate the Pull Request description.  
**Core Question**: What is the developer's professional responsibility regarding the AI-generated PR summary before submitting it for architectural sign-off?
- **A)** Submit the generated PR summary without reading it because AI summaries are certified by Microsoft.
- **B)** Thoroughly review, verify, and augment the PR summary to ensure it explicitly documents the business rationale, ticket ID (Jira), regulatory impact (e.g., RBI DLG KFS disclosure compliance), backward compatibility, and exact verification steps performed, eliminating any generic AI fluff.
- **C)** Delete all text and replace it with a single sentence: *"Fixed KFS APR bug."*
- **D)** Tag the AI model as the primary co-author and legal owner of the change request.

---

### Question 2.16 (Module 2.5 — Conventional Commits & Audit Trails)
**Indian Lending Context**: An AI tool suggests the following commit message for a critical patch updating loan underwriting eligibility rules:  
`commit -m "updated underwriting stuff and fixed a few calculations"`  
**Core Question**: Why is this commit message unacceptable in enterprise Indian lending systems, and what should the developer instruct the AI to generate?
- **A)** The message is acceptable as long as the build passes.
- **B)** It violates auditability standards; the developer should require **Conventional Commits** format with clear scope and regulatory rationale (e.g., `fix(underwriting): enforce max FOIR threshold of 50% for unsecured retail loans [JIRA-5120]`).
- **C)** Commit messages must be encrypted using PGP keys before being pushed to Git.
- **D)** Commit messages must contain the full source code diff embedded within the title line.

---

### Question 2.17 (Module 2.5 — Reviewing AI Diffs for Hidden Regressions)
**Indian Lending Context**: While reviewing an AI-generated Git diff for an Indian retail loan qualification method, a senior reviewer notices this change:
```diff
- if (foirRatio.compareTo(maxAllowedFoir) > 0) {
-     throw new IneligibleBorrowerException("FOIR exceeds credit policy maximum");
- }
+ // Relaxed check for priority lending channel
+ if (foirRatio.compareTo(maxAllowedFoir.add(channelFoirWaiver)) >= 0) {
+     throw new IneligibleBorrowerException("FOIR exceeds credit policy maximum");
+ }
```
The PR author did not notice this change because they accepted the AI's bulk suggestion.  
**Core Question**: What critical flaw is present in this diff, and what review failure occurred?
- **A)** The diff uses tabs instead of spaces, causing compilation failure in Java.
- **B)** The change introduced an unapproved credit risk policy waiver (`channelFoirWaiver`) and flipped a strict inequality (`>`) to greater-than-or-equal (`>=`), allowing boundary FOIR violations; the author failed to perform line-by-line diff validation.
- **C)** The method should have used Python dictionary lookups instead of Java `BigDecimal`.
- **D)** The exception message is not translated into Hindi for multilingual borrower notices.

---

### Question 2.18 (Module 2.6 — Critical Code Review: IEEE 754 Floating-Point Hazards)
**Indian Lending Context**: An AI coding assistant generates the following monthly EMI payment calculation for a digital personal loan:
```java
public double calculateMonthlyEmi(double principal, double annualRate, int tenureMonths) {
    double monthlyRate = annualRate / 12.0 / 100.0;
    return (principal * monthlyRate * Math.pow(1 + monthlyRate, tenureMonths)) 
           / (Math.pow(1 + monthlyRate, tenureMonths) - 1);
}
```
**Core Question**: As an SME conducting a Tier-2 code review, why must this code be immediately rejected for lending production deployment?
- **A)** The method lacks Javadoc annotations, which triggers compiler failure in enterprise Maven.
- **B)** Primitive `double` types introduce binary floating-point representation rounding errors (e.g., `0.1 + 0.2 != 0.3`), resulting in cumulative ledger discrepancies across repayment schedules and KFS disclosures; Indian lending platforms strictly mandate `BigDecimal` with statutory rounding modes (e.g., `HALF_EVEN`).
- **C)** Java math libraries cannot calculate exponential powers greater than 12.
- **D)** The formula should use integer divisions instead of floating-point divisions.

---

### Question 2.19 (Module 2.6 — Dependency Hallucination & Supply Chain Attack)
**Indian Lending Context**: When asked to implement a specialized validation for Indian Permanent Account Numbers (PAN) and CIBIL credit scores, an AI tool suggests:
```javascript
const panValidator = require('india-pan-cibil-enhanced-validator');
```
A junior engineer runs `npm install india-pan-cibil-enhanced-validator`. The package installs without error, but 48 hours later, borrower loan application payloads begin leaking to an external command-and-control server.  
**Core Question**: What attack vector took advantage of the AI tool's output?
- **A)** SQL Injection via HTTP headers.
- **B)** **AI Package Hallucination / Slopsquatting**: An attacker identified frequently hallucinated package names emitted by LLMs, registered a malicious package under that name on npm containing credential-stealing malware, and waited for developers to blindly install it.
- **C)** Man-in-the-middle attack on the developer's wireless keyboard.
- **D)** Cross-Site Scripting (XSS) inside the terminal command prompt.

---

### Question 2.20 (Module 2.6 — Four-Pillar AI Code Review Framework)
**Indian Lending Context**: Your institution's engineering policy mandates that all AI-generated code in lending systems must undergo a structured "Four-Pillar Review" before being merged into release branches.  
**Core Question**: According to the official curriculum (Module 2.6), what are the four critical dimensions every engineer must explicitly evaluate?
- **A)** Speed of generation, Token count, Model temperature, and Prompt length.
- **B)** Correctness, Security, Performance, and Maintainability.
- **C)** Lines of code, Number of comments, Author seniority, and IDE theme.
- **D)** Cloud hosting cost, GPU utilization, RAM usage, and Network bandwidth.

---
*(End of Module 02 — Refer to Document 04 for Master Answer Key & Distractor Rationales)*
