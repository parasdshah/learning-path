# Simple AI Questionnaire for Software Developers
## Everyday AI for Enterprise Lending Coders (30 Questions)

---

### Part 1: AI Basics & Daily Tools (Questions 1 – 10)

#### 1. How does an AI code assistant (like Copilot or Claude) generate code?
- **A)** It executes a hidden compiler and runs the code to see if it works.
- **B)** It predicts the most probable next tokens (words/symbols) based on patterns in its training data.
- **C)** It searches Google and copies the top result from Stack Overflow.
- **D)** It converts your prompt into SQL queries that run against a central library.

#### 2. What is an AI "hallucination" in coding?
- **A)** When the AI crashes the IDE due to low memory.
- **B)** When the AI invents a method, class, or library that does not actually exist.
- **C)** When the AI formats your code using tabs instead of spaces.
- **D)** When the AI takes more than 10 seconds to generate an answer.

#### 3. If you want the AI assistant to give more consistent and predictable code suggestions, what should you do with the temperature setting?
- **A)** Increase the temperature (closer to 1.0 or higher).
- **B)** Lower the temperature (closer to 0.0).
- **C)** Keep the temperature constantly fluctuating.
- **D)** Temperature only affects images, not code.

#### 4. What is an AI model's "context window"?
- **A)** The pop-up chat box window in your IDE.
- **B)** The maximum amount of text (tokens) the model can read and remember in a single conversation.
- **C)** The list of files currently open in your editor tabs.
- **D)** The operating system window where your terminal runs.

#### 5. What happens when you provide too much code in a single prompt (e.g., pasting 10 large files)?
- **A)** The model gets smarter and learns your entire architecture permanently.
- **B)** The model may lose track of details, ignore instructions, or suffer from "Lost in the Middle" degradation.
- **C)** Your IDE will permanently corrupt the local files.
- **D)** The model will automatically split your project into microservices.

#### 6. In GitHub Copilot, what is the main difference between "Ask Mode" and "Agent Mode"?
- **A)** Ask Mode writes unit tests, while Agent Mode only writes documentation.
- **B)** Ask Mode is for chatting and asking questions, while Agent Mode can autonomously edit files and run terminal commands.
- **C)** Ask Mode is paid, while Agent Mode is completely free.
- **D)** Ask Mode only works in Python, while Agent Mode works in Java.

#### 7. What is Claude Code?
- **A)** A web-based drag-and-drop website builder.
- **B)** A terminal-based agentic tool that can read files, run bash commands, execute tests, and edit code autonomously.
- **C)** A VS Code theme with dark mode colors.
- **D)** A database query optimizer for Oracle.

#### 8. What is Google Antigravity?
- **A)** A physical laptop stand designed by Google.
- **B)** Google's agentic IDE designed to run Gemini and other models with built-in agent workflows and project context.
- **C)** An Anthropic plugin that requires a paid Claude Pro subscription.
- **D)** A command-line tool used only for managing Google Drive files.

#### 9. In Google Antigravity, what are "Artifacts"?
- **A)** Old compiled `.jar` and `.class` files from previous builds.
- **B)** Interactive markdown documents where the agent and developer can review, inspect, and approve plans before code changes are made.
- **C)** Error logs that are automatically sent to Google support.
- **D)** Deleted files saved in the trash bin.

#### 10. What does the Model Context Protocol (MCP) allow AI coding assistants to do?
- **A)** Directly connect to external tools, databases, and local documentation servers using a standard protocol.
- **B)** Download pirated software libraries without license warnings.
- **C)** Increase your computer's CPU clock speed during compilation.
- **D)** Automatically pay for cloud server hosting fees.

---

### Part 2: Daily Coding, Prompting & Debugging (Questions 11 – 20)

#### 11. Which prompt will get the best code when writing a loan eligibility check?
- **A)** *"Write loan code."*
- **B)** *"Please make a function that checks loan eligibility and make sure it has no bugs."*
- **C)** *"In Java Spring Boot, write a `checkEligibility` method that takes `LoanApplication` (income, creditScore, requestedAmount). Return `true` if creditScore >= 700 and requestedAmount <= income * 3. Handle null inputs."*
- **D)** *"CRITICAL EMERGENCY: WRITE LOAN CODE NOW!!!"*

#### 12. What is "few-shot prompting" for developers?
- **A)** Asking the AI the same question three times in a row.
- **B)** Giving the AI 1 or 2 concrete examples of inputs and expected outputs in your prompt before asking it to write code.
- **C)** Prompting the AI only when you have fewer than 5 files open.
- **D)** Forcing the AI to answer in under 3 seconds.

#### 13. You want the AI to avoid using deprecated date libraries. Which prompt works best?
- **A)** *"Do NOT use Date or Calendar. NEVER use old dates!"*
- **B)** *"Use `java.time.LocalDate` and `DateTimeFormatter` for all date fields."*
- **C)** *"Don't you dare touch anything created before 2020."*
- **D)** *"Write date code without using the letter D."*

#### 14. Where can you save project-wide instructions so GitHub Copilot always remembers them?
- **A)** In an environment variable on your computer.
- **B)** In a file named `.github/copilot-instructions.md` in the repository root.
- **C)** In a text file on your desktop.
- **D)** In a Slack message to your team.

#### 15. In Claude Code, what is the purpose of the `CLAUDE.md` file?
- **A)** It stores the developer's personal login password.
- **B)** It stores project memory (common build commands, test instructions, and coding standards) that Claude Code reads automatically.
- **C)** It is a license file required to run the CLI.
- **D)** It converts Python code into Java automatically.

