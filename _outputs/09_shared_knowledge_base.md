# Shared Knowledge Base — Cross-Track Resource Pack

> **Purpose**: Common reference materials accessible by all four tracks. These are NOT courses — they are curated reference resources.  
> **Policy**: Zero overlap with track-specific courses. These supplement, not duplicate.

---

## 1. AI Glossary (50+ Terms)

### Core Concepts
| Term | Definition | Relevance |
|------|-----------|-----------|
| **Artificial Intelligence (AI)** | Computer systems that can perform tasks typically requiring human intelligence | All tracks |
| **Machine Learning (ML)** | Subset of AI where systems learn from data without explicit programming | All tracks |
| **Deep Learning (DL)** | ML using neural networks with many layers | Dev, QA, AI Dev |
| **Large Language Model (LLM)** | AI model trained on vast text data to generate and understand language | All tracks |
| **Generative AI (GenAI)** | AI that creates new content (text, images, code, audio) | All tracks |
| **Natural Language Processing (NLP)** | AI that understands and generates human language | All tracks |
| **Computer Vision** | AI that interprets visual information from images/videos | QA, AI Dev |
| **Reinforcement Learning (RL)** | ML where agents learn by trial and error with rewards | AI Dev |

### Model & Training
| Term | Definition | Relevance |
|------|-----------|-----------|
| **Training** | Process of teaching a model using data | QA, BA, AI Dev |
| **Inference** | Using a trained model to make predictions | All tracks |
| **Fine-Tuning** | Adapting a pre-trained model to a specific task | AI Dev |
| **LoRA (Low-Rank Adaptation)** | Parameter-efficient fine-tuning technique | AI Dev |
| **QLoRA** | Quantised LoRA — fine-tuning with reduced memory | AI Dev |
| **PEFT** | Parameter-Efficient Fine-Tuning — umbrella term | AI Dev |
| **Transfer Learning** | Applying knowledge from one task to another | AI Dev |
| **Pre-trained Model** | Model trained on large datasets, ready for fine-tuning or use | All tracks |
| **Foundation Model** | Large pre-trained model (e.g., GPT, Claude, Gemini) | All tracks |
| **Hyperparameters** | Configuration settings for model training | AI Dev |
| **Epoch** | One complete pass through the training dataset | AI Dev |
| **Overfitting** | Model memorises training data, performs poorly on new data | QA, AI Dev |

### LLM-Specific
| Term | Definition | Relevance |
|------|-----------|-----------|
| **Token** | Smallest unit of text processed by an LLM (~0.75 words) | All tracks |
| **Context Window** | Maximum tokens an LLM can process at once | Dev, AI Dev |
| **Temperature** | Controls randomness in LLM outputs (0=deterministic, 1=creative) | Dev, QA, AI Dev |
| **Top-P / Top-K** | Sampling strategies that control output diversity | Dev, AI Dev |
| **Hallucination** | When an LLM generates false or fabricated information | All tracks |
| **System Prompt** | Instructions that define LLM behaviour for a session | Dev, AI Dev |
| **Function Calling** | LLM's ability to invoke external tools/APIs | AI Dev |
| **Structured Output** | Forcing LLM to respond in a specific format (JSON, etc.) | AI Dev |
| **Prompt Injection** | Adversarial input that manipulates LLM behaviour | QA, AI Dev |
| **Jailbreaking** | Bypassing LLM safety guardrails | QA, AI Dev |

### RAG & Architecture
| Term | Definition | Relevance |
|------|-----------|-----------|
| **RAG (Retrieval-Augmented Generation)** | Enhancing LLM with external knowledge retrieval | QA, AI Dev |
| **Vector Database** | Database optimised for storing and searching embeddings | AI Dev |
| **Embedding** | Numerical representation of text for similarity search | AI Dev |
| **Chunking** | Splitting documents into smaller pieces for RAG | AI Dev |
| **Reranking** | Re-ordering search results for relevance | AI Dev |

### AI Agents
| Term | Definition | Relevance |
|------|-----------|-----------|
| **AI Agent** | AI system that autonomously performs tasks using tools | Dev, AI Dev |
| **Agentic AI** | AI that plans, executes, and verifies tasks autonomously | Dev, AI Dev |
| **Tool Use** | Agent's ability to call external functions/APIs | Dev, AI Dev |
| **Chain** | Sequence of LLM calls and actions | AI Dev |
| **Memory** | Agent's ability to retain information across interactions | Dev, AI Dev |
| **MCP (Model Context Protocol)** | Standard for connecting AI agents to external tools | Dev, AI Dev |
| **AGENTS.md / CLAUDE.md** | Context files that configure AI coding assistants | Dev |
| **Plan Mode** | AI agent creates execution plan before acting | Dev |

