# Simple AI Questionnaire: Answer Key & Explanations
## Everyday AI for Enterprise Lending Coders (Questions 1 – 30)

---

### Quick Answer Sheet

| Question | Answer | Question | Answer | Question | Answer |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **1** | **B** | **11** | **C** | **21** | **B** |
| **2** | **B** | **12** | **B** | **22** | **B** |
| **3** | **B** | **13** | **B** | **23** | **B** |
| **4** | **B** | **14** | **B** | **24** | **B** |
| **5** | **B** | **15** | **B** | **25** | **B** |
| **6** | **B** | **16** | **A** | **26** | **B** |
| **7** | **B** | **17** | **B** | **27** | **B** |
| **8** | **B** | **18** | **B** | **28** | **B** |
| **9** | **B** | **19** | **B** | **29** | **B** |
| **10** | **A** | **20** | **A** | **30** | **B** |

---

### Explanations

#### 1. How AI Generates Code
- **Answer: B**
- **Why**: LLMs are statistical language models that predict the most likely next tokens based on patterns learned from billions of lines of code. They do not compile or run code internally.

#### 2. AI Hallucination
- **Answer: B**
- **Why**: Hallucination occurs when an AI generates syntactically plausible but completely non-existent library methods, APIs, or classes. Always verify unfamiliar methods against official documentation.

#### 3. Temperature Setting
- **Answer: B**
- **Why**: Lower temperatures (0.0 to 0.2) reduce randomness and make the model choose the highest-probability, most standard completions, which is ideal for coding.

#### 4. Context Window
- **Answer: B**
- **Why**: The context window is the memory capacity of the LLM for a given prompt and conversation. Once exceeded, earlier information is pushed out and forgotten.

#### 5. Providing Too Much Code in a Prompt
- **Answer: B**
- **Why**: Stuffing too many files into the context window causes attention dilution and the "Lost in the Middle" effect, where the model misses details located in the middle of long texts.

#### 6. Copilot Ask Mode vs Agent Mode
- **Answer: B**
- **Why**: Ask Mode is conversational Q&A. Agent Mode uses tool-calling loops to inspect files, edit across the project, and run terminal build/test commands autonomously.

#### 7. Claude Code CLI
- **Answer: B**
- **Why**: Claude Code is Anthropic's agentic CLI tool that operates directly inside your terminal, allowing it to navigate directories, run bash scripts, view git diffs, and edit code.

#### 8. Google Antigravity
- **Answer: B**
- **Why**: Antigravity is Google's agentic IDE built to run Gemini and other foundation models natively with workspace context, background task handling, and interactive artifacts.

#### 9. Antigravity Artifacts
- **Answer: B**
- **Why**: Artifacts are structured markdown documents created in the brain directory, allowing developers to review, edit, and approve architectural plans before code is changed.

#### 10. Model Context Protocol (MCP)
- **Answer: A**
- **Why**: MCP is an open standard that lets AI assistants connect securely to local or remote tools, databases, and schema servers to fetch real-time context.

#### 11. Writing Good Prompts
- **Answer: C**
- **Why**: High-quality prompts provide the programming language/framework, inputs, outputs, specific business rules, and error handling expectations.

#### 12. Few-Shot Prompting
- **Answer: B**
- **Why**: Showing 1 or 2 concrete input-output examples helps the AI understand custom formats, naming patterns, or edge cases much better than text descriptions alone.

#### 13. Positive Instructions vs Negative Constraints
- **Answer: B**
- **Why**: Saying "don't use X" often makes the LLM pay attention to "X". Stating positively what tool or library to use (e.g., "Use `java.time.LocalDate`") produces more reliable results.

#### 14. Repository Instructions for Copilot
- **Answer: B**
- **Why**: Placing a `.github/copilot-instructions.md` file in the repo root ensures that Copilot Chat automatically includes those project rules in every query.

#### 15. CLAUDE.md Memory File
- **Answer: B**
- **Why**: `CLAUDE.md` is automatically read by Claude Code at startup, providing persistent instructions for common build commands, test patterns, and code guidelines.

#### 16. Providing Context with `#file`
- **Answer: A**
- **Why**: Using `#file:FileName` in Copilot Chat or keeping the file open in an active tab grounds the AI with the exact class interface and method signatures.

#### 17. Debugging with `/explain` and `/fix`
- **Answer: B**
- **Why**: Rushing straight to `/fix` often results in superficial patches. First using `/explain` helps you understand the root cause before applying a targeted fix.

#### 18. Plan → Execute → Verify Loop
- **Answer: B**
- **Why**: Safe agentic refactoring follows three steps: first create a plan, execute changes in small isolated increments, and verify with automated tests after each step.

#### 19. Task Decomposition
- **Answer: B**
- **Why**: Asking an AI to generate an entire system at once leads to monolithic, buggy code. Decomposing tasks into smaller layers produces clean, modular software.

#### 20. AGENTS.md Open Standard
- **Answer: A**
- **Why**: `AGENTS.md` is an open standard promoted by the Linux Foundation to document build commands and coding standards for all AI agents in a vendor-neutral way.

#### 21. Financial Precision with `BigDecimal`
- **Answer: B**
- **Why**: Binary floating-point numbers (`float`, `double`) cannot accurately represent base-10 decimals like $0.10$. Financial and lending applications must use `BigDecimal`.

#### 22. Unit Test Edge Cases
- **Answer: B**
- **Why**: AI naturally generates happy-path tests. Developers must explicitly instruct the AI to generate boundary tests (zero balance, negative interest, large amounts, leap years).

#### 23. Idempotency in Disbursement APIs
- **Answer: B**
- **Why**: If a network timeout occurs and a request is retried with the same idempotency key, the system must not disburse funds twice. Tests must verify this behavior.

#### 24. Protecting Sensitive Data
- **Answer: B**
- **Why**: Never paste real customer PII (names, SSNs, credit scores), database passwords, or production API keys into AI tools to prevent data leaks.

#### 25. Generating Synthetic Test Data
- **Answer: B**
- **Why**: AI is excellent at creating realistic synthetic (mock) test records, eliminating the need to expose real customer databases for testing.

#### 26. Reviewing AI-Generated Documentation
- **Answer: B**
- **Why**: AI often outputs repetitive docstrings that just parrot the method name. Ensure docs explain *why* the method exists, its error codes, and business constraints.

#### 27. Reviewing AI Git Diffs
- **Answer: B**
- **Why**: Always review AI-generated diffs line-by-line. AI can subtly flip comparison operators (`>` to `>=`) or loosen validation rules without you noticing.

#### 28. AI Package Hallucination (Slopsquatting)
- **Answer: B**
- **Why**: Attackers watch for fake package names commonly hallucinated by AI and publish malicious packages with those names. Always check package legitimacy before installing.

#### 29. The Four-Pillar Review Framework
- **Answer: B**
- **Why**: The Four Pillars of AI code review are **Correctness** (does it work?), **Security** (is it safe?), **Performance** (is it fast?), and **Maintainability** (is it clean?).

#### 30. Why Lines of Code (LOC) is Misleading
- **Answer: B**
- **Why**: AI can generate hundreds of lines of verbose boilerplate in seconds. True engineering productivity is measured by working software delivery and system stability, not line count.