#### 16. In VS Code Copilot Chat, how do you make sure the AI knows about an existing class `LoanAccount.java`?
- **A)** Type `#file:LoanAccount.java` in the chat or keep the file open in an active tab.
- **B)** Copy the entire `.class` compiled bytecode into the chat prompt.
- **C)** Rename the file to `Main.java`.
- **D)** Close VS Code and reopen it.

#### 17. When fixing a bug with Copilot Chat, what is the best workflow?
- **A)** Run `/fix` immediately on the entire project without reading the error.
- **B)** First use `/explain` with the error log to understand the root cause, then use `/fix` for a targeted code change.
- **C)** Ask the AI to rewrite the entire project in a different language.
- **D)** Delete the file and prompt the AI to rewrite it from scratch.

#### 18. When refactoring a complex loan calculation service, what is the recommended agentic loop?
- **A)** **Code → Push → Pray**: Generate all code at once and push to main.
- **B)** **Plan → Execute → Verify**: Plan the steps first, execute small changes, and run tests after each step.
- **C)** **Chat → Copy → Paste**: Copy snippets from chat without testing.
- **D)** **Prompt → Retry → Give up**: Retry 10 times until it looks right.

#### 19. Why should you avoid asking an AI agent to build a huge feature in a single prompt?
- **A)** Large prompts overheat the developer's laptop battery.
- **B)** The agent is more likely to miss requirements, generate shallow code, or produce hard-to-debug monolithic files.
- **C)** AI models charge a penalty fee for prompts over 50 words.
- **D)** IDEs do not allow files longer than 100 lines.

#### 20. What is `AGENTS.md`?
- **A)** An open, standard markdown file in a repository that documents coding guidelines and build steps for any AI agent.
- **B)** A list of secret usernames allowed to use AI in the company.
- **C)** A script that automatically installs antivirus software.
- **D)** A legal copyright agreement transferring code to an AI vendor.

---

### Part 3: Testing, Code Review & Safe AI Usage (Questions 21 – 30)

#### 21. When reviewing AI-generated code for loan calculations (such as interest or monthly EMI), why should you reject `double` or `float`?
- **A)** `double` and `float` run too slowly on modern 64-bit processors.
- **B)** Binary floating-point types cause rounding inaccuracies (e.g. `0.1 + 0.2 != 0.3`); financial code must use `BigDecimal`.
- **C)** Java does not allow `double` variables in Spring Boot applications.
- **D)** Floating-point numbers cannot be stored in SQL databases.

#### 22. When asking AI to generate unit tests for a loan repayment function, what should you specifically ask for?
- **A)** Only positive tests that always pass.
- **B)** Boundary conditions and edge cases (e.g., zero payment, negative amounts, maximum loan limits, leap years).
- **C)** Tests with no assertions so the build runs faster.
- **D)** Tests written in plain English instead of code.

#### 23. What is an "idempotent" loan disbursement API, and why should AI test it?
- **A)** An API that runs only once per year.
- **B)** An API where sending the same request twice with the same key will NOT disburse money twice.
- **C)** An API that does not require an internet connection.
- **D)** An API that only accepts cryptocurrency payments.

#### 24. What should you NEVER include in an AI prompt or paste into an AI chat?
- **A)** Method names and interface definitions.
- **B)** Real customer Personally Identifiable Information (PII), live database passwords, or production API keys.
- **C)** Error stack traces with sensitive data masked out.
- **D)** Unit test sample code.

#### 25. When testing a new loan origination feature, how should you use AI to create test data?
- **A)** Ask the AI to scrape your production database for real customer applications.
- **B)** Ask the AI to generate realistic synthetic (fake) test data with dummy names and mock account numbers.
- **C)** Use your own personal credit card and banking details in test scripts.
- **D)** AI cannot generate test data.

#### 26. What is a common flaw in AI-generated documentation (like Javadoc or Swagger)?
- **A)** It writes in poetic rhymes instead of plain English.
- **B)** It writes trivial summaries that just repeat the method name (e.g., `getLoan(): gets the loan`) while missing business rules, error codes, and edge cases.
- **C)** It automatically deletes existing code comments.
- **D)** It makes the compiled `.jar` file 10 times larger.

#### 27. When reviewing a Git diff created by an AI tool, what should you be careful to check?
- **A)** Whether the AI changed the font size of the editor.
- **B)** That the AI didn't subtly change business logic or boundary conditions (like changing `>` to `>=` or relaxing validation checks).
- **C)** Whether the commit was made during business hours.
- **D)** That the AI used emojis in every method.

#### 28. What is "AI Package Hallucination" (or slopsquatting)?
- **A)** When an AI tool installs too many games on your computer.
- **B)** When an AI hallucinates a non-existent package name, and an attacker creates a malicious package with that exact name on npm or PyPI.
- **C)** When your npm cache runs out of disk space.
- **D)** When the AI refuses to write JavaScript code.

#### 29. What are the "Four Pillars" you should check when reviewing any AI-generated code?
- **A)** Speed, Token Count, Prompt Length, and Temperature.
- **B)** Correctness, Security, Performance, and Maintainability.
- **C)** File Size, Author Age, IDE Theme, and Font Family.
- **D)** Cloud Cost, RAM Usage, Number of Comments, and Typing Speed.

#### 30. Why is measuring developer productivity by "Lines of Code (LOC) generated by AI" a bad idea?
- **A)** Modern compilers cannot count lines of code.
- **B)** AI makes it easy to generate bloated, unnecessary boilerplate code that increases maintenance headaches and bugs without delivering real value.
- **C)** DORA guidelines state that developers should only be judged on their typing speed.
- **D)** Generative AI code does not have lines of code.

---
*(End of Questionnaire — See answer_key.md for answers and explanations)*