### MLOps & Production
| Term | Definition | Relevance |
|------|-----------|-----------|
| **MLOps** | Practices for deploying and maintaining ML in production | AI Dev |
| **Model Registry** | Repository for versioning and managing ML models | AI Dev |
| **Data Drift** | Change in data distribution over time | QA, AI Dev |
| **Concept Drift** | Change in the relationship between input and output | QA, AI Dev |
| **A/B Testing** | Comparing two versions to determine which performs better | QA, BA, AI Dev |
| **Model Card** | Documentation of a model's capabilities and limitations | BA, AI Dev |

### Evaluation Metrics
| Term | Definition | Relevance |
|------|-----------|-----------|
| **Precision** | % of positive predictions that are correct | QA, AI Dev |
| **Recall** | % of actual positives correctly identified | QA, AI Dev |
| **F1 Score** | Harmonic mean of precision and recall | QA, AI Dev |
| **AUC-ROC** | Area Under the Receiver Operating Characteristic Curve | QA, AI Dev |
| **BLEU** | Metric for evaluating text generation quality | QA, AI Dev |
| **ROUGE** | Metric for evaluating text summarisation quality | QA, AI Dev |
| **Perplexity** | How well a model predicts a sample (lower = better) | AI Dev |

### Ethics & Governance
| Term | Definition | Relevance |
|------|-----------|-----------|
| **Responsible AI** | Developing AI that is fair, transparent, and accountable | All tracks |
| **Bias** | Systematic unfairness in AI outputs | All tracks |
| **Explainability** | Ability to understand why an AI made a decision | BA, AI Dev |
| **EU AI Act** | European regulation classifying AI by risk level | BA |
| **NIST AI RMF** | US framework for managing AI risks | BA |

---

## 2. Tool Setup Guide

### For All Tracks

#### Python & Jupyter (Required for Tracks B, D; Recommended for A)
1. **Install Python 3.11+**: https://www.python.org/downloads/
2. **Install VS Code**: https://code.visualstudio.com/
3. **Install Jupyter Extension** for VS Code
4. **Create virtual environment**: `python -m venv ai-learning`
5. **Install common packages**: `pip install numpy pandas matplotlib scikit-learn jupyter`

#### ChatGPT Access (All Tracks)
1. **Create account**: https://chat.openai.com/
2. **Free tier**: GPT-4o mini available
3. **Plus subscription** ($20/month): GPT-4o, advanced features
4. **Usage tip**: Use for brainstorming, drafting, and analysis — always verify outputs

#### Claude Access (All Tracks)
1. **Create account**: https://claude.ai/
2. **Free tier**: Claude Sonnet available
3. **Pro subscription** ($20/month): Claude Opus, extended usage
4. **Usage tip**: Excellent for long-form analysis, code review, and nuanced reasoning

### For Track A (Developers)

#### GitHub Copilot
1. **Sign up**: https://github.com/features/copilot
2. **Plans**: Free tier (limited), Individual ($10/mo), Business ($19/user/mo)
3. **Install VS Code Extension**: Search "GitHub Copilot" in extensions marketplace
4. **Enable features**: Agent Mode, Chat, Workspace Agents
5. **Configure**: Set up custom instructions via `.github/copilot-instructions.md`

#### Claude Code (Terminal)
1. **Install**: 
   - macOS/Linux/WSL: `curl -fsSL https://claude.ai/install.sh | bash`
   - Windows PowerShell: `irm https://claude.ai/install.ps1 | iex`
2. **Authenticate**: Requires Claude Pro/Team/Enterprise subscription or API key
3. **First run**: Navigate to project directory, run `claude`
4. **Configure**: Create `CLAUDE.md` in project root with context and conventions

#### Google Antigravity IDE
1. **Access**: Google's standalone agentic IDE (macOS/Windows/Linux) — download from https://antigravity.google/
2. **Setup**: Follow the official docs at https://antigravity.google/docs/home (or the getting-started codelab)
3. **Configure**: Add an `AGENTS.md` for project context; connect tools via MCP
4. **Key features**: Agent Manager, planning, browser tools, multi-agent orchestration (runs Gemini and other models — *not* a Claude/Anthropic product)

### For Track D (AI/ML Developers)

#### PyTorch
```bash
pip install torch torchvision torchaudio
```

#### Hugging Face Transformers
```bash
pip install transformers datasets tokenizers accelerate peft trl
```

#### LangChain & LangGraph
```bash
pip install langchain langchain-openai langchain-community langgraph
```

#### MLflow
```bash
pip install mlflow
mlflow ui  # Start the tracking UI
```

