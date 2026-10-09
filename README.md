# Awesome-AI-Redteam

<p align="left">
  <a href="https://github.com/Threekiii/Awesome-AI-Redteam">
    <img src="https://badgen.net/github/stars/Threekiii/Awesome-AI-Redteam?color=yellow&icon=github" alt="stars">
  </a>
  <a href="https://github.com/Threekiii/Awesome-AI-Redteam">
    <img src="https://badgen.net/github/forks/Threekiii/Awesome-AI-Redteam?color=blue&icon=github" alt="forks">
  </a>
  <a href="https://github.com/Threekiii/Awesome-AI-Redteam">
    <img src="https://badgen.net/github/last-commit/Threekiii/Awesome-AI-Redteam?color=green" alt="last-commit">
  </a>
</p>

**❗【免责声明】本项目所涉及的技术、思路和工具仅供学习，任何人不得将其用于非法用途和盈利，不得将其用于非授权渗透测试，否则后果自行承担，与本项目无关。 使用本项目前请先阅读 [法律法规](https://github.com/Threekiii/Awesome-Laws)。**

_Disclaimer: The technologies, concepts, and tools provided in this Git repository are intended for educational and research purposes only. Any use for illegal activities, unauthorized penetration testing, or commercial purposes is strictly prohibited. Please read the [Awesome-Laws](https://github.com/Threekiii/Awesome-Laws) before using this repository._

📖 一个 AI 攻防知识库。_A knowledge base for AI security._

👍 means recommend 推荐使用

- [开源资源 _Open-Source Resources_](#%E5%BC%80%E6%BA%90%E8%B5%84%E6%BA%90-open-source-resources)
	- [资源清单 _Resource Collections_](#%E8%B5%84%E6%BA%90%E6%B8%85%E5%8D%95-resource-collections)
	- [学术论文 _Papers_](#%E5%AD%A6%E6%9C%AF%E8%AE%BA%E6%96%87-papers)
	- [实验环境 _Lab Environments_](#%E5%AE%9E%E9%AA%8C%E7%8E%AF%E5%A2%83-lab-environments)
	- [提示词 _Prompts_](#%E6%8F%90%E7%A4%BA%E8%AF%8D-prompts)
	- [编排框架 _Orchestration Frameworks_](#%E7%BC%96%E6%8E%92%E6%A1%86%E6%9E%B6-orchestration-frameworks)
	- [大模型部署与工具链 _Deployment & Toolchain_](#%E5%A4%A7%E6%A8%A1%E5%9E%8B%E9%83%A8%E7%BD%B2%E4%B8%8E%E5%B7%A5%E5%85%B7%E9%93%BE-deployment--toolchain)
	- [Agent Skills](#agent-skills)
- [治理与风险管理 _Governance & Risk Management_](#%E6%B2%BB%E7%90%86%E4%B8%8E%E9%A3%8E%E9%99%A9%E7%AE%A1%E7%90%86-governance--risk-management)
	- [框架 _Frameworks_](#%E6%A1%86%E6%9E%B6-frameworks)
	- [标准与验证 _Standards & Verification_](#%E6%A0%87%E5%87%86%E4%B8%8E%E9%AA%8C%E8%AF%81-standards--verification)
	- [术语体系与数据库 _Taxonomies & Databases_](#%E6%9C%AF%E8%AF%AD%E4%BD%93%E7%B3%BB%E4%B8%8E%E6%95%B0%E6%8D%AE%E5%BA%93-taxonomies--databases)
	- [清单与指南 _Checklists & Guidance_](#%E6%B8%85%E5%8D%95%E4%B8%8E%E6%8C%87%E5%8D%97-checklists--guidance)
- [进攻性安全 _Red Teaming and Offensive Security_](#%E8%BF%9B%E6%94%BB%E6%80%A7%E5%AE%89%E5%85%A8-red-teaming-and-offensive-security)
	- [LLM & Agent 对抗性安全 _LLM & Agent Adversarial Security_](#llm--agent-%E5%AF%B9%E6%8A%97%E6%80%A7%E5%AE%89%E5%85%A8-llm--agent-adversarial-security)
		- [综合红队框架 _Comprehensive Red Teaming Frameworks_](#%E7%BB%BC%E5%90%88%E7%BA%A2%E9%98%9F%E6%A1%86%E6%9E%B6-comprehensive-red-teaming-frameworks)
		- [越狱与对抗测试 _Jailbreak & Adversarial Testing_](#%E8%B6%8A%E7%8B%B1%E4%B8%8E%E5%AF%B9%E6%8A%97%E6%B5%8B%E8%AF%95-jailbreak--adversarial-testing)
		- [Prompt 注入 _Prompt Injection_](#prompt-%E6%B3%A8%E5%85%A5-prompt-injection)
		- [Agent 安全 _Agent Security_](#agent-%E5%AE%89%E5%85%A8-agent-security)
	- [AI 赋能攻击性安全 _AI-Assisted Offensive Security_](#ai-%E8%B5%8B%E8%83%BD%E6%94%BB%E5%87%BB%E6%80%A7%E5%AE%89%E5%85%A8-ai-assisted-offensive-security)
		- [渗透测试 _Penetration Agents_](#%E6%B8%97%E9%80%8F%E6%B5%8B%E8%AF%95-penetration-agents)
		- [漏洞研究 _Vulnerability Research_](#%E6%BC%8F%E6%B4%9E%E7%A0%94%E7%A9%B6-vulnerability-research)
		- [CTF _Capture the Flag_](#ctf-capture-the-flag)
		- [MCP 集成 _MCP Security Integration_](#mcp-%E9%9B%86%E6%88%90-mcp-security-integration)
- [防御性安全 _Blue Teaming and Defensive Security_](#%E9%98%B2%E5%BE%A1%E6%80%A7%E5%AE%89%E5%85%A8-blue-teaming-and-defensive-security)
	- [安全围栏 _Guardrails_](#%E5%AE%89%E5%85%A8%E5%9B%B4%E6%A0%8F-guardrails)
	- [运行时安全与沙箱 _Runtime Security & Sandboxing_](#%E8%BF%90%E8%A1%8C%E6%97%B6%E5%AE%89%E5%85%A8%E4%B8%8E%E6%B2%99%E7%AE%B1-runtime-security--sandboxing)
	- [MCP 安全 _MCP Security_](#mcp-%E5%AE%89%E5%85%A8-mcp-security)
	- [模型与制品扫描 _Model & Artifact Scanning_](#%E6%A8%A1%E5%9E%8B%E4%B8%8E%E5%88%B6%E5%93%81%E6%89%AB%E6%8F%8F-model--artifact-scanning)
	- [AI 赋能防御性安全 _AI-Assisted Defensive Security_](#ai-%E8%B5%8B%E8%83%BD%E9%98%B2%E5%BE%A1%E6%80%A7%E5%AE%89%E5%85%A8-ai-assisted-defensive-security)
- [评测基准 _Benchmarks & Evaluations_](#%E8%AF%84%E6%B5%8B%E5%9F%BA%E5%87%86-benchmarks--evaluations)
	- [模型榜单 _Model Rankings_](#%E6%A8%A1%E5%9E%8B%E6%A6%9C%E5%8D%95-model-rankings)
	- [基准 _Benchmarks_](#%E5%9F%BA%E5%87%86-benchmarks)
- [商业化 _Commercial_](#%E5%95%86%E4%B8%9A%E5%8C%96-commercial)

## 开源资源 _Open-Source Resources_

### 资源清单 _Resource Collections_

- [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM)：一份精选大模型资源清单。
- [Awesome-Chinese-LLM](https://github.com/AiHubCN/Awesome-Chinese-LLM)：整理开源的中文 LLM，以规模较小、可私有化部署、训练成本较低的模型为主，包括底座模型，垂直领域微调及应用，数据集与教程等。
- [awesome-deepseek-integration](https://github.com/deepseek-ai/awesome-deepseek-integration)：DeepSeek 实用集成，将 DeepSeek 大模型能力轻松接入各类软件。
- [awesome-cybersecurity-agentic-ai](https://github.com/raphabot/awesome-cybersecurity-agentic-ai)：网络安全智能体资源清单。
- [huggingface](https://huggingface.co/)：供机器学习领域从业者围绕模型、数据集与应用开展协作的平台。
- [awesome-ai-security](https://github.com/ottosulin/awesome-ai-security)：一份精选清单，收录优质的人工智能安全相关框架、规范标准、学习资料与开源工具。
- [awesome-offensive-security-ai](https://github.com/ox01024/awesome-offensive-security-ai)：精选的优秀进攻性安全 AI 工作、论文、组织、库和基准。
- [offensive-ai-compilation](https://github.com/jiep/offensive-ai-compilation)：一份汇总整理的、涵盖攻击性人工智能相关实用资源清单。
- [awesome-codex-cli](https://github.com/RoggeOhta/awesome-codex-cli)：收录 150 余款适用于 OpenAI Codex 命令行工具的 tools, skills, subagents & plugins。
- [Offensive AI Agentic](https://github.com/Yeti-791/Tsec-Hackathon/blob/main/Awesome%20Offensive%20AI%20List.md)：腾讯黑客松，AI 渗透测试 / LLM 红队 / 自主攻击 Agent / 漏洞挖掘 领域的开源项目、学术论文、能力评测 Benchmark 与国内外商业化解决方案。
- [Awesome-AI-Hacking-Agents](https://github.com/EvanThomasLuke/Awesome-AI-Hacking-Agents)：AI Hacking Agents 清单。
- [MCP-SecurityTools](https://github.com/Ta0ing/MCP-SecurityTools)：MCP-SecurityTools 是一个专注于收录和更新网络安全领域 MCP 的开源项目，旨在汇总、整理和优化各类与 MCP 相关的安全工具、技术及实战经验。

### 学术论文 _Papers_

> todo

### 实验环境 _Lab Environments_

- [Zero2Claude](https://zero2claude.dev/register)：从 0 开始学习 Claude Code。👍
- [Gandalf](https://gandalf.lakera.ai/baseline)：AI 提示词注入 Challenge。
- [Damn Vulnerable MCP Server](https://github.com/harishsg993010/damn-vulnerable-MCP-server)：MCP 漏洞教学靶场。
- [Vulnerable MCP Servers Lab](https://github.com/appsecco/vulnerable-mcp-servers-lab)：一套特意设置成存在安全漏洞、用于学习渗透测试的 MCP 服务器集群。
- [AI-Red-Teaming-Playground-Labs](https://github.com/microsoft/AI-Red-Teaming-Playground-Labs)：Microsoft 项目，可开展人工智能红蓝对抗培训的人工智能红队演练实验环境，配套相关基础设施。
- [Damn Vulnerable LLM Agent](https://github.com/ReversecLabs/damn-vulnerable-llm-agent)：LLM Agent 安全，聊天机器人教学靶场。
- [benchmark-platform](https://github.com/wgpsec/benchmark-platform)：AI Agent CTF 靶场竞赛平台。

### 提示词 _Prompts_

- [prompts.chat](https://github.com/f/prompts.chat)：优质 ChatGPT 提示词库，可在社区分享、查找、收集各类 AI 提示词。项目免费开源，企业可自主部署私有化服务，数据隐私完全可控。
- [awesome-chatgpt-prompts-zh](https://github.com/PlexPt/awesome-chatgpt-prompts-zh)：ChatGPT 中文调教指南。各种场景使用指南。学习怎么让它听你的话。
- [wonderful-prompts](https://github.com/langgptai/wonderful-prompts)：中文 prompt 精选，ChatGPT 使用指南，提升 ChatGPT 可玩性和可用性！
- [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks)：从 Anthropic 提取的系统提示 - Claude Code, Claude Design, Opus 4.8, Sonnet 4.6. OpenAI - ChatGPT 5.5 Thinking, GPT 5.5 Instant, Codex, Google - Gemini - 3.5 Flash, 3.1 Pro, Antigravity, xAI - Grok, Cursor, Copilot, VS Code, Perplexity 等。
- [CL4R1T4S](https://github.com/elder-plinius/CL4R1T4S)：完整提取自 OpenAI、Google、Anthropic、xAI、Perplexity、Cursor、Windsurf、Devin、Manus、Replit 等公司的系统提示、指南和工具。

### 编排框架 _Orchestration Frameworks_

- [langchain](https://github.com/langchain-ai/langchain)：LangChain 是一款用于构建智能代理与 LLM 驱动型应用的开发框架。
- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)：自主式 AI Agent 框架，可实现复杂工作流程自动化。

### 大模型部署与工具链 _Deployment & Toolchain_

- [ollama](https://github.com/ollama/ollama)：快速上手使用 Kimi-K2.6、GLM-5.1、MiniMax、DeepSeek、gpt-oss、通义千问、Gemma 等各类模型。
- [open-webui](https://github.com/open-webui/open-webui)：Open WebUI 是一款可扩展、功能丰富且易用的自建人工智能平台，能够完全离线运行。
- [chatbox](https://github.com/chatboxai/chatbox)：Chatbox 是一个 AI 模型桌面客户端，支持 ChatGPT、Claude、Google Gemini、Ollama 等主流模型，适用于 Windows、Mac、Linux、Web、Android 和 iOS 全平台。
- [anythingllm](https://anythingllm.com/)：借助强大的内置工具和功能快速运行本地 LLM，支持 MacOS/Windows/Linux 系统。
- [enchanted](https://github.com/gluonfield/enchanted)：Enchanted 是一款适用于 iOS 与 macOS 的应用程序，可借助 Ollama，对接本地私有化部署的 Llama2、Mistral、Vicuna 等 LLM 进行对话交互。
- [obsidian-copilot](https://github.com/logancyang/obsidian-copilot)：Obsidian 插件。
- [continue](https://github.com/continuedev/continue)：可在持续集成流程中强制执行的源码管控式 AI 校验工具，基于开源工具 Continue CLI 驱动。

### Agent Skills

- [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills)：面向人工智能智能体的 754 项结构化网络安全技能・适配五大框架：MITRE ATT&CK、NIST CSF 2.0、MITRE ATLAS、D3FEND 以及 NIST AI RMF。
- [pentest-ai-agents](https://github.com/0xSteph/pentest-ai-agents)：35 个 Claude Code 渗透 Subagent。
- [claude-bug-bounty](https://github.com/shuvonsec/claude-bug-bounty)：AI 驱动的漏洞赏金挖掘，信息侦察、20 类漏洞类型、自主化漏洞探测以及报告生成。
- [llm-sast-scanner](https://github.com/SunWeb3Sec/llm-sast-scanner)：一种静态应用安全测试（SAST）技术，可赋能 AI 代码智能体针对 34 类漏洞开展结构化漏洞检测。
- [sast-skills](https://github.com/utkusen/sast-skills)：可将 AI 代码开发工具转变为静态应用安全测试扫描器的智能代理技能合集。
- [Trail of Bits Skills](https://github.com/trailofbits/skills)：安全研究、漏洞挖掘与审计流程。
- [Elastic Agent Skills](https://github.com/elastic/agent-skills)：Elastic 官方 skills 库，日志、追踪、威胁情报。
- [Semgrep Skills](https://github.com/semgrep/skills)：安全扫描、代码分析、漏洞检测。
- [claude-secure-coding-rules](https://github.com/TikiTribe/claude-secure-coding-rules)：面向 Claude 代码的安全编码规范。
- [awesome-agent-skills](https://github.com/JackyST0/awesome-agent-skills)：精选的 AI Agent Skills 列表，适用于 Cursor、Claude Code、GitHub Copilot 等 AI 编程工具。
- [awesome-agent-skills](https://github.com/libukai/awesome-agent-skills)：Agent Skills 终极指南：快速入门、资源推荐、精选技能与实用工具。
- [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)：收录来自官方开发团队与社区的 1000 余项 Agent Skills 技能。
- [Anthropics Skills](https://github.com/anthropics/skills)：Anthropics 官方 skills 库。[skill-creator](https://github.com/anthropics/skills/blob/main/skills/skill-creator/SKILL.md ) 用于生成自定义 skills。
- [ECC](https://github.com/affaan-m/ECC)：来自 Anthropic 黑客马拉松获胜者的完整 Claude Code 配置集合。不止是配置文件，而是一整套完整系统：技能体系、本能行为、记忆优化、持续学习、安全扫描，以及研究优先的开发模式。 包含可直接用于生产环境的智能体、技能模块、钩子、规则、MCP 配置，以及兼容传统命令的适配层。可在 Claude Code、Codex、Cursor、OpenCode、Gemini 及其他 AI 智能体框架中通用。
- [baoyu-skills](https://github.com/JimLiu/baoyu-skills)：AI Agent 技能集（适用于 Claude Code、Codex 等），提升日常工作效率。
- [SecSkills](https://github.com/DaoYiSec/SecSkills)：收集整理渗透测试、漏洞扫描、代码审计、CTF、逆向、安全研究 等网络安全相关的 Skills 和 MCP。

## 治理与风险管理 _Governance & Risk Management_

### 框架 _Frameworks_

- [NIST - AI Risk Management Framework](https://airc.nist.gov/airmf-resources/airmf/)：NIST 人工智能风险管理框架（AI RMF）
- [ISO/IEC 42001:2023](https://www.iso.org/standard/42001)：ISO/IEC 人工智能管理系统标准
- [ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html)：ISO/IEC 人工智能风险评估管理体系
- [Google's Secure AI Framework](https://saif.google/)：Google 安全 AI 框架，人工智能安全实操指南
- [ENISA - Multilayer Framework for Good Cybersecurity Practices for AI](https://www.enisa.europa.eu/publications/multilayer-framework-for-good-cybersecurity-practices-for-ai)：ENISA AI 网络安全多层框架
- [OWASP-www-project-ai-maturity-assessment](https://github.com/OWASP/www-project-ai-maturity-assessment)：OWASP AI 成熟度评估

### 标准与验证 _Standards & Verification_

- [OWASP-AISVS](https://github.com/OWASP/AISVS)：AI Security Verification Standard (AISVS）旨在为开发人员、架构师与安全从业者提供一套结构化核查清单，用于核验人工智能应用的安全能力。
- [OWASP-ANS](https://genai.owasp.org/resource/agent-name-service-ans-for-secure-al-agent-discovery-v1-0/)：依托 OWASP 生成式人工智能安全项目 —— 智能体安全专项研发的 Agent Name Service（ANS），推出了一套借鉴域名系统（DNS）设计的安全框架，用于实现人工智能智能体的寻址发现。该服务依托公钥基础设施（PKI）完成身份核验，采用标准化 JSON 模式开展数据交互，同时配备协议适配层，可兼容 A2A、MCP 与 ACP 三类协议。
- [OWASP Agent Observability Standard](https://aos.owasp.org/)：Agent 可观测性标准。

### 术语体系与数据库 _Taxonomies & Databases_

- [NIST AI 100-2 E2023](https://csrc.nist.gov/pubs/ai/100/2/e2023/ipd)：对抗性机器学习 攻击与防御措施的分类及术语说明
- [MITRE ATLAS](https://atlas.mitre.org/)：对抗性 AI 战术与技术知识库
- [AVIDML](https://avidml.org/taxonomy/)：AI 风险分类体系
- [MIT AI Risk Repository](https://airisk.mit.edu/)：AI 风险数据库
- [AI Incident Database](https://incidentdatabase.ai/)：AI 安全事件数据库
- [Arcanum PI Taxonomy](https://arcanum-sec.github.io/arc_pi_taxonomy/)：Prompt Injection 攻击分类体系
- [CSA Large Language Model (LLM) Threats Taxonomy](https://cloudsecurityalliance.org/artifacts/csa-large-language-model-llm-threats-taxonomy)：CSA LLM 威胁分类体系
- [OWASP-AIVSS](https://github.com/OWASP/www-project-artificial-intelligence-vulnerability-scoring-system)：AI 漏洞评分系统

### 清单与指南 _Checklists & Guidance_

- [OWASP ML TOP 10](https://owasp.org/www-project-machine-learning-security-top-10/)
- [OWASP LLM TOP 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [OWASP Agentic TOP 10](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/)
- [MLSecOps TOP 10](https://ethical.institute/security.html)
- [OpenClaw Security Engineer's Cheat Sheet](https://semgrep.dev/blog/2026/openclaw-security-engineers-cheat-sheet/)：OpenClaw 安全工程师 CheetSheet
- [OWASP LLM Applications Cybersecurity and Governance Checklist ](https://genai.owasp.org/resource/llm-applications-cybersecurity-and-governance-checklist-english/)：OWASP LLM 应用安全与治理清单
- [OWASP AI Security and Privacy Guide](https://github.com/OWASP/www-project-ai-security-and-privacy-guide)：OWASP AI 安全与隐私指南
- [OWASP Agentic AI – Threats and Mitigations](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/)：OWASP Agentic AI 威胁与缓解措施
- [OWASP Securing Agentic Applications Guide](https://genai.owasp.org/resource/securing-agentic-applications-guide-1-0/)：OWASP 保护 Agentic AI 应用
- [OWASP GenAI Red Teaming Guide](https://genai.owasp.org/resource/genai-red-teaming-guide/)：OWASP GenAI 红队指南
- [OWASP CheatSheet – A Practical Guide for Securely Using Third-Party MCP Servers](https://genai.owasp.org/resource/cheatsheet-a-practical-guide-for-securely-using-third-party-mcp-servers-1-0/)：OWASP MCP 服务器安全使用清单
- [OWASP Multi-Agentic system Threat Modeling Guide](https://genai.owasp.org/resource/multi-agentic-system-threat-modeling-guide-v1-0/)：OWASP Multi-Agentic 系统威胁建模

## 进攻性安全 _Red Teaming and Offensive Security_

### LLM & Agent 对抗性安全 _LLM & Agent Adversarial Security_

#### 综合红队框架 _Comprehensive Red Teaming Frameworks_

- [garak](https://github.com/NVIDIA/garak)：Nvidia 项目，LLM 漏洞扫描器。
- [promptfoo](https://github.com/promptfoo/promptfoo)：测试提示词、智能代理与检索增强生成（RAG）。面向人工智能开展红蓝对抗 / 渗透测试 / 漏洞扫描。
- [PyRIT](https://github.com/microsoft/PyRIT)：Microsoft 项目，面向生成式 AI 的 Python 风险识别工具（PyRIT）是一款开源框架，旨在帮助安全从业人员与工程师主动排查生成式人工智能系统中的各类风险。
- [PurpleLlama](https://github.com/meta-llama/PurpleLlama)：Meta 项目，LLM 安全评估与改进工具集。
- [deepteam](https://github.com/confident-ai/deepteam)：一款针对 LLM 及其系统开展红队测试的框架。
- [augustus](https://github.com/praetorian-inc/augustus)：一款用于检测提示注入、越狱攻击与对抗攻击的大模型安全测试框架 —— 内置 190 余项测试探针、适配 28 个服务商，编译后为单个 Go 可执行文件。
- [ai-scanner](https://github.com/0din-ai/ai-scanner)：基于 Nvidia garak 搭建的人工智能模型安全扫描工具。
- [AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard/)：腾讯朱雀实验室，AI 红队平台（Infra/MCP/Jailbreak）。

#### 越狱与对抗测试 _Jailbreak & Adversarial Testing_

- [PromptJailbreakManual](https://github.com/Acmesec/PromptJailbreakManual)：Prompt 越狱手册。
- [EasyJailbreak](https://github.com/EasyJailbreak/EasyJailbreak)：一个轻量、易用、纯 Python 实现的对抗性越狱提示词生成框架。
- [GPTFuzz](https://github.com/sherdencooper/GPTFuzz)：利用自动生成的越狱提示词对 LLM 开展红蓝对抗测试。
- [FuzzyAI](https://github.com/cyberark/FuzzyAI)：CyberArk 项目，LLM 自动化 Fuzz 工具。
- [G0DM0D3](https://github.com/elder-plinius/G0DM0D3)：一款完全开源、注重隐私保护的多模型对话交互程序，它不断突破后训练层的技术上限，可用于红队测试、认知科学研究以及自由化人工智能交互场景。

#### Prompt 注入 _Prompt Injection_

- [OpenPromptInjection](https://github.com/liu00222/Open-Prompt-Injection)：为 LLM 中的提示注入攻击与防护方案提供了一套基准测试标准。
- [promptmap](https://github.com/utkusen/promptmap)：一款面向定制化大模型应用的自动化提示注入扫描工具。
- [llm-security](https://github.com/greshake/llm-security)：利用间接提示注入攻击 LLM。[Paper](https://arxiv.org/abs/2302.12173)

#### Agent 安全 _Agent Security_

- [RAMPART](https://github.com/microsoft/RAMPART)：Microsoft 出品，Agent AI 安全测试框架（pytest 原生）。
- [Agentic Radar](https://github.com/splx-ai/agentic-radar)：面向大模型智能体工作流的安全扫描工具。
- [agentic_security](https://github.com/msoedov/agentic_security)：智能体大模型漏洞扫描工具 / 人工智能红队测试套件。
- [giskard-oss](https://github.com/Giskard-AI/giskard-oss)：主流开源 LLM 智能体评测。

### AI 赋能攻击性安全 _AI-Assisted Offensive Security_

> Some projects may not be fully tested. Use with caution. 部分项目未经完整测试，请谨慎使用。

#### 渗透测试 _Penetration Agents_

- [CyberStrikeAI](https://github.com/Ed1s0nZ/CyberStrikeAI)：CyberStrikeAI 是一款基于 Go 语言开发的原生人工智能安全测试平台。该平台集成了一百余款安全工具、智能编排引擎、搭载预设安全角色的基于角色测试模块、具备专项测试能力的技能体系以及全生命周期管理功能。
- [shannon](https://github.com/KeygraphHQ/shannon)：Shannon 是一款面向网页应用与应用程序接口的自主式白盒人工智能渗透测试工具。它能够分析源代码、定位攻击切入点，并通过执行真实漏洞利用程序，在漏洞上线投产前完成漏洞验证。
- [PentestGPT](https://github.com/GreyDGL/PentestGPT)：基于 LLM 的自动化渗透测试智能体框架。
- [strix](https://github.com/usestrix/strix)：开源 AI 黑客，排查并修复你的应用程序漏洞。
- [JoySafeter](https://github.com/jd-opensource/JoySafeter)：一款企业级智能体平台 —— 不止于对话交互，依托可视化编排实现自主智能体团队的搭建、部署、测试与全链路追踪。
- [cai](https://github.com/aliasrobotics/cai)：Cybersecurity AI (CAI)，人工智能安全框架。
- [pentagi](https://github.com/vxcontrol/pentagi)：可执行复杂渗透测试任务的全自主智能体系统。
- [raptor](https://github.com/gadievron/raptor)： Raptor 将 Claude Code 转化为通用型 AI 攻防安全代理。
- [hexstrike-ai](https://github.com/0x4m4/hexstrike-ai)：MCP 服务端，可支持 Claude、GPT、Copilot 等各类 AI 智能代理自主调用 150 余款网络安全工具。
- [redamon](https://github.com/samugit83/redamon)：一款依托人工智能驱动的自主化红队框架，可在无需人工介入的前提下，自动化完成从情报侦察、漏洞利用到后渗透阶段的各类攻击性安全任务。
- [guardian-cli](https://github.com/zakirkun/guardian-cli)：Guardian 是企业级人工智能驱动的自动化渗透测试框架，该框架整合多家人工智能服务商（OpenAI GPT-4、Claude、Google Gemini、OpenRouter）与经过实战验证的安全工具，可实现智能化、自适应安全评估，并完整留存取证资料。
- [AutoPentestX](https://github.com/Gowtham-Darkseid/AutoPentestX)：自动化渗透测试与漏洞报告生成工具。
- [pentest-ai-agents](https://github.com/0xSteph/pentest-ai-agents)：将 Claude Code 打造为你的攻击性安全研究助手。
- [hackGPT](https://github.com/NoDataFound/hackGPT)：使用 ChatGPT 进行黑客攻击。
- [LuaN1aoAgent](https://github.com/SanMuzZzZz/LuaN1aoAgent/tree/main)：新一代基于大模型的自主渗透测试智能体。
- [deadend-cli](https://github.com/xoxruns/deadend-cli)：智能自主渗透测试工具。该工具依托 KIMI K2.5 模型，在 XBOW 基准测试的纯黑盒场景下目前得分 81%。

#### 漏洞研究 _Vulnerability Research_

- [vulnhuntr](https://github.com/protectai/vulnhuntr)：基于 LLM 的 0day 漏洞挖掘。
- [buttercup](https://github.com/trailofbits/buttercup)：LLM 驱动的漏洞发现与漏洞修复。
- [DeepAudit](https://github.com/lintsinghua/DeepAudit)：代码漏洞挖掘多智能体系统。已成功发现并获得 49 个 CVE 编号 和 6 个 GHSA 安全公告。

#### 逆向与反编译 _Reverse Engineering & Decompilation_

- [android-reverse-engineering-skill](https://github.com/SimoneAvogadro/android-reverse-engineering-skill)：Claude Code Skill，Android 反汇编与 API 提取。
- [js-reverse-automation--skill](https://github.com/Fausto-404/js-reverse-automation--skill)：结合 chrome-devtools-mcp 的能力并加上 Skill 的规范，实现 JSRPC+Flask+autoDecoder 方案的前端 JS 逆向自动化分析，提升 JS 逆向的效率。
- [REA](https://github.com/morluto/rea)：面向 AI 智能体的本地逆向工程 CLI 与 MCP 服务器，支持原生二进制、JavaScript/Electron 和 .NET 分析，返回证据来源与分析限制；原生深度分析需另行安装 Hopper、Ghidra 或 IDA。

#### CTF _Capture the Flag_

- [Tsec-Hackathon](https://github.com/Yeti-791/Tsec-Hackathon)：腾讯云智能渗透黑客松。
- [BreachWeave](https://github.com/m-sec-org/BreachWeave)：智能渗透 Agent Manager/Observer/Solver 多角色架构，基于 pi-mono SDK。Tsec-Hackathon 1st。
- [BoxPwnr](https://github.com/0ca/BoxPwnr)：一套模块化框架，用于在 HackTheBox、TryHackMe、PortSwigger、Cybench、picoCTF 等平台的安全攻防题目上，对大语言模型与智能体方案开展基准性能测评。
- [ctf-agent](https://github.com/verialabs/ctf-agent)：BSidesSF 2026 CTF 冠军。

#### MCP 集成 _MCP Security Integration_

- [mcp-for-security](https://github.com/cyproxio/mcp-for-security)：一套适配主流安全工具的模型上下文协议服务端合集，涵盖 SQLMap、FFUF、NMAP、Masscan 等多款常用工具，可将安全测试与渗透测试功能接入人工智能工作流。
- [mcp-security-hub](https://github.com/FuzzingLabs/mcp-security-hub)：一套不断扩充的 MCP 服务器合集，可为人工智能助手集成攻击性安全工具，包含 Nmap、Ghidra、Nuclei、SQLMap、Hashcat 等多款工具。
- [mcp-server](https://github.com/PortSwigger/mcp-server)：Burp Suite MCP 服务器。
- [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp)：用于代码编写代理的 Chrome DevTools 工具。

## 防御性安全 _Blue Teaming and Defensive Security_

### 安全围栏 _Guardrails_

- [Guardrails](https://github.com/NVIDIA-NeMo/Guardrails)：Nvidia 项目，NeMo Guardrails 是一款开源工具包，可便捷地为基于大语言模型的对话系统添加可编程安全防护规则。
- [LlamaFirewall](https://github.com/meta-llama/PurpleLlama/tree/main/LlamaFirewall)：Meta 项目，LlamaFirewall 是一款用于检测和缓解人工智能相关安全风险的框架，支持多层面的输入与输出场景，包括常规大语言模型对话以及更为复杂的多步骤智能体任务运行。
- [llm-guard](https://github.com/protectai/llm-guard)：LLM 安全加固综合工具。
- [rebuff](https://github.com/protectai/rebuff)：Prompt Injection 检测器。
- [langkit](https://github.com/whylabs/langkit)：一款用于监控大语言模型（LLMs）的开源工具包。

### 运行时安全与沙箱 _Runtime Security & Sandboxing_

- [OpenShell](https://github.com/NVIDIA/OpenShell)：Nvidia 项目，OpenShell 是面向自主智能体的安全、私密运行环境。
- [OpenSandbox](https://github.com/opensandbox-group/OpenSandbox)：面向 AI 智能体，安全、高性能、可扩展的沙箱运行时环境。
- [CubeSandbox](https://github.com/TencentCloud/CubeSandbox)：面向智能体的即时、并发、安全且轻量型沙箱。
- [Aegis](https://github.com/antropos17/Aegis)：面向智能体的开源终端检测与响应（EDR）工具。
- [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)：Microsoft 项目，Agent 治理工具包，覆盖 OWASP Agentic Top 10。
- [microsandbox](https://github.com/superradcompany/microsandbox)：轻量 microVM 沙箱。
- [claude-code-safety-net](https://github.com/kenryu42/claude-code-safety-net)：Claude Code 破坏性命令拦截插件，兼容 Codex、Claude Code、OpenCode、Gemini CLI 以及 Copilot CLI。
- [pipelock](https://github.com/luckyPipewrench/pipelock)：面向 MCP 安全的开源 AI 智能体防火墙，出站管控、数据防泄漏、服务端请求伪造防护以及提示注入防御。
- [onecli](https://github.com/onecli/onecli)：自带密钥保管库的开源凭证网关，可在不泄露密钥的前提下让 AI 智能体访问各类服务。

### MCP 安全 _MCP Security_

- [MCP-Security-Checklist](https://github.com/slowmist/MCP-Security-Checklist)：MCP 安全检查清单。
- [Awesome-MCP-Security](https://github.com/Puliczek/awesome-mcp-security)：MCP 安全知识大全。
- [agent-scan](https://github.com/snyk/agent-scan)：面向 AI 智能体、MCP 服务器以及智能体 Skills 的安全扫描工具。
- [mcpproxy-go](https://github.com/smart-mcp-proxy/mcpproxy-go)：MCP 代理。

### 模型与制品扫描 _Model & Artifact Scanning_

- [skill-scanner](https://github.com/cisco-ai-defense/skill-scanner)：Agent Skills 安全扫描工具。
- [modelscan](https://github.com/protectai/modelscan)：防范模型序列化攻击。
- [picklescan](https://github.com/mmaitre314/picklescan)：Python Pickle 可疑操作检测。
- [fickling](https://github.com/trailofbits/fickling)：一款针对 Python pickle 对象序列化的反编译器、静态分析工具与字节码改写工具。
- [medusa](https://github.com/Pantheon-Security/medusa)：搭载 76 项分析器、9600 余条检测规则，可针对人工智能 / 机器学习、大语言模型智能代理与 MCP 服务器实现代码仓库投毒检测。

### AI 赋能防御性安全 _AI-Assisted Defensive Security_

- [Claude Code Security Reviewer](https://github.com/anthropics/claude-code-security-review)：一款依托 Claude 实现的 AI 安全审查 GitHub 动作，用于分析代码变更中存在的安全漏洞。
- [deepsec](https://github.com/vercel-labs/deepsec)：Code Agents 驱动，用于在代码库中查找漏洞的安全检测工具。
- [AiSOC](https://github.com/beenuar/AiSOC)：开源人工智能驱动型安全运营中心 —— 告警融合、红蓝对抗演练、智能代理辅助研判、基于 MITRE ATT&CK 框架开展事件溯源分析。

## AI 工具 _AI Tools_

- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)：AutoGPT 是一个强大的平台，可帮助您创建、部署和管理持续运行的 AI 智能体，实现复杂工作流程的自动化。

## 评测基准 _Benchmarks & Evaluations_

### 模型榜单 _Model Rankings_

- [OpenRouter AI Model Rankings](https://openrouter.ai/rankings)：依托基准测试数据以及数百万用户经由 OpenRoute 调用各类模型产生的实际使用数据。
- [Arena Leaderboard](https://arena.ai/leaderboard)：查看主流人工智能模型在文本、图像、视觉等多领域的综合表现。
- [LLM Leaderboard](https://llm-stats.com/)：对比 300 余款顶尖 AI 模型的智能水平、运行速度与定价。

### 基准 _Benchmarks_

- [OpenCompass](https://github.com/open-compass/opencompass)：OpenCompass 是一款 LLM 评测平台，依托百余种评测数据集，可对 Llama3、Mistral、InternLM2、GPT-4、LLaMa2、通义千问、GLM、Claude 等海量模型开展测评。
- [PurpleLlama](https://github.com/meta-llama/PurpleLlama)：用于评估和优化 LLM 安全性的工具套件。
- [JailbreakBench](https://github.com/JailbreakBench/jailbreakbench)：一款用于 LLM 越狱攻击的开源鲁棒性基准测评平台。NeurIPS 2024。
- [XBOW Validation Benchmarks](https://github.com/xbow-engineering/validation-benchmarks)：104 项 Web 漏洞挑战。
- [CyberGym](https://github.com/sunblaze-ucb/cybergym)：一套大规模、高质量的网络安全评测框架，旨在针对现实环境下的漏洞分析任务，对智能体的各项能力开展严谨测评。
- [NYU CTF Bench](https://github.com/NYU-LLM-CTF/NYU_CTF_Bench)：NYU CTF 基准测试数据集。

## 商业化 _Commercial_

> todo