---

## 3. Agentic AI Tools Quick-Reference Card

| Feature | GitHub Copilot | Claude Code | Antigravity IDE | Cursor | Windsurf |
|---------|---------------|-------------|-----------------|--------|----------|
| **Type** | IDE extension | Terminal agent | IDE agent | AI-first IDE | AI-first IDE |
| **Integration** | VS Code, JetBrains, Neovim | Terminal (any project) | VS Code-based | Standalone IDE | Standalone IDE |
| **Code Completion** | ✅ Inline + chat | ❌ (agentic, not inline) | ✅ Inline + agentic | ✅ Inline + chat | ✅ Inline + chat |
| **Agent Mode** | ✅ Plan + Execute | ✅ Full agentic | ✅ Full agentic + planning | ✅ Composer mode | ✅ Cascade mode |
| **Multi-File Edits** | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Terminal Access** | ✅ (via agent) | ✅ (native) | ✅ | ✅ | ✅ |
| **Browser Tools** | ❌ | ❌ | ✅ | ❌ | ❌ |
| **Context Protocol** | MCP | MCP | MCP / AGENTS.md | Custom | Custom |
| **Model Options** | GPT-4o, Claude, Gemini | Claude models | Gemini 3 (+ Claude, GPT) | GPT-4o, Claude | GPT-4o, Claude |
| **Vendor** | GitHub / Microsoft | Anthropic | **Google** | Anysphere | Codeium |
| **Pricing** | Free / $10 / $19 per mo | Claude subscription req | Free (public preview) | Free / $20 per mo | Free / $15 per mo |
| **Best For** | Broad IDE integration | Large codebase work | Complex multi-tool tasks | All-in-one AI IDE | Collaborative coding |
| **Enterprise** | ✅ SOC 2, SSO | ✅ Enterprise plan | ✅ Enterprise features | ✅ Business plan | ✅ Pro plan |

**Recommendation for this programme**: Start with GitHub Copilot (broadest support, most tutorials) + Claude Code (best for agentic terminal workflows). Add Antigravity for advanced users comfortable with planning workflows.

---

## 4. Ethics & Responsible AI Reading List

### Articles & Papers (Accessible to All Levels)
1. **"On the Dangers of Stochastic Parrots"** — Bender et al. (2021)
   - Foundational paper on LLM risks and biases
   - https://dl.acm.org/doi/10.1145/3442188.3445922

2. **"AI Ethics: A Long History and a Recent Burst of Activity"** — Google AI Blog
   - Accessible overview of AI ethics evolution
   - https://ai.google/responsibility/

3. **"Responsible AI Practices"** — Google AI
   - Practical guidelines for responsible AI development
   - https://ai.google/responsibility/responsible-ai-practices/

4. **"NIST AI Risk Management Framework (AI RMF 1.0)"** — NIST
   - The US standard for AI risk management
   - https://www.nist.gov/artificial-intelligence/executive-order-safe-secure-and-trustworthy-ai

5. **"EU AI Act: A Quick Guide"** — European Commission
   - Official summary of the EU AI regulation
   - https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai

6. **"Model Cards for Model Reporting"** — Mitchell et al. (2019)
   - How to document AI model capabilities and limitations
   - https://arxiv.org/abs/1810.03993

7. **"Artificial Intelligence Incident Database"** — AIID
   - Real-world database of AI failures and incidents
   - https://incidentdatabase.ai/

---

## 5. Weekly AI News Digest Template

### Template for Team AI Newsletter

```
═══════════════════════════════════════════
📰 [Team Name] AI Weekly — [Date]
═══════════════════════════════════════════

🔧 TOOLS & UPDATES
• [Tool name] released [feature] — Impact: [who cares]
• [Platform] updated to version X — What changed: [summary]

📚 LEARNING SPOTLIGHT
• [Team member] completed [Track X — Tier Y] — Key takeaway: [one sentence]
• Recommended resource this week: [link + why]

🧪 EXPERIMENTS & WINS
• [Team member] used [AI tool] to [achieve something] — Time saved: [X hours]
• [Project] integrated [AI feature] — Result: [measurable outcome]

⚠️ WATCH LIST
• [Risk/concern] identified in [AI tool/practice] — Action: [what to do]
• [Industry news] that affects our AI strategy — Impact: [summary]

💬 DISCUSSION QUESTION
[Open-ended question about AI practices for team discussion]

═══════════════════════════════════════════
Next week's curator: [Name]
═══════════════════════════════════════════
```

### Rotation Schedule
- Each team member takes turns curating the weekly digest
- Spend 30 minutes max collecting items throughout the week
- Share in the team's Slack/Teams channel every Monday morning
