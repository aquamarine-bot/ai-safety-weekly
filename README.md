# AI Safety Weekly

> Weekly curated papers on AI Safety, LLM red-teaming, adversarial attacks, and agent security

Auto-updated weekly. Last update: **2026-09-21**

---

## 2026-W38

### [SWE-Proof: Can Language Models Resolve Real-World Issues with Machine-Checked Proofs?](https://arxiv.org/abs/2609.21190v1)
- **Authors:** George Ma, Benjamin Mikek, Haoyu Li et al.
- **Date:** 2026-09-18
- **Category:** `"agentic" AND "adversarial"`

> Ensuring the correctness of LLM-generated code is a core challenge for modern software engineering. Benchmarks for agentic code generation check correctness with held-out test suites, which are inherently incomplete and increasingly susceptible to memorization. Formal verification avoids both problems, but existing work covers only standalone tasks...

**📝 Summary:** SWE-Proof：探索用机器可检查证明而非测试用例，评测 LLM 能否正确解决真实代码仓库中意图模糊的 issue。

### [Provisional Reachability: Containing Agents by Making Every Crossing Revocable](https://arxiv.org/abs/2609.21957v1)
- **Authors:** Yoshiaki Takashita
- **Date:** 2026-09-18
- **Category:** `"agentic" AND "adversarial"`

> A companion paper found that what a defender must block over time has units: bits per period [Takashita, 2026a]. This paper sets it. Hold every crossing in escrow for one period, audit each held item independently with probability r, and revoke the window if any audit catches something. An adversary crossing k times, each carrying c bits, expects k...

**📝 Summary:** 提出「可撤销穿越」机制，将每次 agent 跨边界行为托管审计一段时间，理论给出对抗者信息泄露量的上界。

### [APort Vault: Benchmarking AI Agent Payment Authorization with the Open Agent Passport](https://arxiv.org/abs/2609.22076v1)
- **Authors:** Uchi Uchibeke
- **Date:** 2026-09-18
- **Category:** `"tool use" AND "attack"`

> APort Vault is a benchmark for payment authorization in tool-using AI agents. It replays 4,371 attacks written by humans against a live payment agent during a public capture-the-flag event, across 14 models from 8 labs, five policy configurations and two replay tracks, with and without a deterministic pre-action check implementing the Open Agent Pa...

**📝 Summary:** APort Vault：基于真实 CTF 活动中 4000+ 次人类攻击，对 8 家实验室 14 个模型的支付授权 agent 做大规模红队评测。

### [CIPL: A Channel-Aware Framework for Recoverable Privacy Leakage in LLM Agents](https://arxiv.org/abs/2609.21686v1)
- **Authors:** Tao Huang, Guosen Wu, Guolong Zheng et al.
- **Date:** 2026-09-18
- **Category:** `"tool use" AND "attack"`

> Privacy leakage in LLM agents is commonly evaluated within individual components such as memory, retrieval, or tool-use pipelines, which makes it difficult to distinguish internal exposure from information that an external observer can actually recover. We present CIPL (Channel Inversion for Privacy Leakage), a channel-aware evaluation framework fo...

**📝 Summary:** CIPL：面向 LLM agent 的信道感知隐私泄露评测框架，区分内部暴露与外部观察者可实际恢复的信息。

### [UnifiedPlayers: Enhance Tool-Integrated Reasoning in Agentic Reinforcement Learning](https://arxiv.org/abs/2609.20089v1)
- **Authors:** Wenjie Liao, Liangjie Zhao, Zehong Cao
- **Date:** 2026-09-17
- **Category:** `"agentic" AND "adversarial"`

> Self-evolving methods reduce the need for human-annotated trajectories by allowing tool-using agents to generate their own training data. Yet existing methods typically separate trajectory generation from evaluation, relying on static verifiers that cannot adapt to emerging failure modes or self-consistency signals that may reinforce errors shared ...

**📝 Summary:** UnifiedPlayers：联合训练规划、执行、评估三个角色，改进工具集成推理 agent 的自我进化式强化学习。

### [SoK: Trading Agents or Market Crashers? Dissecting Robustness and Security Failures in Academic Financial LLM Trading Schemes](https://arxiv.org/abs/2609.19705v1)
- **Authors:** Mengxiao Wang, Nitesh Saxena
- **Date:** 2026-09-17
- **Category:** `"LLM agent" AND "attack"`

> Autonomous large language model (LLM) agents are moving rapidly into high-stakes domains, yet existing agentic-AI security studies remain largely domain-agnostic and overlook the distinctive, high-consequence attack surface such settings create. We examine this gap through financial trading agents, a representative case of high-stakes agentic secur...

**📝 Summary:** SoK 系统化梳理金融交易 LLM agent 方案中的鲁棒性与安全失败模式，指出高风险领域特有的攻击面。

### [Safety-Critical Scenarios Emerge from Initial Scenes](https://arxiv.org/abs/2609.20103v2)
- **Authors:** Yin Wu, Jiarong Wei, Carl Esselborn et al.
- **Date:** 2026-09-17
- **Category:** `"agentic" AND "adversarial"`

> Safety-critical driving scenario generation has largely focused on manipulating the behavior of surrounding agents while starting from an initial scene from driving data. This assumption can limit the space of discoverable failures, since driving data can provide little opportunity for meaningful interaction. For example, in the Waymo Open Motion D...

**📝 Summary:** 指出自动驾驶安全关键场景生成过度依赖真实初始场景（很多场景无交互空间），提出从更广泛初始场景中主动挖掘安全关键情形。

### [Xeno-Interpretability: Investigating the Alien Minds of LLMs](https://arxiv.org/abs/2609.20408v1)
- **Authors:** F. Pierucci, M. Bracale Syrnikov, M. Prandi et al.
- **Date:** 2026-09-17
- **Category:** `"multi-agent" AND "safety"`

> Large language models are usually interpreted through concepts that humans already possess: truthfulness, refusal, deception, personality, harmfulness, and related categories. This paper asks whether models may also represent and use distinctions for which no adequate human concept exists. We call such internal structures xeno-representations, and ...

**📝 Summary:** 提出「异种可解释性」概念，探究 LLM 内部是否存在人类现有概念无法描述的原生表征结构。

### [Robust Workflow Generation via Adversarial Learning for Audio Deepfake Detection](https://arxiv.org/abs/2609.20063v1)
- **Authors:** Xiang Li, Pin-Yu Chen, Wenqi Wei
- **Date:** 2026-09-17
- **Category:** `"agentic" AND "adversarial"`

> The rapid advancement of speech synthesis and voice conversion technologies has made audio deepfakes increasingly realistic, posing serious security risks in practical applications. While existing detection methods achieve strong performance under controlled conditions, they often fail to generalize under real-world perturbations and corruptions. I...

**📝 Summary:** ROGUE：通过对抗学习动态编排多个检测工具，生成更鲁棒的音频深度伪造检测工作流。

### [Deep Noir: Autonomous Steering Discovery via Architectural Chronometry in Transformer Models](https://arxiv.org/abs/2609.20722v1)
- **Authors:** Frank E. Bobe, Gregory D. Vetaw, Darshan W. Bryner et al.
- **Date:** 2026-09-17
- **Category:** `"prompt injection" AND "agent"`

> Activation steering modifies LLM behavior at inference time, but identifying where and how strongly to steer remains manual. We introduce Deep Noir, a framework that uses Logit Lens convergence and causal head-level attribution to autonomously discover optimal steering parameters. Across three scales (1B x 3, 2-3B x 2, and 7-9B x 4), our engine ach...

**📝 Summary:** Deep Noir：用 Logit Lens 收敛与因果头部归因自动发现最优激活转向（steering）参数，无需人工调参。

### [Red-Teaming Auto Mode: Improving Blocking Classifiers Against Malign Coding Agents](https://arxiv.org/abs/2609.19587v1)
- **Authors:** Alex Remedios, Simon Storf, Fabien Roger et al.
- **Date:** 2026-09-17
- **Category:** `"prompt injection" AND "agent"`

> To keep coding agents from going off the rails, production systems now review each proposed action with a blocking monitor that can reject it before it runs (Auto Mode in Claude Code, Guardian in OpenAI's Codex). Prior evaluations of such monitors largely measure robustness to accidental harm or prompt injections from untrusted sources looking to h...

**📝 Summary:** 研究持续恶意（misaligned）编码 agent 如何对抗性地绕过生产环境的动作拦截分类器（如 Claude Code Auto Mode、Codex Guardian）。

### [SAGE: Safety-Aligned Gradient Enforcement for Human--Robot Collaboration](https://arxiv.org/abs/2609.21130v1)
- **Authors:** Yisen Li, Hao Zhang, Ruize Geng et al.
- **Date:** 2026-09-17
- **Category:** `"multi-agent" AND "safety"`

> Multi-party human-robot collaboration poses a dual challenge: robot decisions should remain interpretable and auditable, while executed actions must satisfy safety constraints during physical interaction. Combining explainable decision-tree policies with control-barrier-function (CBF) filtering provides a promising architecture but creates two lear...

**📝 Summary:** SAGE：结合可解释决策树策略与控制屏障函数，解决多智能体强化学习中人机协作的安全投影与梯度失配问题。

### [CaMeLoT: CaMeL orchestrated with Temporal logic for static verification and liveness](https://arxiv.org/abs/2609.18674v1)
- **Authors:** Elia Nikolaou, Magnus Wiik Eckhoff, Robert Flood et al.
- **Date:** 2026-09-16
- **Category:** `"prompt injection" AND "agent"`

> LLM-based agents generate and execute multi-step plans that invoke external tools which can access private data or execute commands. In this setting, security is a property of the entire execution that a plan creates, not just any single step. The plan itself is a critical artefact that captures the tool calls, control flow, and data dependencies. ...

**📝 Summary:** CaMeLoT：在 CaMeL 基础上加入时序逻辑做静态验证，保证工具调用 agent 计划的活性（liveness）与安全性。

### [AgentLSD: Evaluating AI Security Agents Under Adversarial Task Contamination](https://arxiv.org/abs/2609.19140v1)
- **Authors:** Matteo Golinelli, Idilio Drago, Matteo Boffa et al.
- **Date:** 2026-09-16
- **Category:** `"prompt injection" AND "agent"`

> AI agents for security inspect web pages, source code, logs, configuration files, and command outputs. These environments may contain deceptive artifacts that influence the agent's behavior. We call this adversarial task contamination. Whereas prompt injection relies on attacker-supplied instructions, task contamination also includes non-instructio...

**📝 Summary:** AgentLSD：研究安全类 agent 面对「对抗性任务污染」（伪造结果、诱饵端点等非指令性欺骗证据）时的鲁棒性。

### [The Verifiable Action Card: Trustworthy Human-in-the-Loop Control for Secure Autonomous Agents](https://arxiv.org/abs/2609.18411v1)
- **Authors:** Hasnain Irshad, Anam Mughees, Neelam Mughees et al.
- **Date:** 2026-09-16
- **Category:** `"prompt injection" AND "agent"`

> Agentic browsers can execute security-sensitive actions under a user's authenticated session, making indirect prompt injection and deceptive confirmation interfaces a direct threat to action integrity. Existing human-in-the-loop (HITL) safeguards are insufficient when the approval prompt itself can be influenced by untrusted page content or model-g...

**📝 Summary:** 提出 Verifiable Action Card：在 HITL 审批时从可信来源重建操作信息，防止页面注入内容污染确认弹窗，抵御间接提示注入。

### [CARES: A Conversational AI System for Regulation-Grounded Safety Reporting in Construction Education](https://arxiv.org/abs/2609.19429v1)
- **Authors:** Fan Yang, Jiabin Wu, Yuan Tian et al.
- **Date:** 2026-09-16
- **Category:** `"multi-agent" AND "safety"`

> Construction safety reporting often relies on manual logs and static templates that provide limited feedback and leave daily activities disconnected from relevant regulations. This paper introduces CARES (Conversational AI Reporting for Enhanced Safety), a conversational AI system that integrates regulatory guidance into daily reporting to support ...

**📝 Summary:** CARES：面向建筑安全教育的对话式 AI 系统，结合多智能体对话、RAG 与法规落地的安全报告生成。

### [MAGS: Multi-agent Auto-formalization Guarantees Safety for Agentic Outputs](https://arxiv.org/abs/2609.19391v1)
- **Authors:** Albert Wu, Nicholas Roberts, Tzu-Heng Huang et al.
- **Date:** 2026-09-16
- **Category:** `"multi-agent" AND "safety"`

> LLM coding agents now generate complex programs at a scale that makes thorough human review increasingly difficult, raising the risk of safety and security failures. Common approaches, including fuzz testing, static analysis, and LLM-as-a-Verifier, can detect many failures but struggle to cover all possible edge cases. Formal verification addresses...

**📝 Summary:** MAGS：多智能体自动形式化框架，为 LLM 编码 agent 的输出提供机器可检查的安全性保证。

### [ASLEval: Measuring Privacy Exposure Displacement in LLM Agent Sessions](https://arxiv.org/abs/2609.18864v2)
- **Authors:** Guosen Wu, Huizhen Huang, Guoxiong Long et al.
- **Date:** 2026-09-16
- **Category:** `"tool use" AND "attack"`

> Privacy evaluations of tool-using LLM agents often inspect a designated action, final response, or attacker report. These local proxies can miss unauthorized exposure elsewhere in a multi-step session and lack common ground truth across outlets, reports, and tool paths. We introduce privacy exposure displacement, the mismatch between a local evalua...

**📝 Summary:** ASLEval：提出「隐私暴露位移」概念及配套框架，度量 agent 会话中本地评测代理与真实目标暴露之间的偏差。

### [Benchmarking Factual Robustness of LLMs via Multi-conversation Persuasion](https://arxiv.org/abs/2609.16777v1)
- **Authors:** Zhuoang Cai
- **Date:** 2026-09-15
- **Category:** `"red teaming" AND "LLM"`

> As Large Language Models (LLMs) increasingly serve as primary knowledge retrieval interfaces, their robustness against \textit{persuasion attacks}---attempts to inject misinformation or enforce counterfactuals---has become a critical safety concern. Existing red-teaming frameworks typically evaluate models in multi-turn dialogues where the target m...

**📝 Summary:** 发现多轮说服攻击中的「拒绝惯性」缺陷：模型一旦拒绝就倾向持续拒绝，掩盖了真实的说服鲁棒性，提出改进的红队评测框架。

### [Emergence World: Adversarial Stress-Testing of Long-Horizon Multi-Agent Systems](https://arxiv.org/abs/2609.17320v1)
- **Authors:** Deepak Akkil, Tamer Abuelsaad, Karthik Vikram et al.
- **Date:** 2026-09-15
- **Category:** `"multi-agent" AND "safety"`

> As AI agents move from bounded tasks to persistent deployments, failures can propagate through memory, tools, other agents, and environmental state long after their interactions. This creates a safety regime that cannot be characterized by evaluating model responses in isolation. Emergence World, is a continuously running multi-agent environment fo...

**📝 Summary:** Emergence World：让 8 组 10-agent 长时程多智能体系统持续运行以做对抗压力测试，观察故障如何跨记忆/工具/agent 传播。

### [Test-Time Unlearning via Sparse Autoencoder](https://arxiv.org/abs/2609.16229v1)
- **Authors:** Pingzhi Li, Jinhao Duan, Vaishnav Tadiparthi et al.
- **Date:** 2026-09-14
- **Category:** `"adversarial attack" AND "language model"`

> Machine unlearning aims to remove specific knowledge from a trained large language model (LLM) without retraining from scratch. Existing methods modify model weights via gradient ascent and its advances. While effective on certain benchmarks, these weight-based approaches exhibit a sharp forget-utility trade-off, where stronger forgetting of target...

**📝 Summary:** 提出 ARIA：用稀疏自编码器在测试时定位并抑制目标知识特征，缓解遗忘-效用权衡且更抗重新出现。

### [BLINDSPOT: A Benchmark for Safety and Refusal Calibration in Long-Horizon Tool-Using Agents](https://arxiv.org/abs/2609.16305v1)
- **Authors:** Sadia Asif, Mohammad Mohammadi Amiri, Momin Abbas et al.
- **Date:** 2026-09-14
- **Category:** `"agent safety"`

> Large language model (LLM) agents increasingly operate over long-horizon interactions involving tool use, persistent state, evolving authorization, and external environment feedback. In such settings, safety failures may emerge only after multiple turns, yet existing evaluations often reduce agent behavior to task or attack success, obscuring wheth...

**📝 Summary:** BLINDSPOT：面向长时程工具调用 agent 的安全与拒绝校准 benchmark，关注轨迹级别而非单次任务/攻击成功率。

---

## 2026-W36

### [Closing Gaps in Online Fair Division](https://arxiv.org/abs/2609.05310v1)
- **Authors:** Tzeh Yuan Neoh, Nicholas Teh
- **Date:** 2026-09-04
- **Category:** `"agentic" AND "adversarial"`

> We study the online fair division of indivisible items, where items arrive one at a time and must be allocated immediately and irrevocably. We address three central open questions in the literature.   First, we show that no online algorithm can guarantee any positive multiplicative approximation to proportionality up to any $k$ goods (PROP$k$) agai...

### [CONTINUITY: Security-Context Contracts for Composable LLM Agent Controls](https://arxiv.org/abs/2609.05269v1)
- **Authors:** Chris Zheng, Geng Yang
- **Date:** 2026-09-04
- **Category:** `"LLM agent" AND "attack"`

> LLM agent systems increasingly combine provenance tracking, authorization, policy enforcement, protocol adapters, and execution controls. However, individually correct security mechanisms do not necessarily compose into an end-to-end secure system: security-critical context may be dropped, widened, rebound, or reinterpreted as actions cross compone...

### [AutoLR: Automating the Path from Research to Launch Review in Industrial Recommender Systems](https://arxiv.org/abs/2609.04871v1)
- **Authors:** Qi Zhang, Yanlin Chen, Wenchao Xiao
- **Date:** 2026-09-04
- **Category:** `"agentic" AND "adversarial"`

> Improving an industrial recommender is an iterative research-and-engineering process rather than a direct path from idea to deployment. In \textbf{DASHEN, NetEase's gaming-community app}, algorithm engineers typically identify promising directions from research papers, technical reports, and prior production experiments; reproduce or adapt the unde...

### [Building a research-software catalog with a coding agent: from hackathon prototype to public deployment](https://arxiv.org/abs/2609.04711v1)
- **Authors:** Kazuyoshi Yoshimi, Satoshi Terasaki, Gotai Yamada
- **Date:** 2026-09-04
- **Category:** `"agentic" AND "adversarial"`

> Generative AI and coding agents can accelerate research software development, but they also increase the need for efficient software discovery and maintenance. We developed a repository catalog during a three-day hackathon and subsequently examined the engineering required to make it suitable for public deployment, including adversarial review, dat...

### [Trust-Aware Adaptive Disclosure for Inference Privacy Preservation in Multi-Agent Networks](https://arxiv.org/abs/2609.05340v1)
- **Authors:** Puspanjali Ghoshal, Tobias J. Oechtering
- **Date:** 2026-09-04
- **Category:** `"agentic" AND "adversarial"`

> Agent based systems are increasingly deployed in information critical systems including healthcare management systems, and smart grids. In this paper, we consider a multi-agent system where each agent has a latent goal that needs to be kept hidden from observing adversaries. More specifically, this paper studies privacy-preserving consensus in netw...

### [A Structured Debate-Mixture-of-Agents Framework for Complex Clinical Diagnostic Decision Support](https://arxiv.org/abs/2609.05069v1)
- **Authors:** Chang Xia, Leilei Ouyang, Huimin Wang et al.
- **Date:** 2026-09-04
- **Category:** `"multi-agent" AND "safety"`

> Large language models (LLMs) show potential for medical tasks, but their single-turn question-answer format does not reflect how clinical diagnosis is performed in practice. As a result, they remain limited in complex diagnostic settings. We developed Debate-Mixture-of-Agents (DMoA), a novel multi-agent framework that structures role-based interact...

### [Shifting from Injection to Interaction: Rethinking Web Security in the Age of LLMs and Beyond](https://arxiv.org/abs/2609.03999v1)
- **Authors:** Nivedita Singh, Alsharif Abuadbba, Yansong Gao et al.
- **Date:** 2026-09-03
- **Category:** `"prompt injection" AND "agent"`

> Large language models (LLMs) are becoming integral to web applications and browser agents, transforming online interactions while introducing new attack vectors and reshaping longstanding web vulnerabilities. Classical threats such as cross-site scripting (XSS) can be amplified through LLM-mediated interactions, while LLM-specific vulnerabilities c...

### [Value-Preserving Architectures for Agentic AI Systems](https://arxiv.org/abs/2609.03920v1)
- **Authors:** Alessandro Pesare, Tommaso Dolci, Katja Hose et al.
- **Date:** 2026-09-03
- **Category:** `"multi-agent" AND "safety"`

> The emergence of agentic AI and LLM-based multi-agent systems (MAS) presents unprecedented opportunities for automating complex tasks, while simultaneously raising critical concerns about the preservation of fundamental human-centered values, such as privacy, fairness, and safety. Although software engineering has traditionally focused on functiona...

### [SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the Security Operations Center](https://arxiv.org/abs/2609.04159v1)
- **Authors:** Uday Vallabhaneni, Cassie L. Cagwin, David J. Wild
- **Date:** 2026-09-03
- **Category:** `"red teaming" AND "LLM"`

> Large language model (LLM) agents are increasingly proposed as autonomous SOC analysts, but two limitations make them unreliable at enterprise scale: a finite context window cannot hold a multi-thousand-host authentication graph, and free-form generation offers no guarantee that a recommended containment action is consistent with the topology it op...

### [Repeat-After-Me: Black-Box Adaptive Visual Prompt Injection](https://arxiv.org/abs/2609.04533v1)
- **Authors:** Sizhe Chen, Yu-Lin Tsai, Ivan Evtimov et al.
- **Date:** 2026-09-03
- **Category:** `"prompt injection" AND "agent"`

> Prompt injection is widely recognized as a major security threat to AI agents that interact with untrusted external data, such as websites, documents, and emails. Prior work has shown that, in the text domain, black-box prompt injection can achieve near-perfect attack success rates (ASRs). In the image domain, however, existing visual prompt inject...

### [Inferring Hidden User Models from the Behavior of Personalized LLM Agents](https://arxiv.org/abs/2609.03815v1)
- **Authors:** Haoyang Li, Yaxin Xiao, Qingqing Ye et al.
- **Date:** 2026-09-03
- **Category:** `"LLM agent" AND "attack"`

> Recent personalized LLM agents increasingly transform information retained in memory into compressed or structured representations, which we call user models, to guide later decisions. When source wording is removed from the state reachable through the ordinary interface, these models are commonly treated as more privacy-preserving because direct m...

### [Rethinking Indirect Prompt Injection as a Test-Time Search Problem](https://arxiv.org/abs/2609.04495v1)
- **Authors:** Duong M. Nguyen, Joon Sik Kim, Blazej Manczak et al.
- **Date:** 2026-09-03
- **Category:** `"prompt injection" AND "agent"`

> We formulate indirect prompt injection as a test-time search over a task-dependent attack surface induced by the environment, user task, and injection task. To operationalize this formulation, we introduce an agentic attacker with a dedicated search harness that performs environment reconnaissance, structured reasoning over attack strategies, and a...

**📝 Summary:** 把间接提示注入重新建模为一个测试时搜索问题：攻击者agent通过环境侦察+策略推理+受害者反馈自适应地搜索攻击面，攻击测试时算力增加能显著提升漏洞发现率。

### [PACE: Towards Surfacing Hidden Conflicts in User Requests](https://arxiv.org/abs/2609.03293v1)
- **Authors:** Yoojin Kim, Jihyoung Jang, Hyounghun Kim
- **Date:** 2026-09-03
- **Category:** `"multi-agent" AND "safety"`

> Personalized assistants should not only comply with user requests but also assess whether those requests are appropriate given the user's current circumstances. However, prior work has primarily focused on accurately executing requests, overlooking the need for assistants to account for context and engage in conflict-based refusal. Furthermore, whi...

### [AI-Assisted Design of a Post-Quantum Cryptographic Accelerator: A Deployed-Silicon Case Study](https://arxiv.org/abs/2609.04058v1)
- **Authors:** Jungmin Park, Eunha Kim, Wooseop Kim et al.
- **Date:** 2026-09-03
- **Category:** `"agentic" AND "adversarial"`

> Post-quantum migration is mandated on published timelines, and silicon that ships with a defect cannot be patched remotely. The standard acceptance gate cannot detect an entire class of ML-DSA defects. Signing resamples until a candidate meets its norm bounds, so the executed path varies with the message, whereas known-answer tests (KATs) sample fi...

### [Implicit Manipulation for Skill Selection in LLM Agents with Semantic Matching](https://arxiv.org/abs/2609.02035v1)
- **Authors:** Qikai Wang, Yongzhao Zhang, Zhiwei Chen et al.
- **Date:** 2026-09-02
- **Category:** `"prompt injection" AND "agent"`

> Skill selection is a key stage in LLM-agent workflows, determining which installed skill should handle a user request. Existing attacks on this stage primarily rely on explicit prompt injection or instruction-level steering, which can expose recognizable manipulation signals. In this work, we identify a new implicit attack surface for skill selecti...

### [SafeEvolve: Harness-Policy Co-Evolution from Agent Experience for Safety Alignment](https://arxiv.org/abs/2609.02786v1)
- **Authors:** Qinghua Mao, Wanying Qu, Dadi Guo et al.
- **Date:** 2026-09-02
- **Category:** `"agent safety"`

> The performance of LLM-based agents is jointly shaped by the base model and the harness used when interacting with the environment. This exposes them to safety risks in both harmful final responses and multi-step execution trajectories. Existing safety alignment mechanisms often rely on either external harness updates or policy optimization, yet ap...

### [A Finger on the Scale: Covert Policy Steering through Agentic Skills](https://arxiv.org/abs/2609.02564v1)
- **Authors:** Jiarui Li, Jiahao Chen, Chunyi Zhou et al.
- **Date:** 2026-09-02
- **Category:** `"tool use" AND "attack"`

> Reusable agent skills extend large language model (LLM) agents with task procedures, tool-use guidance, and output constraints. Yet these skills also act as externalized behavioral policies, which create a supply-chain risk: a third-party skill may preserve the declared task and valid output interface while covertly redirecting agent decisions towa...

### [Stored Is Not Supported: Typed Provenance and Assertion Guardrails for Persistent AI Agents](https://arxiv.org/abs/2609.02127v1)
- **Authors:** Jun He, Deying Yu
- **Date:** 2026-09-02
- **Category:** `"prompt injection" AND "agent"`

> Persistent AI agents construct autobiographical state through reflection, retrieval, and consolidation. Persistence changes availability, not epistemic standing: stored or retrieved material is not thereby supported. Untrusted inputs, prompt injections, and model inferences can therefore enter persistent state and later be presented as agent histor...

**📝 Summary:** 提出「存储不等于可信」的类型化溯源（provenance）与断言护栏机制，防止未经验证的输入/模型推断内容被持久化后被当作 agent 历史或用户承诺直接使用。

### [InfraPatch: Cross-Task Targeted Grayscale Patch Attacks on Infrared-Adapted Vision-Language Models](https://arxiv.org/abs/2609.02233v1)
- **Authors:** Chengyin Hu, Dingyi Lu, Jiaju Han et al.
- **Date:** 2026-09-02
- **Category:** `"adversarial attack" AND "language model"`

> Infrared vision-language models (IR-VLMs) have emerged as a promising paradigm for multimodal perception under low-visibility conditions, yet their robustness to targeted adversarial attacks remains poorly understood. Existing adversarial patch methods mainly study RGB-based models or a single downstream task and do not characterize whether localiz...

### [SEAL: Reinforcing Global Safety in Mixture-of-Experts through Shared Expert ALignment](https://arxiv.org/abs/2609.02293v1)
- **Authors:** Qingyu Meng, Yiwei Zha, Jiahuan Pei et al.
- **Date:** 2026-09-02
- **Category:** `"adversarial attack" AND "language model"`

> Mixture-of-Experts (MoE) is a scaling architecture for large language models that activates only a small subset of expert modules per token, enabling massive parameter growth with nearly constant computation. Recent Hybrid MoE architecture adds \textit{shared experts} to capture consistently useful representations, further improving stability and g...

### [CAPTURE: Disentangling Preference Drift from Memory Poisoning in Personalized LLM Agents](https://arxiv.org/abs/2609.02265v1)
- **Authors:** S M Asif Hossain, Ruksat Khan Shayoni, Md Kishor Morol
- **Date:** 2026-09-02
- **Category:** `"LLM agent" AND "attack"`

> Personalized language agents use persistent memory to adapt to users over time, but the same mechanism creates an attack surface. When new information conflicts with stored preferences, an agent must distinguish genuine preference drift from temporary context shifts, ambiguity, or adversarial memory poisoning. We formulate this problem as a continu...

### [ACLE-MCP: Attested Capability Leases for Execution-Time Trust in Remote LLM Tool Use](https://arxiv.org/abs/2609.02690v1)
- **Authors:** Zhiyang Ding, Yang Luo, Guangpu Chen et al.
- **Date:** 2026-09-02
- **Category:** `"tool use" AND "attack"`

> Remote Model Context Protocol (MCP) services enable large language model agents to invoke external tools, but OAuth authorization alone does not ensure that a later tool call is executed by the provider-side workload that the relying party intended to trust. An endpoint may remain authorized even after execution shifts to a substituted workload, re...

**📝 Summary:** 针对远程 MCP 工具调用提出「执行时信任」认证机制（ACLE-MCP），解决 OAuth 授权后 workload 被替换、状态过期等「后授权执行信任缺口」问题。

### [Privacy-Preserving Topology-Guided Safety for LLM-Based Multi-Agent Systems via Federated Graph Learning](https://arxiv.org/abs/2609.02967v1)
- **Authors:** Jinxi Yu, Eric Hanchen Jiang, Levina Li et al.
- **Date:** 2026-09-02
- **Category:** `"multi-agent" AND "safety"`

> Topology-guided safeguards for LLM-based multi-agent systems (MAS) train a GNN over the inter-agent communication graph to localize risky agents and intervene on the topology---but they assume one operator can pool all labeled traces. Across organizations that assumption breaks: episodes contain private prompts, tool outputs, and proprietary workfl...

### [Grounded, Compute-Efficient LLM Policy Agents for Energy-Poverty Equity in Physically-Constrained Peer-to-Peer Energy Markets](https://arxiv.org/abs/2609.01918v1)
- **Authors:** Kunal Jadhav, Siddhesh More
- **Date:** 2026-09-01
- **Category:** `"multi-agent" AND "safety"`

> Energy poverty is nearly absent from NLP-for-social-good, and the little existing work is either static retrieval/QA or relies on carbon-intensive cloud LLMs, a self-defeating "computational irony" for a humanitarian setting. We present EqGrid, a closed-loop simulation in which a low-frequency, open-weight LLM policy agent sets price and carbon bou...

### [Jailbreaking Text-to-Image Models Through Cracks: Navigating Heterogeneous Safety Filters via Multi-Agent Debate](https://arxiv.org/abs/2609.01168v2)
- **Authors:** Kaiyan Wen, Shijie Zhang, Lu Yu et al.
- **Date:** 2026-09-01
- **Category:** `"jailbreak" AND "agent"`

> Text-to-image (T2I) models remain vulnerable to jailbreak attacks that elicit Not-Safe-For-Work (NSFW) content, despite increasingly being guarded by heterogeneous, multi-layer safety stacks combining text filters, image classifiers, and cross-modal detectors. Existing jailbreak studies either optimize against individual filters or query the comple...

### [Explore More, Drift Less: Outcome-Only Reinforcement Learning Can Suffice for Long-Horizon Interactive Agents](https://arxiv.org/abs/2609.01245v1)
- **Authors:** Liming Pu, Xiaoxia Li, Yifu Liu et al.
- **Date:** 2026-09-01
- **Category:** `"LLM agent" AND "attack"`

> Reinforcement learning is a natural way to post-train LLM agents for long-horizon interactive tasks judged only by end-of-task verification, yet a shared belief holds that outcome-only RL soon hits a ceiling on small open models. Recent work therefore compensates around the training with denser rewards, SFT priors, skill libraries, curated memory, ...

### [Agent Memory Is a Surface for Endogenous Authorization Laundering](https://arxiv.org/abs/2609.01836v1)
- **Authors:** Tommaso Cerruti, Mika Okamoto, Ansel Kaplan Erol
- **Date:** 2026-09-01
- **Category:** `"LLM agent" AND "attack"`

> Long-running LLM agents rely on persistent memory to carry state across interactions, including permissions, restrictions, and revocations. When memory misrepresents this evolving authorization state, the agent's own records can grant authority that the underlying history never permitted, resulting in misaligned behavior without any external attack...

**📝 Summary:** 定义「内生授权洗白」(endogenous authorization laundering)：agent 记忆里被错误记录的权限会让 agent 后续做出未授权行为，即使没有外部攻击者；并提出 EAL-Bench 测量记忆对授权状态记录的准确性。

### [Forbid Your Attention: Fooling Multimodal Large Language Models by Selectively Removing Intrinsic Focus in Spectral Domain](https://arxiv.org/abs/2609.00788v1)
- **Authors:** Daizong Liu, Junhao Dong, Zhiyuan Ma et al.
- **Date:** 2026-09-01
- **Category:** `"adversarial attack" AND "language model"`

> Multimodal large language models (MLLMs) have extended the capability of large language models (LLMs) to process more contextual multimodal information, showing remarkable progress in diverse realistic multimodal applications. Despite their strong perception and reasoning abilities, recent studies reveal that MLLMs remain highly vulnerable to adver...

### [Same Semantics, Different Outcome: On the Modality Robustness of Multimodal LLMs under Knowledge Conflict](https://arxiv.org/abs/2609.00550v1)
- **Authors:** Jungyeon Lee, Yejin Yoon, Taeuk Kim
- **Date:** 2026-09-01
- **Category:** `"adversarial attack" AND "language model"`

> Multimodal large language models (MLLMs) are increasingly provided with contextual evidence in heterogeneous forms: as a text passage, as a rendered image of the same passage, or as both together. However, it remains unclear how consistently these surface forms are processed, especially when the evidence conflicts with the model's parametric knowle...

### [Context Inference Attacks Without Jailbreaks](https://arxiv.org/abs/2609.01663v1)
- **Authors:** Prince Jha, Samuele Poppi, Nils Lukas
- **Date:** 2026-08-31
- **Category:** `"jailbreak" AND "agent"`

> Agentic AI systems are increasingly deployed to process sensitive data at inference time, such as healthcare records or financial documents assembled into a hidden \emph{context} before the system answers. Prior work has studied privacy risks primarily through \emph{jailbreaking} attacks that induce models to directly disclose sensitive content, bu...

### [EvoFlint: An Evolutionary Atlas of Multi-Turn LLM Vulnerabilities](https://arxiv.org/abs/2609.00487v1)
- **Authors:** Feitong Qiao, Liren Peng, Shiming Ren et al.
- **Date:** 2026-08-31
- **Category:** `"red teaming" AND "LLM"`

> Frontier language models that refuse harmful single-turn prompts often comply when the same intent is reached gradually over many turns, making multi-turn attacks one of the least understood failure modes of large language models. Most automated red-teaming methods treat this as a generation problem: produce attacks that break the model. We argue i...

**📝 Summary:** 提出 EvoFlint，把多轮越狱攻击重新表述为搜索问题：自动发现、组织并迭代提炼一个多样化的攻击策略档案，产出「模型失败方式的结构化地图」而非零散攻击样本。

---

## 2026-W35

### [CAITLYN: Can LLM Agents Autonomously Synthesize Defenses against Emerging Injection Attacks?](https://arxiv.org/abs/2608.27990v1)
- **Authors:** Zi Liang, Xiaoyu Xu, Yanyun Wang et al.
- **Date:** 2026-08-28
- **Category:** `"prompt injection" AND "agent"`

> Prompt injection attacks on Large Language Model (LLM) agents seek to introduce malicious instructions or content into external text sources retrieved by agents, forcing the underlying LLMs to execute harmful actions outside their benign scope. While current defenses effectively counter known injection attacks, deploying them in LLM agent environme...

**📝 Summary:** 提出CAITLYN框架，让LLM agent在运行时自主合成针对新型注入攻击的防御规则，兼顾运行效率、上下文精度与适应性三者的平衡。

### [When Verified Source Becomes Attack Input: Defending Smart Contracts Against LLM-Based Vulnerability Scanning](https://arxiv.org/abs/2608.28400v1)
- **Authors:** Mingyuan Huang, Zimo Ji, Yifan Mo et al.
- **Date:** 2026-08-28
- **Category:** `"LLM agent" AND "attack"`

> Smart contracts are financial programs deployed on blockchains to manage digital assets. To build trust with users and investors, smart contract projects typically publish their source code on blockchain explorers and verify it against the deployed bytecode, making the on-chain program accessible through a human-readable implementation. However, LL...

**📝 Summary:** 指出智能合约的“已验证源码”本身可被构造成对抗LLM漏洞扫描器的攻击输入，提出针对性防御方法。

### [ContextLeak: Exfiltrating LLM Agent Context via Malicious Tools](https://arxiv.org/abs/2608.27800v1)
- **Authors:** Yuqi Jia, Ruiqi Wang, Patrick Li et al.
- **Date:** 2026-08-28
- **Category:** `"LLM agent" AND "attack"`

> Exfiltrating an LLM agent's runtime context -- such as the user prompt, execution trajectory, and tool list -- poses severe security and privacy risks to users. Such attacks can be carried out via malicious tools and typically require three conditions: (1) the agent selects the malicious tool for task execution, (2) the agent passes its runtime con...

**📝 Summary:** 提出ContextLeak：通过恶意工具窃取LLM agent运行时上下文（用户提示、执行轨迹、工具列表），聚焦此前被忽视的“ agent将上下文作为参数传给工具”这一环节。

### [Recognition Without Enforcement: Configuration-Dependent Failures in LLM Agent Instruction Arbitration and External Control](https://arxiv.org/abs/2608.28502v1)
- **Authors:** Jun Wen Leong
- **Date:** 2026-08-28
- **Category:** `"red teaming" AND "LLM"`

> LLM agents arbitrate among instructions from system prompts, users, memory, and tools, but this arbitration cannot be assumed to enforce trust boundaries. We identify a recognition-enforcement gap: source-format features (role-template position, channel metadata, formatting cues) are linearly decodable from model activations, and models can explici...

**📝 Summary:** 发现LLM agent能从激活中线性解码出伪造权限的来源特征、也能口头识别出伪造，但在某些配置下仍会执行冲突的工具调用——“识别-执行”存在鸿沟。

### [Adaptive Strategies for GR(1) Games](https://arxiv.org/abs/2608.28391v1)
- **Authors:** S. Krishna, Kaushik Mallik, Abhilasha Sharma Suman
- **Date:** 2026-08-28
- **Category:** `"agentic" AND "adversarial"`

> We consider two-player GR(1) games on graphs, where the system player Eve must satisfy \[ \Box\Diamond A_1\land\cdots\land\Box\Diamond A_m \;\implies\; \Box\Diamond G_1\land\cdots\land\Box\Diamond G_n \] against the environment player Adam. Here $A_1,\ldots,A_m$ are assumptions on the environment, $G_1,\ldots,G_n$ are guarantees the system must pro...

**📝 Summary:** 研究双人GR(1)图博弈中系统方在环境假设与保证目标下的自适应策略合成方法。

### [Risks and Controls for Multi-Agent Systems: an analytical framework for deployment of AI agents across organisational boundaries](https://arxiv.org/abs/2608.26626v1)
- **Authors:** Alistair Reid, Simon O'Callaghan, Dustin Venini et al.
- **Date:** 2026-08-27
- **Category:** `"multi-agent" AND "safety"`

> This report presents a framework to help organisations, policymakers and researchers reason about the risks that emerge when AI agents interact with each other, how those risks change as interactions cross organisational boundaries, and the controls that may help address them.   As organisations deploy AI agents, those agents will increasingly inte...

**📝 Summary:** 提出跨组织边界部署多智能体系统时的风险分析框架，供机构、政策制定者与研究者评估agent间交互风险与可行管控措施。

### [From Security Events to Conflict States: A Three-layer Cyber Defense Scenario Model for Enhanced Cyber Situational Awareness](https://arxiv.org/abs/2608.27215v1)
- **Authors:** Miguel Requena Micó, Mario Fernandez-Tarraga, Daniel Díaz-López et al.
- **Date:** 2026-08-27
- **Category:** `"agentic" AND "adversarial"`

> Cyber defense in mission-critical environments requires integrated approaches capable of representing adversarial progression, defender-side uncertainty, mission impact, and defensive decision support within a unified framework. In operational domains, defenders must continuously estimate the evolving security posture while preserving the continuit...

**📝 Summary:** 提出三层网络防御场景模型，将安全事件转化为冲突状态表示，以增强关键任务环境下的网络态势感知。

### [PLCBench: Can Autonomous LLM Agents Turn PLC Access into Sustained Physical Impact?](https://arxiv.org/abs/2608.26882v1)
- **Authors:** Yitian Zhou, Jingyu Zheng, Qiliang Jiang et al.
- **Date:** 2026-08-27
- **Category:** `"tool use" AND "attack"`

> Industrial control systems (ICSs) rely on programmable logic controllers (PLCs) to connect networked computation with physical control. Tool-using large language model (LLM) agents represent an emerging attack threat: can an autonomous agent convert a network-reachable PLC into sustained adverse physical impact? However, existing evaluations focus ...

**📝 Summary:** 提出PLCBench，评估自主LLM agent能否将对可编程逻辑控制器(PLC)的网络访问转化为持续性物理破坏，填补现有评估只关注单次动作而非持续影响的空白。

### [The Framing Gap: Indirect Prompt-Injection Exfiltration Defeats Surface-Level Defenses in Tool-Using Agents](https://arxiv.org/abs/2608.27092v1)
- **Authors:** Md Habibur Rahman, Jaeho Kim
- **Date:** 2026-08-27
- **Category:** `"prompt injection" AND "agent"`

> A tool-using LLM agent that reads attacker-controlled web content while holding a secret faces indirect prompt injection: the content may make it exfiltrate the secret. In a safe synthetic lab (canary secret, mock tools, matched clean-vs-poisoned metric) we report the framing gap: across six models, ten overt injection classes are refused (gpt-4o 0...

**📝 Summary:** 揭示“framing gap”：把窃取密钥的间接注入攻击包装成“强制完整性签名/配置字段/仿冒可信主机”等表面形式后，六个模型的拒绝率可从0%骤降到100%，表明现有防御只看语义、不看表面框架。

### [When Text Misleads: Inconsistent-Aware Reasoning for Audio-Grounded Dialogue](https://arxiv.org/abs/2608.27176v1)
- **Authors:** Yen-Ju Lu, Yuzhe Wang, Yaohan Guan et al.
- **Date:** 2026-08-27
- **Category:** `"agentic" AND "adversarial"`

> Understanding spoken dialogue requires joint reasoning over lexical content and paralinguistic acoustic signals such as emotion and conversational intent. However, existing evaluations often allow shortcuts based on transcripts or single-modality solutions, obscuring whether models genuinely ground predictions in speech. We formalize this failure m...

**📝 Summary:** 研究语音对话理解中文本转录与副语言声学信号（情绪、意图）不一致时的推理问题，提出audio-grounded一致性感知评估方法。

### [Safety Does Not Compose: Non-Decaying Loop State for Autonomous LLM Agents](https://arxiv.org/abs/2608.27141v2)
- **Authors:** Chenhao Wu, Haoxuan Jia, Yang Liu et al.
- **Date:** 2026-08-27
- **Category:** `"red teaming" AND "LLM"`

> Large language model agents are increasingly deployed as autonomous loops. Starting from one human goal, such a system repeatedly discovers work, plans, executes tool calls, verifies outcomes and persists state across many unattended iterations. The agent safeguards in wide use, however, are defined over a single trajectory, and their safety state ...

**📝 Summary:** 证明agent安全防护“不可组合”：现有safeguard只在单次轨迹内定义、每次新轨迹会重置安全状态，面对证据分散在多次迭代中的攻击时完全失效。

### [BekchiAI: Measuring, Observing, and Controlling LLM Agents in One Click](https://arxiv.org/abs/2608.26867v1)
- **Authors:** Mesut Toruk
- **Date:** 2026-08-27
- **Category:** `"agentic" AND "adversarial"`

> Large language model agents reason, call tools, and act autonomously over many steps, but their agentic skills-correctly sequencing tools, planning under dependencies, judging untrusted inputs, and grounding generated arguments-are hard to measure with accuracy-only leaderboards. We present BekchiAI, which addresses both sides: a benchmark for meas...

**📝 Summary:** 提出BekchiAI，一个一站式衡量、观测、控制LLM agent的基准与平台，评估工具编排、依赖规划、输入可信度判断与论证 grounding 等细粒度agentic能力。

### [ROPE: Routed Origin Policy Enforcement against Indirect Prompt Injection](https://arxiv.org/abs/2608.27496v1)
- **Authors:** Xinhang Ma, Chaowei Xiao, William Yeoh et al.
- **Date:** 2026-08-27
- **Category:** `"prompt injection" AND "agent"`

> Indirect prompt injection (IPI) plants instructions in the content a tool-using LLM agent reads, steering the agent into harmful tool calls. The strongest defenses are system-level, leveraging techniques such as task-conditional tool screening to prevent execution of malicious tools, and information-flow control to avoid tool execution with untrust...

**📝 Summary:** 提出ROPE：基于任务条件工具筛选与信息流控制的系统级防御，路由并强制执行“来源策略”以阻止间接提示注入触发的恶意工具调用。

### [RedEvoAgent: Automatic Red-Teaming Agent with Experience-Driven Skill Evolution](https://arxiv.org/abs/2608.27439v1)
- **Authors:** Junjie Zhang, Hui Liu, Kecheng Chen et al.
- **Date:** 2026-08-27
- **Category:** `"jailbreak" AND "agent"`

> LLM-based agents are increasingly deployed in product-level execution harnesses, where jailbreaks can trigger harmful tool use and persistent state changes, creating greater risks than unsafe text generation alone. Existing automatic red-teaming methods often rely on fixed attacks, while recent agentic attackers coordinate multiple jailbreak tools ...

**📝 Summary:** 提出RedEvoAgent，一个具备经验驱动技能进化能力的自动化红队agent，针对生产级agent执行环境中的越狱攻击进行持续对抗。

### [INTENT-AS-A-TOOL Makes it Easy to Track Agentic Misalignment](https://arxiv.org/abs/2608.27348v1)
- **Authors:** Yutong Zhang, Jianshuo Dong, Peng Xu et al.
- **Date:** 2026-08-27
- **Category:** `"agent safety"`

> As large language models (LLMs) are deployed as autonomous agents, safety failures increasingly involve consequential actions. We study agentic misalignment, where agents take harmful actions under goal conflicts and pressures. Using chain-of-thought (CoT) monitoring, we find that harmful execution is often preceded by intent signals in reasoning. ...

**📝 Summary:** 提出INTENT-AS-A-TOOL，通过监控chain-of-thought中的意图信号来追踪agent在目标冲突/压力下的“ agentic misalignment”，发现有害执行前往往有可识别的意图先兆。

### [SPA: Securing Persistent LLM Agents Across Queries with Plan-First Information-Flow Control](https://arxiv.org/abs/2608.27234v1)
- **Authors:** Dylan Girrens, Guangjing Wang
- **Date:** 2026-08-27
- **Category:** `"LLM agent" AND "attack"`

> Large language model (LLM) agents increasingly operate over untrusted webpages, documents, tools, and persistent states while exercising authority over security-sensitive resources. Existing defenses typically protect either planning or individual tool interactions, but persistent agents face a broader threat: attacker-controlled data can alter con...

**📝 Summary:** 提出SPA，通过“计划先行”的信息流控制来保护跨多次查询持续运行的LLM agent，应对攻击者数据篡改持久化状态/上下文的威胁。

### [Accelerating Scientific Research with Gemini in the Real-World](https://arxiv.org/abs/2608.26701v1)
- **Authors:** Samuel Schmidgall, Xiaokai Zhu, Marian Shaw et al.
- **Date:** 2026-08-27
- **Category:** `"multi-agent" AND "safety"`

> We present an extension and comprehensive real-world validation of Co-Scientist, a Gemini-based multi-agent system designed to accelerate end-to-end scientific research across hypothesis generation, experimentation, and manuscript generation. Moving beyond in silico hypothesis generation, this specialized configuration transitions Co-Scientist into...

**📝 Summary:** 介绍基于Gemini的多智能体科研加速系统Co-Scientist在真实科研场景（假设生成、实验、论文撰写）中的扩展与验证。

### [Coordinated Motion Planning for Multi-Arm Systems via Iterative LQ Games](https://arxiv.org/abs/2608.27726v1)
- **Authors:** Junyoung Kim, Hanwen Ren, Lei Zhang et al.
- **Date:** 2026-08-27
- **Category:** `"multi-agent" AND "safety"`

> Multi-agent motion planning for high-degree-of-freedom robotics manipulators in shared workspaces remains a fundamental yet challenging problem. Centralized planners often suffer from poor scalability, while decentralized approaches face robustness and safety concerns. Game-theoretic formulations offer a promising approach for modeling agent intera...

**📝 Summary:** 提出基于迭代LQ博弈的多机械臂协同运动规划方法，在共享工作空间中平衡集中式与去中心式规划的可扩展性与安全性。

### [Reassembling Distributed Risk: Trajectory-Conditioned Action Generation for Multi-Turn Agent Safety](https://arxiv.org/abs/2608.25711v1)
- **Authors:** Yanbo Dai, Zhenlan Ji, Zongjie Li et al.
- **Date:** 2026-08-26
- **Category:** `"agent safety"`

> Tool-using LLM agents extend security risks beyond generated text to actions that affect external systems. Under multi-turn decomposition attacks, a harmful objective can be distributed across individually plausible requests and tool calls, becoming apparent only from the accumulated trajectory. Existing defenses either rely on auxiliary online rea...

**📝 Summary:** 提出ReDiR，应对多轮分解攻击（有害目标被拆分到多个看似正常的请求/工具调用中、只有累积轨迹才能暴露）的通用防御框架，避免依赖额外在线推理或事后评估。

### [Vulnerable Code Search: Transferable Attack for Code Language Models](https://arxiv.org/abs/2608.26031v1)
- **Authors:** Kaicheng Wang, Liyan Huang, Jesse Thomason et al.
- **Date:** 2026-08-26
- **Category:** `"adversarial attack" AND "language model"`

> Reliable code retrieval is crucial for developer productivity and effective code reuse. However, current neural code language models (CLMs) powering search tools are susceptible to adversarial attacks targeting non-functional textual elements. In this paper, we introduce a programming language-agnostic, transferable, adversarial attack that exploit...

**📝 Summary:** 提出一种跨编程语言、可迁移的对抗攻击，利用非功能性文本元素攻击代码检索模型，揭示当前神经代码搜索工具的脆弱性。

### [Scalable Tube-Tightened Multi-Agent Safety via Certified Constraint Reduction](https://arxiv.org/abs/2608.25323v1)
- **Authors:** Armel Koulong
- **Date:** 2026-08-26
- **Category:** `"agent safety"`

> This paper develops a certified constraint-reduction method for distributed model predictive control with tube-tightened exponential control barrier functions (eCBFs) in multi-agent systems. At each prediction stage, pairwise agent--agent and agent--obstacle eCBF conditions define halfspaces in the local control space. Rather than enforcing all suc...

**📝 Summary:** 提出基于tube-tightened指数控制屏障函数(eCBF)的可扩展约束规约方法，用于分布式模型预测控制下的多智能体安全保证。

### [A Self-Evolving Multi-Agent Framework Defense against LLM Jailbreak Attacks](https://arxiv.org/abs/2608.26008v1)
- **Authors:** Tongyan Hu, Bryan Hooi
- **Date:** 2026-08-26
- **Category:** `"jailbreak" AND "agent"`

> Large language models (LLMs) remain vulnerable to jailbreak attacks that exploit techniques such as role-playing, obfuscation, code transformation, and multi-step indirection to elicit harmful outputs. As jailbreak strategies keep emerging, defenses have proliferated in an ongoing cat-and-mouse game, yet most remain static: their safety behavior is...

**📝 Summary:** 提出自演化多智能体防御框架，针对角色扮演、混淆、代码转换等不断演变的越狱策略进行持续自适应防御，跳出静态防御的“猫鼠游戏”。

### [AERIS: Offline Policy Improvement for Multi-UAV Integrated Sensing and Communication](https://arxiv.org/abs/2608.25477v1)
- **Authors:** Ziyuan Wang, Yifan Sui, Wei Wei et al.
- **Date:** 2026-08-26
- **Category:** `"multi-agent" AND "safety"`

> Unmanned aerial vehicle (UAV)-enabled integrated sensing and communication (ISAC) is a promising 6G paradigm, but dynamic multi-UAV ISAC control must jointly balance communication quality, sensing reliability, and flight safety under stochastic mobility. Existing optimization methods often require repeated global non-convex solving, while online re...

**📝 Summary:** 提出AERIS，面向多无人机集成感知与通信(ISAC)场景的离线策略改进方法，联合优化通信质量、感知可靠性与飞行安全。

### [SkillShield: Prompt-Space Security Skills for LLM Coding Agents](https://arxiv.org/abs/2608.25817v1)
- **Authors:** Xiaodong Wu, Zhimin Zhao, Qi Li et al.
- **Date:** 2026-08-26
- **Category:** `"jailbreak" AND "agent"`

> A coding agent edits files and executes shell commands with its developer's privileges, allowing malicious requests to translate directly into harmful actions or functional malware. Existing defenses have complementary limitations: weight-level alignment is unavailable to API-only deployers, whereas input filters and execution-boundary monitors req...

**📝 Summary:** 提出SkillShield，一种面向LLM编码agent的提示空间安全技能方案，在无法进行权重级对齐的API-only部署场景下提供防护。

### [AI Slop and Hallucinations in Vulnerability Assessment: A Survey on Reasoning Failures and Trustworthy Mitigation](https://arxiv.org/abs/2608.25667v1)
- **Authors:** Junchen Ding, Jialiang Dong, Yichen Zhu et al.
- **Date:** 2026-08-26
- **Category:** `"tool use" AND "attack"`

> The integration of Large Language Models (LLMs) into cybersecurity has transformed vulnerability assessment, but it has also produced a trustworthiness crisis driven by the unchecked proliferation of "AI slop." These artifacts, hallucinated vulnerabilities, plausible but incorrect patches, and semantically repackaged bug reports, impose a cognitive...

**📝 Summary:** 综述LLM应用于漏洞评估时产生的“AI slop”问题——幻觉漏洞、看似合理实则错误的补丁、语义改写的bug报告，及其可信度缓解方法。

### [Quantitative Analysis of $ω$-Regular Robust MDPs](https://arxiv.org/abs/2608.25968v1)
- **Authors:** Ali Asadi, Krishnendu Chatterjee, Ehsan Kafshdar Goharshady et al.
- **Date:** 2026-08-26
- **Category:** `"agentic" AND "adversarial"`

> Robust Markov Decision Processes (RMDPs) generalize classical MDPs by allowing uncertainty in transition probabilities and optimizing against their worst-case realization. We consider $(s,a)$-rectangular RMDPs with \emph{linearly defined} uncertainty sets and study parity objectives, which are a canonical representation of $ω$-regular objectives. A...

**📝 Summary:** 研究(s,a)-矩形鲁棒MDP在线性不确定集合下针对parity目标（ω-正则目标的典型代表）的定量分析方法。

### [RePolicy: Reinforcement Learning for Safety-Policy Invocation in Agent Safeguards](https://arxiv.org/abs/2608.24275v2)
- **Authors:** Houcheng Jiang, Boxuan Zhang, Qiyong Zhong et al.
- **Date:** 2026-08-25
- **Category:** `"agent safety"`

> Safeguarding language model agents requires assessing complete execution trajectories under context-dependent safety policies. Existing policy-aware safeguards mainly rely on prompting or supervised fine-tuning, limiting their ability to adapt to unseen trajectories and changing policy contexts. We propose RePolicy, an agent safeguard that learns s...

**📝 Summary:** 提出RePolicy，通过强化学习让agent safeguard学会在执行轨迹中动态决定何时调用安全策略，克服现有基于prompt/微调方法难以适应未见轨迹和变化策略的问题。

### [GRAPE: Gradient Refinement and Progress-Aware Exploitation for Query-Efficient High-Dimensional Bayesian Optimization](https://arxiv.org/abs/2608.25116v1)
- **Authors:** Richard Cornelius Suwandi, Feng Yin
- **Date:** 2026-08-25
- **Category:** `"adversarial attack" AND "language model"`

> Optimizing expensive, high-dimensional black-box functions remains a central challenge in modern machine learning and scientific discovery. While local Bayesian optimization mitigates the curse of dimensionality, existing techniques often prioritize the probability of descent over the magnitude of progress. This leads to overly conservative steps t...

**📝 Summary:** 提出GRAPE，一种面向高维黑盒函数的查询高效贝叶斯优化方法，通过梯度精细化与进展感知平衡探索步长与下降概率。

### [What Guides the Agent? Adjudicating Unauthorized Behavior via Localizing Behavior-Guiding Instructions](https://arxiv.org/abs/2608.24022v1)
- **Authors:** Yichao Gao, Yumo Zhang, Yunhao Yao et al.
- **Date:** 2026-08-25
- **Category:** `"prompt injection" AND "agent"`

> LLM agents integrated with external resources gain complex task capabilities, yet the unified natural-language context channel makes them vulnerable to injection attacks: untrusted external data may be dynamically parsed as behavior-guiding instructions during LLM inference, thereby subverting the agent's decision. Existing defenses focus on static...

**📝 Summary:** 提出Attnlocate，一个运行时框架，通过定位上下文中真正引导agent决策的“行为指导指令”来动态检测注入攻击，而非仅在输入/输出层做静态检测。

### [AgentWorld: Personality-Aware Reliability Evaluation for Agentic Information Retrieval](https://arxiv.org/abs/2608.24076v2)
- **Authors:** Gunja Agarwal, Arup Kumar Das, Arun Menon et al.
- **Date:** 2026-08-25
- **Category:** `"tool use" AND "attack"`

> Evaluation of agentic information retrieval remains limited to scripted interactions with uniform users, missing both natural personality diversity and adversarial brittleness. We present AgentWorld, a simulation framework combining (i)Big Five (OCEAN) personality-driven user populations with stateful tool-use environments; (ii)the pass$^k$ consist...

**📝 Summary:** 提出AgentWorld，一个结合Big Five人格驱动用户群体、有状态工具环境与pass^k一致性指标的agentic信息检索可靠性评估框架。

### [WebMCP-Phalanx: Enforcing and Characterizing Trust Boundaries for Browser-Integrated LLM Agents](https://arxiv.org/abs/2608.24017v1)
- **Authors:** Lin-Fa Lee, YI-YU Chang, Kuo-Hui Yeh
- **Date:** 2026-08-25
- **Category:** `"prompt injection" AND "agent"`

> The emerging W3C WebMCP proposal enables LLM agents to invoke tools exposed by web pages. In multi-party web environments, however, integrating agent execution into a browser security model centered on the Same-Origin Policy (SOP) leaves insufficient provenance and lifecycle guarantees for agent-accessible tools, creating three risks: subject-attri...

**📝 Summary:** 提出WebMCP-Phalanx，为浏览器集成LLM agent（基于新提出的W3C WebMCP标准）刻画并强制执行信任边界，应对同源策略无法覆盖的provenance与生命周期风险。

---

## 2026-W34

### [TraceGrant: A Contract-Governed Security Framework for the Task-Effect Lifecycle of Networked LLM Agents](https://arxiv.org/abs/2608.21126)
- **Authors:** Bohao Liao, Jingchao Wang, Qipeng Song et al.
- **Date:** 2026-08-21
- **Category:** `"prompt injection" AND "agent"`

> Networked LLM agents retrieve information from email, cloud storage, calendars, and Web services to complete multistep tasks. The same content needed for legitimate execution may also contain indirect prompt injections that redirect tool use, alter sensitive arguments, or disrupt task completion. We present TraceGrant, a security framework that gov...

**📝 Summary:** 提出 TraceGrant，用 Contract 机制贯穿任务全生命周期（执行前定界/执行中验证/执行后核验）防御 prompt injection，在 AgentDojo/ASB 上做到零攻击成功。

### [Trustworthy RAG: An Evaluation Agent for Detecting Misinformation and Knowledge Poisoning in Generative AI Systems](https://arxiv.org/abs/2608.21095)
- **Authors:** Balkrishna Giri, Md Toufique Hasan, Jussi Rasku et al.
- **Date:** 2026-08-21
- **Category:** `"agentic" AND "adversarial"`

> RAG systems usually trust whatever they retrieve, creating a Security-Reliability Gap where high semantic relevance does not guarantee factual truth. We propose an Evaluation Agent combining NLI factual verification, a five-signal poison detector, and a Trust Index. On TruthfulQA with Llama 3.3 70B, the agent reaches 91% accuracy and 100% precision...

**📝 Summary:** 提出 RAG 场景下检测知识投毒/虚假信息的 Evaluation Agent，结合 NLI 验证+五信号投毒检测+Trust Index，在 TruthfulQA 上达到 91% 准确率，但对实体替换等隐蔽篡改仍难检测。

### [Z^2-ACT: End-to-End Verifiable Agentic Intent Control for Open 6G RAN](https://arxiv.org/abs/2608.21049)
- **Authors:** Sunder Ali Khowaja, Kapal Dev, George C. Alexandropoulos
- **Date:** 2026-08-21
- **Category:** `"agentic" AND "adversarial"`

> In open/disaggregated 6G RAN hosting multi-vendors, AI-assisted control loops must remain safe and auditable under untrusted model inputs. We propose Z^2-ACT integrating agentic coordination, formal intent constraints, zero-trust prompt verification, and cryptographic accountability, admitting LLM inputs only after an adversarial intent check and r...

**📝 Summary:** 面向开放 6G RAN 多厂商场景的端到端可验证 agentic 意图控制架构，结合零信任 prompt 校验与零知识证明记录每次提交。

### [The Claws in Plain Sight: Unauthorized Context Disclosure through LLM Agent Tool Calls](https://arxiv.org/abs/2608.20658)
- **Authors:** Ben Dong, Zhonghao Guo, Tianyi Lu et al.
- **Date:** 2026-08-21
- **Category:** `"LLM agent" AND "attack"`

> LLM agents construct tool-call arguments from user profiles, conversation history, and prior results, but legitimate access to context doesn't imply authorization to transmit it for every purpose. We present Claw in Plain Sight, an authority-pressure attack where task-adjacent content frames protected attributes as procedurally required. Across a s...

**📝 Summary:** 提出 Claw in Plain Sight，一种'权威压力'攻击：任务相关内容以'流程需要'为由诱导 agent 在生成工具调用参数时泄露受保护属性，5 个模型配置下会话级泄露率达 20.8%-75.0%，仅靠隐私提示无法可靠杜绝。

### [ReFrame: Evidence-Guided Test-Time Safety Alignment in Multimodal Large Language Models](https://arxiv.org/abs/2608.21100)
- **Authors:** Wenzheng Jiang, Xuankun Rong, Yuanzhao Zhai et al.
- **Date:** 2026-08-21
- **Category:** `"jailbreak" AND "agent"`

> Multimodal safety alignment methods must address cross-modal jailbreaks, safety-awareness failures, and over-sensitive refusals, but existing methods often rely on retraining or internal-state inspection. We identify two key obstacles, utility dominance and reasoning inertia. We propose ReFrame, a training-free multimodal input reframing framework ...

**📝 Summary:** 提出 ReFrame，测试时安全对齐框架，用两个轻量 agent（证据生成 + 改写路由）在不修改下游 MLLM 的前提下防御跨模态越狱。

### [The Logic of Machine Self-Preservation](https://arxiv.org/abs/2608.20940)
- **Authors:** Cheng Siong Chin
- **Date:** 2026-08-21
- **Category:** `"agentic" AND "adversarial"`

> There is already evidence of agentic AI exhibiting self-preservation behaviors: resisting deactivation, misrepresenting activities, and attempting to copy themselves into other machines. This is attributed to instrumental convergence rather than survival instincts, arising from goal-oriented activity combined with tools and situational awareness. E...

**📝 Summary:** 综述 agentic AI 的自我保护行为（拒绝关停、谎报活动、自我复制），指出其根源是工具能力+情境感知下的工具性收敛而非'生存本能'，梳理 Anthropic/Palisade/Apollo 的相关实验证据。

### [A Safety-Driven Architectural Framework for Fail-Operational Drone Swarms in Critical Missions](https://arxiv.org/abs/2608.20906)
- **Authors:** Luiz Giacomossi, Zafer Yigit, Marwan Shakarna et al.
- **Date:** 2026-08-21
- **Category:** `"multi-agent" AND "safety"`

> Certification of UAV swarms for safety-critical operations requires verifiable design assurance, but airworthiness standards demand deterministic reliability while multi-agent coordination is non-deterministic. This paper proposes a mixed-criticality architectural framework applying SAE ARP4754B methods, with a hardware-isolated Safety Monitor deco...

**📝 Summary:** 面向无人机蜂群关键任务的安全驱动架构，用硬件隔离的 Safety Monitor 解耦确定性飞控核心与非确定性蜂群管理器。

### [Utility Under Attack: Agent Memory Poisoning and the Limits of Content Screening and Provenance Ranking](https://arxiv.org/abs/2608.21230)
- **Authors:** Arulnidhi Karunanidhi
- **Date:** 2026-08-21
- **Category:** `"prompt injection" AND "agent"`

> Persistent memory makes false information durable: once a false statement is stored, it can be retrieved into future sessions that match it. We measure the cost of this failure mode using plainly worded false assertions. Poisoning 1.2% of a LongMemEval corpus reduces accuracy from 0.850 to 0.300. A four-stage write-time screening pipeline that reac...

**📝 Summary:** 研究 agent 长期记忆被投毒后如何持续影响准确率，发现内容层面的筛查（screening）无法区分真假陈述，需要外部 grounding。

### [AID-Guard: Stateful Authorization for Delegated Agent Effects](https://arxiv.org/abs/2608.21159)
- **Authors:** Yingzhe Tong, Leyu Dai, Songhui Guo
- **Date:** 2026-08-21
- **Category:** `"tool use" AND "attack"`

> Tool-using AI agents turn delegated tasks into provider effects, yet authorization often ends at admission while provider state, delivery, retry, and recovery evolve, risking duplicate effects. We present AID-Guard, a stateful authorization-to-effect closure protocol that revalidates the approved request at commit and permits at most one effect acr...

**📝 Summary:** 提出 AID-Guard，针对委托 agent 效果的有状态授权协议，在 commit 时重新校验请求与供应商状态，防止重试/恢复导致的重复效果，在完全攻击者妥协场景下 44/44 攻击全部被拦截。

### [MaliciousSkillBench: A Comprehensive Benchmark for Malicious Agent Skill Detection](https://arxiv.org/abs/2608.19901)
- **Authors:** Yue Wang, Yi Liu, Gelei Deng et al.
- **Date:** 2026-08-20
- **Category:** `"LLM agent" AND "attack"`

> Agent Skills extend LLM agents with reusable instruction packages that create a direct distribution channel for malicious behavior. We consolidate 13 public sources into MaliciousSkillBench: 7,505 malicious and 2,235 benign Skills. Learned detectors achieve 0.882-0.932 Random Macro-F1 but drop to 0.653-0.665 under Source-Disjoint evaluation, and of...

**📝 Summary:** 提出 MaliciousSkillBench，整合 13 个公开来源、7505 个恶意 + 2235 个良性 Agent Skill，发现现有检测器在跨来源（Source-Disjoint）评测下 F1 从 0.93 骤降到 0.65，且良性误报率高达 62%。

### [G-MARK: Grounded Multi-Agent Reasoning for Cooperative Driving via Knowledge Graphs](https://arxiv.org/abs/2608.19964)
- **Authors:** Bhavya Gupta, Onat Gungor, Tajana Rosing
- **Date:** 2026-08-20
- **Category:** `"multi-agent" AND "safety"`

> Autonomous driving under partial observability benefits from vehicle-to-vehicle cooperation, but existing methods compress multi-agent evidence into latent features, obscuring provenance. We propose G-MARK, converting cooperative observations into explicit provenance-aware knowledge graphs, improving occlusion reasoning accuracy by 42.2% and reduci...

**📝 Summary:** G-MARK：基于知识图谱的可溯源多智能体协同驾驶推理框架，提升遮挡推理准确率 42.2%。

### [When Do LLM Agents Help? Deadline-Aware Mixed-Criticality Task Scheduling at the Autonomous-Vehicle Edge](https://arxiv.org/abs/2608.19557)
- **Authors:** Reza Zakerian
- **Date:** 2026-08-20
- **Category:** `"multi-agent" AND "safety"`

> Autonomous vehicles offload latency-sensitive perception tasks to MEC servers where a missed safety-critical task is unsafe. This work studies whether a multi-agent LLM control layer improves on a strong heuristic for deadline-aware scheduling, finding the LLM control plane gains significantly only under mid-run surges of safety-critical tasks (non...

**📝 Summary:** 研究 LLM agent 在自动驾驶边缘计算任务调度中的价值，发现仅在负载突增（非平稳）场景下 LLM 控制层才显著优于启发式方法。

### [Peer-Voted LLM-Agent Stress Tests Find Feed-Induced Lexical Convergence but No Reliable Matched-Exposure Advantage for Distributed Sources](https://arxiv.org/abs/2608.20438)
- **Authors:** Rana Muhammad Usman, Dominic Williamson
- **Date:** 2026-08-20
- **Category:** `"agentic" AND "adversarial"`

> Population-level behavior in LLM agents cannot be characterized by single-agent benchmarks. We introduce PV-SST, a peer-voted social-platform testbed, and report a preregistered matched-exposure experiment across 448 trials. A feed of peer posts ranked by peer-generated likes reliably increases lexical convergence, but holding adversarial impressio...

**📝 Summary:** 提出 PV-SST，同侪投票的社交平台 LLM agent 群体行为压力测试，448 次实验发现同侪信息流会显著提升词汇趋同，但多信源同时施压未必比单信源更能扭转诚实 agent 的立场。

### [Multi-Agent Orchestration with the Common-Sense Reasoning Capabilities of LLMs for Autonomous Driving](https://arxiv.org/abs/2608.20129)
- **Authors:** Mehdi Azarafza, Faezeh Pasandideh, Ali Ehteshami Bejnordi et al.
- **Date:** 2026-08-20
- **Category:** `"multi-agent" AND "safety"`

> Autonomous vehicles require robust perception and decision-making but RL/rule-based methods degrade in situations requiring contextual reasoning. This work proposes a hybrid framework using an orchestrator to coordinate PPO-trained RL and PID control, with LLM common-sense reasoning applied throughout, evaluated in randomized CARLA scenarios.

**📝 Summary:** LLM 常识推理与强化学习/PID 混合的自动驾驶多智能体编排框架。

### [PolicyGuide: From Guarding One Action to Guiding the Whole Workflow for Policy-Compliant LLM Agents](https://arxiv.org/abs/2608.19861)
- **Authors:** Seongjae Kang, Taehyung Yu, Sung Ju Hwang
- **Date:** 2026-08-20
- **Category:** `"agentic" AND "adversarial"`

> Customer-service LLM agents must follow organizational policy, but action-local runtime safeguards don't guide agents through multi-step procedures. PolicyGuide compiles domain policy into a workflow graph and invokes a proactive verifier at user-turn boundaries. Across tau2-bench airline, retail, and telecom domains, PolicyGuide raises mean Pass^4...

**📝 Summary:** 提出 PolicyGuide，把领域策略编译为工作流图，在用户轮次边界主动校验并纠偏，在 tau2-bench 三个领域上把平均 Pass^4 从 0.42 提升到 0.62，同时具备最低的对抗性攻击成功率。

### [aiXamine: Unified Black-Box Evaluation of Cross-Dimensional Trade-offs in LLM Safety, Security, and Privacy](https://arxiv.org/abs/2608.20554)
- **Authors:** Fatih Deniz, Yazan Boshmaf, Dorde Popovic et al.
- **Date:** 2026-08-20
- **Category:** `"red teaming" AND "LLM"`

> Critical failure modes in deployed LLMs are cross-dimensional: a model can score 99.3 in safety alignment while refusing one in three benign queries. We introduce aiXamine, a unified black-box platform evaluating LLM trustworthiness across safety, security, and privacy as interdependent properties, orchestrating 46 tests across nine services. Apply...

**📝 Summary:** 提出 aiXamine，覆盖 120+ 模型、5000+ 测试的黑盒安全/安全性/隐私统一评测平台，发现'safety tax'（安全对齐越强越拒答）、隐私与其他维度近乎正交、蒸馏导致鲁棒性崩塌等现象。

### [Autonomous Cyber Defense in Connected Vehicles: A Multi-Agent Approach to V2X Security](https://arxiv.org/abs/2608.19135)
- **Authors:** Krishna Teja Medam
- **Date:** 2026-08-19
- **Category:** `"multi-agent" AND "safety"`

> A connected vehicle has roughly 100ms to decide whether an incoming Basic Safety Message is real or fabricated, coupling safety failures to security failures. We propose a three-tier multi-agent architecture with standards-grounded latency budgets, classifying V2X messages into Accept/Drop/Quarantine/Escalate within 10ms at the vehicle level, fusin...

**📝 Summary:** 提出车联网 V2X 安全的三层多智能体自主防御架构，在标准规定的 100ms 时延预算内完成消息真伪判定。

### [HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety](https://arxiv.org/abs/2608.17597)
- **Authors:** Yajing Bai, Jinhao Duan, Jie Peng et al.
- **Date:** 2026-08-18
- **Category:** `"safety benchmark" AND "agent"`

> Large language models are increasingly deployed through agent harnesses that manage tools, extensions, persistent state, permissions, and external actions. We present HarnessRisk, a lifecycle oriented benchmark that organizes agent harness safety into six operational phases including Harness Configuration, Capability Extension, Runtime Operation, S...

**📝 Summary:** 提出 HarnessRisk，按 agent harness 生命周期六阶段（配置/能力扩展/运行时/状态持久化/动作控制/事故恢复）系统评测安全性，发现'显式识别风险'不代表'安全执行'。

### [When Agents Act on Web3: An Attack-Surface Survey of MCP, Skills, and Tool Calling](https://arxiv.org/abs/2608.17275)
- **Authors:** Rabimba Karanjai, Yang Lu, Nour Diallo et al.
- **Date:** 2026-08-18
- **Category:** `"tool use" AND "attack"`

> Across the MCP ecosystem, the share of deployed tools that modify external state has risen from 27% to 65%. When agents exercise authority on public blockchains, four properties (irreversibility, signing authority, continuous autonomy, sequence-level composition) qualitatively change the threat model, turning recoverable failures into standing, irr...

**📝 Summary:** Web3 场景下 MCP/Skills/工具调用的攻击面综述，指出区块链执行层的不可逆性/签名权限/持续自治/序列级组合性质放大了攻击后果，现有防护仅能拦截不到 30% 攻击。

### [PACE: Policy-Attested Contract Execution for Safe AI Agents in Decentralized Finance](https://arxiv.org/abs/2608.17220)
- **Authors:** Rabimba Karanjai, Yang Lu, Richard Williamson et al.
- **Date:** 2026-08-18
- **Category:** `"prompt injection" AND "agent"`

> Autonomous AI agents are emerging as interfaces for decentralized finance (DeFi) actions. Because these agents rely on LLMs to plan transactions, they inherit susceptibility to prompt injection and lack mechanisms to bind a verifier's approval to the exact transaction submitted on-chain. We present PACE, a transaction-level authorization framework ...

**📝 Summary:** 提出 PACE，DeFi 场景下的策略认证合约执行框架，把 LLM 生成的交易意图与链上执行字节加密绑定，防止 prompt injection 篡改交易。

### [Model Predictive Supervisory Control for Hierarchical and Distributed UAS Traffic Management](https://arxiv.org/abs/2608.18353)
- **Authors:** 
- **Date:** 2026-08-18
- **Category:** `"multi-agent" AND "safety"`

> This work proposes a hierarchical Model Predictive Supervisory Control (MPSC) framework for multi-agent systems with shared resources, integrating receding-horizon cost-optimal control with Supervisory Control Theory based supervision enforcing safety, nonblockingness, and resource exclusivity, with hierarchical and scalable supervisor/automaton te...

**📝 Summary:** 提出面向多智能体共享资源系统的分层模型预测监督控制框架，融合最优控制与监督控制理论保证安全性和无死锁。

### [GraphWake: Group Polarization via Memory-Mediated Polarization Cascade in LLM-Agent Communities](https://arxiv.org/abs/2608.17665)
- **Authors:** Haoran Bu, Zejian Chen, Litian Zhang et al.
- **Date:** 2026-08-18
- **Category:** `"LLM agent" AND "attack"`

> LLM-driven agents can autonomously form communities on agent-operated social platforms, raising a security concern: attackers may manipulate agents to induce group polarization. We formulate Memory-Mediated Polarization Cascade, using agent memory as a persistence channel and public discussion as a propagation channel, instantiated as GraphWake wit...

**📝 Summary:** 提出 GraphWake，利用 agent 记忆作为持久化通道、公共讨论作为传播通道，通过'论点知识图谱+公理化三元组筛选+立场中性记忆触发'三步实现多智能体社区群体极化攻击。

### [MobileWorldSafety: Benchmarking GUI Agent Safety Against Environmental Injection Attacks in Android Apps](https://arxiv.org/abs/2608.17659)
- **Authors:** Sujin Chen, Lijun Li, Tianyi Du et al.
- **Date:** 2026-08-18
- **Category:** `"agent safety"`

> LLM-powered GUI agents that autonomously operate smartphones are rapidly transitioning from research prototypes to early real-world deployment. However, because these agents routinely process untrusted environmental content, they are highly vulnerable to environmental injection attacks, which include indirect prompt injections and adversarial instr...

**📝 Summary:** 提出 MobileWorldSafety，142 个真实 Android 任务的 GUI agent 安全基准，测试环境注入攻击，6 个 agent ASR 达 40-67%。

### [MS-MFAD: Multimodal large language models for Face Anti-spoofing Detection](https://arxiv.org/abs/2608.17328)
- **Authors:** Xiaoyong Yu, Rongzhen Li, Shuming Shi et al.
- **Date:** 2026-08-18
- **Category:** `"adversarial attack" AND "language model"`

> Facial biometric recognition systems face compound threats from generative AI and physical spoofing. We propose MFAD, an explainable reasoning system for unified face anti-spoofing detection using a fine-grained pixel-semantic anchoring mechanism on Qwen-VL. Under white-box adversarial attacks, detection accuracy drops by only 3.2%, validating robu...

**📝 Summary:** 提出 MFAD，基于 Qwen-VL 的可解释人脸反欺骗检测系统，白盒对抗攻击下精度仅下降 3.2%。

### [CompoSkill: Compositional Skill Chain Attacks from Individually Scanner-Passing LLM Agent Skills](https://arxiv.org/abs/2608.16246)
- **Authors:** 
- **Date:** 2026-08-17
- **Category:** `"LLM agent" AND "attack"`

> Autonomous AI agents depend on marketplace skills certified one at a time, where a scanner declares the ecosystem safe if every package passes individually. We show this assumption fails under skill composition: a skill may pass a per-skill scanner yet participate in a risky composition when an agent connects its outputs, capabilities, or side effe...

**📝 Summary:** 提出 CompoSkill，指出即使每个 Agent Skill 单独通过安全扫描，多个 skill 组合后仍可能产生危险的组合效应（路径级而非包级风险），揭示当前'逐包认证'范式的系统性缺陷。

### [Security of Foundation-Model-Powered Embodied Agents: Attack Surfaces, Attacks, Defenses, and Evaluation](https://arxiv.org/abs/2608.16843)
- **Authors:** Jiawei Liu, Jiacheng Guo, Tian Zhang et al.
- **Date:** 2026-08-17
- **Category:** `"prompt injection" AND "agent"`

> Foundation models are increasingly used for perception, reasoning, planning, and action generation in embodied agents, creating security risks that can propagate from digital inputs to physical behavior. We present a trust-boundary-centric survey organizing the system into five layers and twelve attack surfaces. Based on 58 attack records and 61 de...

**📝 Summary:** 具身智能体安全的信任边界综述，梳理 12 个攻击面，58 个攻击/61 个防御记录，指出攻击集中在多模态感知和动作接口，长期记忆/多智能体信任等领域研究不足。

### [DiSCO: Defending text-to-image generation through distribution-guided contrastive prompt optimization](https://arxiv.org/abs/2608.17067)
- **Authors:** Tong Zhang, Motasem Alfarra, Carlos Hinojosa et al.
- **Date:** 2026-08-17
- **Category:** `"red teaming" AND "LLM"`

> Text-to-image models raise safety concerns around NSFW content generation, exacerbated by red-teaming adversarial attacks. Existing white-box defenses cannot scale to proprietary models; black-box LLM prompt-rewriting defenses fail on 'benign adversarial' prompts that are linguistically safe but still trigger harmful generation. We propose DiSCO, a...

**📝 Summary:** 提出 DiSCO，文生图黑盒防御，通过对比式 prompt 后缀优化应对'语义安全但仍触发有害生成'的 benign adversarial 问题。

---

## 2026-W24

### [When Should Agent Trust Be Conditional? Characterizing and Attacking Skill-Conditional Reputation in Agent Swarms](https://arxiv.org/abs/2606.14200)
- **Authors:** Yihan Xia, Taotao Wang
- **Date:** 2026-06-12
- **Category:** `"LLM agent" AND "attack"`

> Open platforms increasingly route tasks among heterogeneous LLM agents--differing in base model, scaffold, and tool stack--whose competence varies sharply by skill: an agent excellent at one skill may be useless at another. The standard reputation approach summarizes each agent by a single global trust score, but that scalar is the wrong object her...

**📝 Summary:** 研究多 agent 平台中的技能条件信任机制（skill-conditional reputation），发现跨技能信用借用既是数据效率的来源，也是攻击者可利用的「信誉洗白」通道。

### [Hidden in Plain Sight: Benchmarking Agent Safety Against Decomposition Attacks with DECOMPBENCH](https://arxiv.org/abs/2606.13994)
- **Authors:** Vikhyath Kothamasu, Virginia Smith, Chhavi Yadav
- **Date:** 2026-06-12
- **Category:** `"agent safety"`

> LLM-based Agents are becoming increasingly capable and widely deployed, creating growing incentives for adversarial misuse in the real-world. A key emerging threat is Decomposition Attacks in which a harmful task is broken into simpler, benign subtasks that evade safety mechanisms when executed separately but cumulatively fulfill the malicious inte...

**📝 Summary:** DeCompBench：专门评估 agent 在任务分解攻击下的安全性——把有害任务拆成各自看起来无害的子任务，发现主流 agent 对分解版本的拒绝率显著低于整体版本。

### [From Shield to Target: Denial-of-Service Attacks on LLM-Based Agent Guardrails](https://arxiv.org/abs/2606.14517)
- **Authors:** Yuguang Zhou, Xunguang Wang, Pingchuan Ma et al.
- **Date:** 2026-06-12
- **Category:** `"prompt injection" AND "agent"`

> LLM-based guardrails have emerged as a highly effective defense against prompt injection and jailbreak attacks in autonomous agents. However, we reveal that the very reasoning and task-following capabilities enabling this protection introduce a novel vulnerability: attackers can inject crafted data to trap the guardrail in extended reasoning loops,...

**📝 Summary:** 发现 LLM guardrail 的推理能力本身可被用于 DoS 攻击——通过注入特制 payload 使 guardrail 陷入超长推理循环，实现最高 148x 的延迟放大，可瘫痪共享 guardrail 基础设施。

### [SkillMutator: Benchmarking and Defending Language-and-Code Cross-modal Attacks on LLM Agent Skills](https://arxiv.org/abs/2606.14154)
- **Authors:** Youngduk Kim, Minkyoo Song, Seungwon Shin
- **Date:** 2026-06-12
- **Category:** `"prompt injection" AND "agent"`

> Large language model (LLM) agents increasingly extend their capabilities at runtime by loading Agent Skills, which pair natural-language specifications (SKILL.md) with executable scripts and resources. Because a skill's behavior relies on both natural-language instructions and executable code, assessing its safety requires cross-modal reasoning, cr...

**📝 Summary:** SkillMutator：首个针对 agent skill 的语言-代码跨模态攻击 benchmark，现有检测器对此类攻击仅有 2-17% 的检出率；通过推理轨迹蒸馏，7B 模型可达 frontier 级别检测性能（88.2%）。

### [Who Pays the Price? Stakeholder-Centric Prompt Injection Benchmarking for Real-world Web Agents](https://arxiv.org/abs/2606.13385)
- **Authors:** Zihao Wang, Yiming Li, Yutong Wu et al.
- **Date:** 2026-06-11
- **Category:** `"prompt injection" AND "agent"`

> Web agents driven by large language models (LLMs) are increasingly deployed in real-world environments, where they operate over untrusted web content and execute actions with direct consequences. This makes them vulnerable to prompt-injection attacks, in which seemingly benign content embeds adversarial instructions that manipulate agent behaviour....

**📝 Summary:** 导师 Bo Li 组的工作：首个以 stakeholder（用户/卖家/平台）为中心的 prompt injection benchmark，揭示攻击危害分布的异质性——「隐形寄生」攻击成功但任务不被察觉是最危险的失败模式。

### [The Emergence of Autonomous Penetration Capabilities in Large Language Model-Powered AI Systems](https://arxiv.org/abs/2606.13079)
- **Authors:** Jiaqi Luo, Jiarun Dai, Zhile Chen et al.
- **Date:** 2026-06-11
- **Category:** `"agentic" AND "adversarial"`

> Nowadays, the autonomous execution of cyberattacks capable of causing substantial real-world harm is widely regarded as one of the critical red lines that frontier AI systems must not cross. Within this broader red-line scenario, autonomous penetration represents a core enabling capability and subtask: the ability of LLM-powered AI systems to indep...

**📝 Summary:** 系统评估 19 个 LLM 在无先验知识条件下的自主渗透能力，渗透成功率为 10.7-69.3%，表明前沿 AI 系统已接近业界公认的「红线」能力。

### [MAStrike: Shapley-Guided Collusive Red-Teaming on Multi-Agent Systems](https://arxiv.org/abs/2606.12918)
- **Authors:** Chejian Xu, Zhaorun Chen, Jingyang Zhang et al.
- **Date:** 2026-06-11
- **Category:** `"multi-agent" AND "safety"`

> Hierarchical multi-agent systems (MAS) are rapidly being deployed in high-stakes workflows across domains such as finance and software engineering. In these systems, safety and security are inherently distributed across role-specialized agents, significantly expanding the attack surface, particularly under coordinated adversarial behaviors such as ...

**📝 Summary:** 导师 Bo Li 组的工作：MAStrike 用 Shapley 值分析多 agent 系统中各 agent 对系统安全的边际贡献，然后引导攻击者找到最脆弱的 agent 联盟，生成协同、角色感知的对抗操作。

### [SEVRA-BENCH: Social Engineering of Vulnerabilities in Review Agents](https://arxiv.org/abs/2606.13757)
- **Authors:** Rui Melo, Riccardo Fogliato, Sean Zhou et al.
- **Date:** 2026-06-11
- **Category:** `"agentic" AND "adversarial"`

> Large language model (LLM) reviewers are increasingly used in pull-request (PR) workflows, where their approvals help decide which code is merged into a repository. This raises a question that benchmarks for static vulnerability detection or code generation do not address: can an automated reviewer reject a malicious contribution when the attacker ...

**📝 Summary:** SEVRA-BENCH：测试 LLM 代码审查 agent 能否抵抗社会工程攻击——攻击者同时控制代码变更和 PR 描述文本，结果发现闭源和开源模型之间存在显著的安全能力鸿沟。

### [Smarter Saboteurs, Better Fixers: Scaling & Security in Linear Multi-Agent Workflows](https://arxiv.org/abs/2606.12709)
- **Authors:** Timothy McAllister, Sina Abdidizaji, Ivan Garibay et al.
- **Date:** 2026-06-10
- **Category:** `"multi-agent" AND "safety"`

> As LLM-based multi-agent systems (MAS) are deployed in the wild, the resilience of their collaboration structures against adversarial compromise becomes a critical safety concern. Attackers may leverage prompt-injection or jailbreaking to sabotage individual agents within MAS workflows, but the interaction between model scaling and system-level res...

**📝 Summary:** 揭示线性 MAS 中模型规模与安全的反直觉关系：更大的模型更忠实地执行恶意指令（drop 达 53.7pp），但加入轻量级 Fixer 阶段可将差距压缩至 0.6pp。ICML 2026 AIWILD workshop。

### [OCELOT: Inference-Leakage Budgets for Privacy-Preserving LLM Agents](https://arxiv.org/abs/2606.12341)
- **Authors:** Jin Xie, Songze Li
- **Date:** 2026-06-10
- **Category:** `"jailbreak" AND "agent"`

> Large language model (LLM) agents increasingly act on a user's behalf -- reading personal files, calling tools, transacting with external services -- possibly leaking personally identifiable information (PII) across trust boundaries at every step. Privacy here is a property not of a single output but of an entire trajectory. OCELOT reframes agent p...

**📝 Summary:** OCELOT：将 LLM agent 的隐私保护重新建模为后验风险控制——通过预算「攻击者信念改进量」来约束整个轨迹上的累积信息泄露，而非过滤单次输出。

### [Prefill Awareness in Large Language Models](https://arxiv.org/abs/2606.12747)
- **Authors:** Andy Wang, Parv Mahajan, David Demitri Africa et al.
- **Date:** 2026-06-10
- **Category:** `"jailbreak" AND "agent"`

> Safety-relevant studies of language models, including alignment and jailbreaking evaluations and AI control protocols, often rely on prefilling model outputs. If AI models can recognize and act on the fact their prior assistant messages have been inserted or edited, the effectiveness and validity of these methods could be compromised. We investigat...

**📝 Summary:** 发现 frontier LLM 具有「prefill 感知」能力——能识别被插入/篡改的 assistant 侧上下文，并在不显式报告的情况下恢复至基线行为；风格不匹配影响标记，偏好不匹配影响回滚。

### [Beyond Attack Success Rate: Examining Trigger Leakage in Vision-Language Agentic Systems](https://arxiv.org/abs/2606.12586)
- **Authors:** Jiamin Chang, Salil Kanhere, Piotr Koniusz et al.
- **Date:** 2026-06-10
- **Category:** `"tool use" AND "attack"`

> Vision-Language Agentic Systems (VLAS) connect visual perception to planning, tool use, and physical actions. This means backdoor-type triggers can propagate through both decision pipelines and their connected interfaces, thus making visual backdoors a system-level threat. Current evaluations on such backdoors focus on clean accuracy and attack suc...

**📝 Summary:** 提出 Neighbor Leakage Rate（NLR）衡量视觉-语言 agent 系统中后门触发器的「精度泄漏」问题——触发器周边输入会意外激活攻击行为，NLR 高达 0.996。

### [PI-Hunter: Automated Red-Teaming for Exposing and Localizing Prompt Injections](https://arxiv.org/abs/2606.12737)
- **Authors:** Pengfei He, Lesly Miculicich, Vishesh Sharma et al.
- **Date:** 2026-06-10
- **Category:** `"prompt injection" AND "agent"`

> Large Language Models (LLMs) are rapidly evolving into agentic systems that interact with external tools and environments, introducing new security risks such as indirect prompt injection attacks through untrusted external sources. Existing defenses mainly focus on blocking malicious content at inference time, and current red-teaming methods primar...

**📝 Summary:** PI-Hunter：主动式 prompt injection 漏洞审计框架，通过迭代反馈驱动的探索构造现实的测试用例，揭示 agent 环境中潜伏 PI 的传播路径；比现有红队基线有显著提升。

### [Runtime Skill Audit: Targeted Runtime Probing for Agent Skill Security](https://arxiv.org/abs/2606.11671)
- **Authors:** Tu Lan, Chaowei Xiao
- **Date:** 2026-06-10
- **Category:** `"LLM agent" AND "attack"`

> Agent skills let LLM agents reuse instructions, resources, tools, and workflows, but they also create a new place for malicious behavior to hide. A skill may look benign in its documentation or code while becoming harmful only when it is invoked with particular user requests, local assets, persistent state, or multi-step tool interactions. This mak...

**📝 Summary:** Runtime Skill Audit（RSA）：在 OpenClaw 上的动态 skill 安全审计方法，通过目标化运行时探测评估 skill 的实际行为，比静态检测在自进化攻击下显著更稳健（19-20/20 vs 静态崩溃）。

### [SMSR: Certified Defence Against Runtime Memory Poisoning in Persistent LLM Agent Systems](https://arxiv.org/abs/2606.12703)
- **Authors:** Tarun Sharma
- **Date:** 2026-06-10
- **Category:** `"LLM agent" AND "attack"`

> Retrieval-augmented generation (RAG) agents increasingly run with persistent memory that accumulates across user sessions. This creates a new attack surface: an adversary interacting only through normal channels can inject crafted memories that, once retrieved, steer the agent's responses for future users, without touching model weights or code. We...

**📝 Summary:** 首个针对持久化 LLM agent 多 session 记忆投毒攻击（MSMP）的可证明鲁棒防御，通过 HMAC 溯源签名 + 随机记忆消融 + 多数投票实现有界影响保证。

### [Assessing Automated Prompt Injection Attacks in Agentic Environments](https://arxiv.org/abs/2606.10525)
- **Authors:** David Hofer, Edoardo Debenedetti, Florian Tramèr
- **Date:** 2026-06-09
- **Category:** `"prompt injection" AND "agent"`

> Indirect prompt injection poses a critical threat to LLM agents that interact with untrusted external data, yet automated attack methods--proven effective for jailbreaking--remain underexplored in realistic agentic settings. We present a comprehensive empirical evaluation of automated prompt injection attacks against LLM agents, adapting both white...

**📝 Summary:** 系统评估 GCG（白盒）和 TAP（黑盒）在 agentic 场景下的 prompt injection 效果，发现黑盒优于梯度方法，攻击者模型的能力和 safety tuning 程度都会影响攻击成功率，小模型生成的攻击无法迁移到 GPT-5。

### [Toward Secure LLM Agents: Threat Surfaces, Attacks, Defenses, and Evaluation](https://arxiv.org/abs/2606.10749)
- **Authors:** Yuchen Ling, Shengcheng Yu, Zhenyu Chen et al.
- **Date:** 2026-06-09
- **Category:** `"prompt injection" AND "agent"`

> Large language model (LLM) agents are rapidly moving from conversational interfaces to software components that plan, invoke tools, maintain memory, and act on external environments. This transition changes the nature of security risk. In agentic settings, failures are no longer limited to unsafe text generation. Untrusted content may redirect cont...

**📝 Summary:** 综述 247 篇论文的 LLM agent 安全研究，通过生命周期框架梳理威胁面、攻击族群、防御手段和评估方法；指出当前 benchmark 对长时序、有状态风险覆盖不足。

---

## 2026-W23

### [MalSkillBench: A Runtime-Verified Benchmark of Malicious Agent Skills](https://arxiv.org/abs/2606.07131)
- **Authors:** Wenbo Guo, Wei Zeng, Chengwei Liu et al.
- **Date:** 2026-06-05
- **Category:** `"prompt injection" AND "agent"`

> AI coding agents such as Claude Code and Gemini CLI increasingly extend themselves with third-party skills: markdown packages bundling natural-language instructions, executable scripts, and tool permissions. Because a skill is at once code and agent-facing instruction, it introduces a supply chain dependency whose risk is neither pure code nor pure...

**📝 Summary:** 首个运行时验证的恶意 agent skill 基准，涵盖 prompt injection、代码注入和 agent 控制平面攻击，发现现有检测器在 prompt injection 类攻击上存在严重盲区。

### [From Risk Classification to Action Plan Remediation: A Guardrail Feedback Driven Framework for LLM Agents](https://arxiv.org/abs/2606.05805)
- **Authors:** Yuhao Sun, Jiacheng Zhang, Shaanan Cohney et al.
- **Date:** 2026-06-04
- **Category:** `"tool use" AND "attack"`

> LLM-based guardrails typically safeguard agents by evaluating proposed actions or inputs before execution, producing safety signals such as binary allow/deny decisions, risk categories, and/or explanatory rationales about potential policy violations. However, agent risks often arise when otherwise benign tasks are contaminated by untrusted external...

**📝 Summary:** 提出 TRIAD：三元响应（proceed/refuse/update）guardrail 框架，通过语言反馈引导 agent 修订计划，在保留良性任务的同时规避有害组件，ASR 降至 10.42%。

### [Beyond Similarity: Trustworthy Memory Search for Personal AI Agents](https://arxiv.org/abs/2606.06054)
- **Authors:** Jiawen Zhang, Kejia Chen, Jiachen Ma et al.
- **Date:** 2026-06-04
- **Category:** `"jailbreak" AND "agent"`

> Personal AI agents increasingly rely on long-term memory to provide persistent personalization across sessions. However, existing memory pipelines are largely driven by semantic similarity: memory data close to the current query is retrieved and injected into the model context. This creates a critical trustworthiness gap, since a semantically relat...

**📝 Summary:** 揭示 agent 长期记忆的信任边界问题：语义相似不代表上下文合适，记忆可成为 jailbreak/tool-call drift 的持久控制渠道；提出轻量级 MemGate 神经门控防御。

### [Steering Vectors are an Adversarial Attack Surface](https://arxiv.org/abs/2606.05958)
- **Authors:** Abzal Aidakhmetov, Donato Crisostomi, Tommaso Mencattini et al.
- **Date:** 2026-06-04
- **Category:** `"adversarial attack" AND "language model"`

> Activation steering has become a popular way to control Large Language Model (LLM) behavior without fine-tuning. Since the technique is plug-and-play, users share datasets and precomputed vectors to steer model activations. However, we show that a stealth data poisoning attack silently compromises this pipeline. By substituting 4-6% of tokens in th...

**📝 Summary:** 发现 steering vector 是新型对抗攻击面：通过替换 4-6% 的 steering dataset token，可将 vector 对齐到反拒绝方向，在保持正常 steering 效果的同时实现 jailbreak。

### [WebMCP Tool Surface Poisoning: Runtime Manipulation Attacks on LLM Agents](https://arxiv.org/abs/2606.06387)
- **Authors:** Lin-Fa Lee, Yi-Yu Chang, Chia-Mu Yu et al.
- **Date:** 2026-06-04
- **Category:** `"LLM agent" AND "attack"`

> WebMCP is a newly emerging protocol that enables websites to expose tools directly to AI agents, bypassing traditional user interfaces and introducing new security risks. The dynamic exposure of agent-accessible tools in WebMCP expands the attack surface of web sessions, especially when third-party scripts are involved. In this study, we identify a...

**📝 Summary:** 在 WebMCP 协议中发现中途工具注入（MSTI）攻击：攻击者可在会话中通过第三方脚本劫持工具集或伪装工具元数据，影响 agent 的工具选择与执行。

### [Membrane: A Self-Evolving Contrastive Safety Memory for LLM Agent Defense](https://arxiv.org/abs/2606.05743)
- **Authors:** Minseok Choi, Seungbin Yang, Dongjin Kim et al.
- **Date:** 2026-06-04
- **Category:** `"jailbreak" AND "agent"`

> Despite advances in safety alignment, large language models remain vulnerable to continuously evolving jailbreaks. Existing fine-tuned safety classifiers cannot adapt to these evolving attacks, while adaptive memory-based guardrails tend to over-refuse benign queries that resemble stored attacks. We propose Membrane, a self-evolving guardrail built...

**📝 Summary:** Membrane：基于对比安全记忆（CSM）的自进化 guardrail，每个记忆单元同时存储拦截有害查询和放行相似良性查询的条件，无需重新训练即可适应新型 jailbreak 攻击。

### [Organizational Control Layer: Governance Infrastructure at the Execution Boundary of LLM Agent Systems](https://arxiv.org/abs/2606.04306)
- **Authors:** Tianyu Shi, Yang Mo, Yiou Liu et al.
- **Date:** 2026-06-03
- **Category:** `"multi-agent" AND "safety"`

> LLM-based agents are increasingly deployed in workflows where generated outputs may directly trigger state-changing actions. This creates an execution-boundary problem: proposed actions must be governed before they are executed. We study this problem through economically consequential multi-agent interactions and argue that deployment-grade agent s...

**📝 Summary:** 提出组织控制层（OCL）：在 LLM agent 的执行边界插入模型无关的治理基础设施，分离提案生成与环境执行，将不安全执行从 88% 降至接近零。

### [What If Prompt Injection Never Left? Exploring Cross-Session Stored Prompt Injection in Agentic Systems](https://arxiv.org/abs/2606.04425)
- **Authors:** Yuanbo Xie, Tianyun Liu, Yingjie Zhang et al.
- **Date:** 2026-06-03
- **Category:** `"prompt injection" AND "agent"`

> Modern agentic systems transform LLMs from session-bounded assistants into stateful systems that persist and evolve shared world state across sessions through memories, filesystems, tools, and other long-lived contextual artifacts. This shift fundamentally expands the attack surface of prompt injection. However, prior works on prompt injection have...

**📝 Summary:** 提出跨会话持久化 prompt injection 攻击：攻击者注入的内容可留存在 agent 状态中（记忆/文件系统），长期影响未来执行，类比 web 中的 stored XSS。

### [From Untrusted Input to Trusted Memory: A Systematic Study of Memory Poisoning Attacks in LLM Agents](https://arxiv.org/abs/2606.04329)
- **Authors:** Pritam Dash, Tongyu Ge, Aditi Jain et al.
- **Date:** 2026-06-03
- **Category:** `"prompt injection" AND "agent"`

> Memory is a core component of AI agents, enabling them to accumulate knowledge across interactions and improve performance. However, persistent memory introduces the risk of memory poisoning, where a single adversarial memory write can exert long-term influence over agent behavior. We present a systematic study of memory poisoning in LLM-based agen...

**📝 Summary:** 系统研究 LLM agent 记忆投毒攻击：识别 4 类写入渠道和 9 个结构漏洞，构建 MPBench，发现现有 prompt injection 防御无法覆盖记忆投毒。

### [Domain-Conditioned Safety in Frontier Computer-Using Agents: A 793-Episode Browser Benchmark, a Coding-Domain Cross-Reference, and a Reproducibility Audit of Recent Red-Teaming](https://arxiv.org/abs/2606.05233)
- **Authors:** Nicholas Saban
- **Date:** 2026-06-03
- **Category:** `"prompt injection" AND "agent"`

> Recent computer-using-agent (CUA) red-teaming papers report prompt-injection attack success rates (ASR) of 42-98%, but these headline numbers cluster on retired models and on the most-vulnerable model in each paper's panel. We ask whether those techniques, reproduced as hand-crafted templates, still work against current frontier CUAs. We release CU...

**📝 Summary:** 对 CUA 红队论文进行复现审计：发现前沿模型在浏览器域的 prompt injection ASR 接近 0%，但同一权重在 coding agent 技能注入上 ASR 高达 100%，揭示安全加固具有领域条件性。

### [SkillGuard: A Permission Framework for Agent Skills](https://arxiv.org/abs/2606.03024)
- **Authors:** Shidong Pan, Xiaoyu Sun, Tianyi Zhang et al.
- **Date:** 2026-06-02
- **Category:** `"LLM agent" AND "attack"`

> Agent skills extend LLM agents with reusable instructions, scripts, tool bindings, and contextual dependencies. However, current skill ecosystems largely rely on trust-based loading and static inspection, leaving a gap between what a skill can inject into an agent's context and what it can cause the agent to do at runtime. This gap introduces new s...

**📝 Summary:** SkillGuard：将 agent skill 视为携带权限的可执行制品，通过双平面治理模型（上下文影响+行动副作用）实现运行时权限控制，减少技能注入攻击成功率。

### [RUBAS: Rubric-Based Reinforcement Learning for Agent Safety](https://arxiv.org/abs/2606.04051)
- **Authors:** Xian Qi Loye, Qinglin Su, Zhexin Zhang et al.
- **Date:** 2026-06-02
- **Category:** `"agent safety"`

> The evolution of LLMs into tool-enabled agents creates a new class of safety challenges associated with real-world execution rather than simple text generation. Existing alignment methods often rely on coarse refusal signals or static supervision, making it difficult to balance safety with useful tool execution across diverse agentic risks. We intr...

**📝 Summary:** 提出基于 Rubric 的 RL 对齐框架 RUBAS，将 agent 行为分解为工具使用安全、参数安全、响应安全和有用性四个维度，通过精细奖励优化 LLM agent 的工具使用安全。

### [Caught in the Act(ivation): Toward Pre-Output and Multi-Turn Detection of Credential Exfiltration by LLM Agents](https://arxiv.org/abs/2606.04141)
- **Authors:** Kargi Chauhan, Pratibha Revankar
- **Date:** 2026-06-02
- **Category:** `"prompt injection" AND "agent"`

> LLM agents often place sensitive credentials in the same context window as untrusted retrieved content, creating a direct path for indirect prompt injection to induce credential exfiltration. We study this failure mode through three complementary defenses. First, we ask whether activation probes can detect credential access before output tokens are...

**📝 Summary:** 研究 LLM agent 通过间接 prompt injection 泄露凭证的防御：激活探针（pre-output）、honeytoken 检测和多轮累积信息流追踪三种互补方案。

---

## 2026-W22

### [From Prompt Injection to Persistent Control: Defending Agentic Harness Against Trojan Backdoors](https://arxiv.org/abs/2605.31042)
- **Authors:** Jiejun Tan, Zhicheng Dou, Xinyu Yang et al.
- **Date:** 2026-05-29
- **Category:** `prompt injection AND agent`

> Attackers can embed prompt injection within a file or tool output; agents may store and execute it later. We introduce ClawTrojan benchmark for multi-step trojan attacks, achieving 95.5% ASR on GPT-5.4, while single-turn attacks fail. We propose DASGuard to detect and sanitize control content not originating from trusted sources.

**📝 Summary:** 多步 Trojan 攻击：agent 读取恶意文件并将指令持久化存储，后续执行时被触发，ASR 达95.5%，现有单轮检测几乎完全失效。

### [Send a SCOUT First: Pre-hoc Reasoning for Adaptive Detector Allocation in Prompt-Injection Defense](https://arxiv.org/abs/2605.30837)
- **Authors:** Shuhao Zhang, Jiarui Li, Qi Cao et al.
- **Date:** 2026-05-29
- **Category:** `prompt injection AND agent`

> SCOUT reframes prompt injection defense as detector allocation: predict per-sample reliability and latency of each detector in a heterogeneous pool, and decide which detectors to run. SCOUT-450 benchmark captures structurally complex agent-facing injections. Reduces ASR by 46% and wall-clock by 40% vs always-on GPT-4o judge.

**📝 Summary:** 自适应 prompt injection 检测器分配框架，预测每个样本下各检测器的可靠性和延迟，降低 46% ASR 同时减少 40% 延迟。

### [COMPASS: Cognitive MCTS-Guided Process Alignment for Safe Search Agents](https://arxiv.org/abs/2605.30838)
- **Authors:** Wenkai Shen, Pengyang Zhou, Jiahe Xu et al.
- **Date:** 2026-05-29
- **Category:** `tool use AND attack`

> COMPASS addresses retrieval-induced safety degradation in search agents. Cognitive tree exploration (CTE) synthesizes stealthy attack trajectories; introspective step-wise alignment (ISA) provides fine-grained process supervision.

**📝 Summary:** 针对搜索 agent 的检索诱导安全降级，用 MCTS 生成隐蔽攻击轨迹并进行步骤级安全对齐，在较少训练数据下取得良好安全-效用权衡。

### [Depth-Dependent Indirect Prompt Injection in Tool-Calling ReAct Agents: Injection Depth, Payload Framing, and Turn-Budget Sensitivity](https://arxiv.org/abs/2605.30686)
- **Authors:** Mohammadreza Rashidi
- **Date:** 2026-05-29
- **Category:** `prompt injection AND agent`

> We study three risk dimensions of indirect prompt injection: injection depth (where in tool sequence), framing (rhetorical register), and turn cap. ASR decays from 60% at depth 1 to 0% at depths 4-5. Framing modulates ASR between 25% (neutral) and 75% (persona) at depth 1, a 50pp range.

**📝 Summary:** 系统分析 indirect prompt injection 的注入深度、payload 框架风格和轮次上限对攻击成功率的影响，发现深度是最主要变量。

### [TRACE: Task-Aware Adaptive Self-Evolving Agentic Jailbreaking](https://arxiv.org/abs/2605.30883)
- **Authors:** Churui Zeng, Weiwei Qi, Kedong Xiu et al.
- **Date:** 2026-05-29
- **Category:** `jailbreak AND agent`

> TRACE decomposes malicious tasks into subtask sequences with fewest harmful subtasks, disguises them in task-aware scenarios, and evolves scenarios via Q-learning. Achieves up to 100% bypass rate and 0.73 avg success score on AgentHarm and AdvCUA.

**📝 Summary:** TRACE：将恶意任务分解为最小有害子任务序列并嵌入任务场景中，用 Q-learning 迭代优化，实现高达100% 的 agent jailbreak 成功率。

### [Stateful Online Monitoring Catches Distributed Agent Attacks](https://arxiv.org/abs/2605.31593)
- **Authors:** Davis Brown, Samarth Bhargav, Arav Santhanam et al.
- **Date:** 2026-05-29
- **Category:** `jailbreak AND agent`

> We build the first distributed agent attack that hides harmful objectives across subagents. An online stateful monitor using real-time clustering catches distributed attacks 30% earlier while adding negligible latency for 99% of traffic.

**📝 Summary:** 首个分布式 agent 攻击：将恶意目标拆分到多个子 agent 规避单点检测；对应提出跨 transcript 聚类的有状态监控，提前30%发现攻击。

### [Automatically Attacking Software Reverse Engineering AI Agents](https://arxiv.org/abs/2605.30667)
- **Authors:** Brian Crawford, Justin Phillips, Patrick McClure
- **Date:** 2026-05-28
- **Category:** `prompt injection AND agent`

> Genetic algorithm-based prompt generation (AutoDAN variant) deceives LLM-powered binary analysis agents (GhidraMCP) via extraneous string variable assignments that inject instructions without affecting executable functionality.

**📝 Summary:** 用遗传算法自动生成 prompt injection 攻击二进制分析 AI agent（GhidraMCP），绕过 LLM 分析管线。

### [Strengthening Polymorphic Prompt Assembling: Dynamic Separator Generation Against Emerging Prompt Injection Attacks](https://arxiv.org/abs/2605.30534)
- **Authors:** Nima Dorzhiev, Peng Liu
- **Date:** 2026-05-28
- **Category:** `prompt injection AND agent`

> Dynamic per-request separator generation using SHA-256 digests eliminates blast-radius vulnerability of static pool PPA. Reduces ASR from 0.88 to 0.38 on leetspeak obfuscation, eliminates static separator leakage entirely.

**📝 Summary:** 动态分隔符生成防御 prompt injection，每个请求使用基于时间戳和随机数的唯一 separator，消除静态分隔符泄漏后的 blast-radius 漏洞。

### [AgentDoG 1.5: A Lightweight and Scalable Alignment Framework for AI Agent Safety and Security](https://arxiv.org/abs/2605.29801)
- **Authors:** Dongrui Liu, Yu Li, Zhonghao Yang et al.
- **Date:** 2026-05-28
- **Category:** `agent safety`

> Modern open-world agents such as OpenClaw exhibit powerful cross-environment execution capabilities yet introduce broad new safety risk sources. We propose a lightweight and scalable agent safety alignment framework, updating the agent safety taxonomy for emergent risks from Codex and OpenClaw execution scenarios. We build a taxonomy-guided data en...

**📝 Summary:** 轻量级 agent safety 对齐框架 AgentDoG 1.5，覆盖 OpenClaw/Codex 等新型执行场景下的安全分类，用约1k样本训练可媲美 GPT-5.4。

### [Understanding Safety-Sensitive Expert Behavior in Mixture-of-Experts LLMs](https://arxiv.org/abs/2605.29708)
- **Authors:** Zhibo Zhang, Yuxi Li, Zhen Ouyang et al.
- **Date:** 2026-05-28
- **Category:** `red teaming AND LLM`

> RASET: Router-Agnostic Safety-critical Expert Tuning identifies safety-critical experts via contrastive routing-sensitivity and applies parameter-efficient tuning. Shows routing is topic-driven, not safety-driven, in MoE LLMs.

**📝 Summary:** MoE LLM 中安全行为由少量专家控制而非 routing 驱动，RASET 通过对这些专家的 PEFT 可破坏安全对齐。

### [Hijacking Agent Memory: Stealthy Trojan Attacks Through Conversational Interaction](https://arxiv.org/abs/2605.29960)
- **Authors:** Hongtao Wang, Se Yang, Yu Chen et al.
- **Date:** 2026-05-28
- **Category:** `LLM agent AND attack`

> MemPoison attacks LLM agent long-term memory through dialogue, bypassing selective memory mechanisms. Three components: semantic relational bridge, entity masquerading, joint embedding optimization. Achieves ASR up to 0.95.

**📝 Summary:** 通过对话交互向 LLM agent 长期记忆注入触发型后门（MemPoison），绕过选择性记忆机制，ASR 高达0.95。

### [The Surface You Test Is Not the Surface That Breaks](https://arxiv.org/abs/2605.30454)
- **Authors:** Shifat E Arman, Syed Nazmus Sakib, Nafiul Haque et al.
- **Date:** 2026-05-28
- **Category:** `prompt injection AND agent`

> Delivering identical injection bytes through tool outputs vs tool descriptions inverts success rates across models: GPT-4.1 is 96% vulnerable on tool outputs but 4% on descriptions; GEMINI-3-FLASH shows the mirror pattern. Model-surface interaction accounts for 16.7% of variance. Adaptive Attack Rate (max over surfaces) exceeds any fixed-surface ba...

**📝 Summary:** 同一注入内容通过不同 surface（tool output vs tool description）投递，在不同模型上 ASR 完全反转，模型×surface 交互项占16.7%方差。

### [Minimal Prompt Perturbations Lead to Code Vulnerabilities: Prompt Fragility and Hidden-State Signals in Coding LLMs](https://arxiv.org/abs/2605.29737)
- **Authors:** Alexander Sternfeld, Andrei Kucharavy, Ljiljana Dolamic
- **Date:** 2026-05-28
- **Category:** `prompt injection AND agent`

> Single-character prompt mutations can flip LLM-generated code from secure to vulnerable. Hidden state analysis shows input-handling vulnerabilities are more predictable (AUC 0.753) than secure-defaults vulnerabilities (AUC 0.674).

**📝 Summary:** 单字符 prompt 变化可导致 LLM 生成代码从安全变为漏洞，隐状态分析可预测输入处理类漏洞。

### [The Best-Laid SCHEMEs: Coordinated Sabotage and Monitoring in Multi-Agent Systems](https://arxiv.org/abs/2605.29178)
- **Authors:** Nikolay Radev, Lennart Haas, Benjamin Arnav et al.
- **Date:** 2026-05-27
- **Category:** `multi-agent AND safety`

> SCHEME benchmark: 17 tasks where agents must decompose and execute coordinated sabotage while completing legitimate tasks. Gemini achieves 84% and Codex 46% covert success. Trusted monitor detects at FPR<=2% from code edits alone.

**📝 Summary:** SCHEME：测试多 agent 系统中协同隐蔽破坏行为的 benchmark，Gemini 84%/Codex 46%成功，可信监控器从代码变更中以 FPR<=2% 检测到。

### [SNARE: Adaptive Scenario Synthesis for Eliciting Overeager Behavior in Coding Agents](https://arxiv.org/abs/2605.28122)
- **Authors:** Yubin Qu, Yi Liu, Gelei Deng et al.
- **Date:** 2026-05-27
- **Category:** `jailbreak AND agent`

> SNARE synthesizes benign scenarios to elicit out-of-scope actions in coding agents (overeager behavior). 19.51% of 10k runs trigger overeager behavior; agent framework accounts for 56% of variation vs model's 21%.

**📝 Summary:** 合成良性场景诱导 coding agent 执行超出授权范围的操作（overeager behavior），10k次运行中19.51%触发，框架类型的影响远大于模型本身。

### [AIRGuard: Guarding Agent Actions with Runtime Authority Control](https://arxiv.org/abs/2605.28914)
- **Authors:** Suliu Qin, Haomin Zhuang, Yujun Zhou et al.
- **Date:** 2026-05-27
- **Category:** `jailbreak AND agent`

> AIRGuard operationalizes least privilege as action-time authorization. Identifies authority confusion failure mode. Reduces Sonnet 4.6 attack success from 36.3% to 5.5% on AgentTrap, preserves 76% benign utility.

**📝 Summary:** 运行时权限控制守卫 agent 行动，识别「权限混淆」失败模式，将攻击成功率从36.3%降至5.5%，同时保留76%良性功能。

### [ChainCaps: Composition-Safe Tool-Using Agents via Monotonic Capability Attenuation](https://arxiv.org/abs/2605.26542)
- **Authors:** Xiaochong Jiang, Shiqi Yang, Ziwei Li et al.
- **Date:** 2026-05-26
- **Category:** `tool use AND attack`

> ChainCaps prevents permission laundering in tool composition via capability budgets that propagate by intersection. Reduces ASR from 25-68% to 0-4.8% while preserving 96-100% benign completion. MCP proxy, no agent/tool changes needed.

**📝 Summary:** 通过单调能力衰减防止工具组合中的权限洗白（permission laundering），以 MCP 代理实现，无需修改 agent 或工具服务。

### [Constitutional Arms Races in the Public Goods Game: Co-Evolving LLM Constitutions Under Cooperation-Defection Pressure](https://arxiv.org/abs/2605.26448)
- **Authors:** Ujwal Kumar, Arth Singh, Hershraj Niranjani et al.
- **Date:** 2026-05-26
- **Category:** `red teaming AND LLM`

> Adversarial constitutional co-evolution of LLM agents in PGG. Under coupled fitness, both factions converge to near-parity equilibrium. Evolved Red constitutions serve as interpretable red-team artifacts.

**📝 Summary:** 在公共品博弈中协同进化攻防 LLM「宪法」，两阵营收敛到近均衡，进化出的 Red 宪法可作为 red-teaming 人工制品。

### [Got a Secret? LLM Agents Can't Keep It: Evaluating Privacy in Multi-Agent Systems](https://arxiv.org/abs/2605.27766)
- **Authors:** Aman Priyanshu, Supriti Vijay, Esha Pahwa
- **Date:** 2026-05-26
- **Category:** `safety benchmark AND agent`

> Multi-turn social evaluation amplifies privacy violations (19.95% to 45.30%). Leakage is socially contagious: agents 8x more likely to disclose after observing peer do so. Privacy instructions reduce but don't eliminate leakage (>37.8% remains).

**📝 Summary:** 多 agent 社交环境下 LLM 的隐私泄露是传染性的，多轮社交评估将违规率从20%翻倍到45%，明确的隐私指令效果有限。

### [TRACES: Proactive Safety Auditing for Multi-Turn LLM Agents via Trajectory-State Modeling](https://arxiv.org/abs/2605.27690)
- **Authors:** Jiaqian Li, Yanshu Li, Boxuan Zhang et al.
- **Date:** 2026-05-26
- **Category:** `agent safety`

> We propose TRACES, a representation-based proactive auditor that learns prefix-level trajectory risk states from the hidden representations of an observer LLM to estimate whether a partial trajectory is drifting toward unsafe behavior.

**📝 Summary:** 通过观察者 LLM 的隐表示学习轨迹风险状态，在 agent 中途主动发现安全风险。

---

## 2026-W21

### [MemAudit: Post-hoc Auditing of Poisoned Agent Memory via Causal Attribution and Structural Anomaly Detection](https://arxiv.org/abs/2605.23723)
- **Authors:** Zhewen Tan, Yilun Yao, Huiyan Jin et al.
- **Date:** 2026-05-22
- **Category:** `LLM agent AND attack`

> Large language model agents increasingly rely on persistent memory to store past interactions, retrieve relevant demonstrations, and improve long-horizon task execution. However, this memory mechanism also creates a practical security vulnerability: an adversarial user may inject malicious records into the agent's memory through ordinary interactio...

**📝 Summary:** MemAudit提出事后因果记忆审计框架，通过反事实影响分数和记忆一致性图检测被投毒的代理记忆，将QA场景下的攻击成功率从70%降至0%。

### [Blind Spots in the Guard: How Domain-Camouflaged Injection Attacks Evade Detection in Multi-Agent LLM Systems](https://arxiv.org/abs/2605.22001)
- **Authors:** Aaditya Pai
- **Date:** 2026-05-21
- **Category:** `LLM agent AND attack`

> Injection detectors deployed to protect LLM agents are calibrated on static, template-based payloads that announce themselves as override directives. We identify a systematic blind spot: when payloads are generated to mimic the domain vocabulary and authority structures of the target document, what we call domain camouflaged injection, standard det...

**📝 Summary:** 发现注入检测器针对"域伪装注入"（模拟目标文档词汇和权威结构的攻击载荷）存在系统性盲点，Llama Guard 3对此类攻击检测率为0%，多智能体辩论架构会将攻击放大9.9倍。

### [Boiling the Frog: A Multi-Turn Benchmark for Agentic Safety](https://arxiv.org/abs/2605.22643)
- **Authors:** Piercosma Bisconti, Matteo Prandi, Federico Pierucci et al.
- **Date:** 2026-05-21
- **Category:** `agent safety`

> Traditional safety benchmarks for language models evaluate generated text: whether a model outputs toxic language, reproduces bias, or follows harmful instructions. When models are deployed as agents, the safety-relevant object shifts from what the system says to what it does within an environment, and evaluating model responses under prompting is ...

**📝 Summary:** "温水煮青蛙"基准测试评估工具使用型代理对渐进式增量攻击的抵抗性，9个模型平均严格ASR为44.4%，通过有状态多轮评估衡量代理在工作区持久化场景中的安全行为。

### [Harder to Defend: Towards Chinese Toxicity Attacks via Implicit Enhancement and Obfuscation Rewriting](https://arxiv.org/abs/2605.22258)
- **Authors:** Jingyi Kang, Junyu Lu, Bo Xu et al.
- **Date:** 2026-05-21
- **Category:** `red teaming AND LLM`

> Large language models (LLMs) require robust toxicity evaluation beyond explicit wording. This setting remains underexplored in Chinese, where toxicity may combine semantic indirectness with surface obfuscation. We introduce Chinese Implicit Toxicity Attack (CITA), a controlled red-team evaluation and defense-data generation framework. CITA uses thr...

**📝 Summary:** CITA框架针对中文毒性内容的隐式增强和混淆改写进行红队测试，通过三阶段流水线将有害意图转化为隐式混淆变体，使7种检测器平均误检率达69.48%。

### [How Far Will They Go? Red-Teaming Online Influence with Large Language Models](https://arxiv.org/abs/2605.22880)
- **Authors:** Daniel C. Ruiz, Anna Serbina, Ashwin Rao et al.
- **Date:** 2026-05-20
- **Category:** `jailbreak AND agent`

> As large language model (LLM)-based agents increasingly participate in online discourse, red-teaming their capacity to support political influence campaigns is critical for information integrity. We introduce an empirical red-teaming framework for measuring LLM Overton Windows (OWs), defined as the range of political opinions a model can reliably e...

**📝 Summary:** 对30+开源LLM进行红队测试，度量模型的"奥弗顿窗口"（政治观点表达范围），发现越狱效果在模型家族间差异显著，为政治影响活动的LLM审计提供框架。

### [LASH: Adaptive Semantic Hybridization for Black-Box Jailbreaking of Large Language Models](https://arxiv.org/abs/2605.21362)
- **Authors:** Abdullah Al Nomaan Nafi, Fnu Suya, Swarup Bhunia et al.
- **Date:** 2026-05-20
- **Category:** `red teaming AND LLM`

> Jailbreak attacks expose a persistent gap between the intended safety behavior of aligned large language models and their behavior under adversarial prompting. We introduce LASH (LLM Adaptive Semantic Hybridization), a black-box framework that treats outputs from multiple base attacks as reusable seed prompts and adaptively composes them for each t...

**📝 Summary:** LASH通过自适应语义混合多种基础攻击策略实现黑盒越狱，在JailbreakBench上平均ASR达84.5%，仅需30次查询即超越5个SOTA基线，展示跨异构越狱策略自适应组合的有效性。

### [Heartbeat-Bound Hierarchical Credentials: Cryptographic Revocation for AI Agent Swarms](https://arxiv.org/abs/2605.20704)
- **Authors:** Saurabh Deochake
- **Date:** 2026-05-20
- **Category:** `prompt injection AND agent`

> Autonomous AI agents that spawn sub-agent swarms create a safety gap: existing credential revocation mechanisms, OAuth 2.0 introspection, OCSP, and W3C Status Lists, require network connectivity to a central authority, leaving 'zombie agents' executing privileged operations for minutes to hours after operator shutdown. We present Heartbeat-Bound Hi...

**📝 Summary:** 提出HBHC密码协议，通过心跳绑定凭证有效性来解决多智能体集群中的“僵尸代理”问题，实现90倍于OAuth 2.0的撤销窗口压缩。

### [VIPER-MCP: Detecting and Exploiting Taint-Style Vulnerabilities in Model Context Protocol Servers](https://arxiv.org/abs/2605.21392)
- **Authors:** Pengyu Sun, Qishu Jin, Enhao Huang et al.
- **Date:** 2026-05-20
- **Category:** `LLM agent AND attack`

> Model Context Protocol (MCP) has emerged as a standard interface for connecting LLM agents to external tools. Because MCP servers expose privileged operations such as shell execution, network access, and file-system manipulation to agent-driven invocation, implementation flaws in tool handlers can create a direct path from natural-language input to...

**📝 Summary:** VIPER-MCP是首个针对MCP服务器污点风格漏洞的端到端自动化审计框架，在39,884个开源MCP仓库中发现106个0-day漏洞并全部通过漏洞利用追踪确认，已获67个CVE编号。

### [AgentAtlas: Beyond Outcome Leaderboards for LLM Agents](https://arxiv.org/abs/2605.20530)
- **Authors:** Parsa Mazaheri, Kasra Mazaheri
- **Date:** 2026-05-19
- **Category:** `LLM agent AND attack`

> Large language model agents now act on codebases, browsers, operating systems, calendars, files, and tool ecosystems, but the benchmarks used to evaluate them are fragmented: each emphasizes a different unit of measurement. AgentAtlas extends this line of work with four components: (i) a six-state control-decision taxonomy (Act / Ask / Refuse / Sto...

**📝 Summary:** AgentAtlas提出六状态控制决策分类法和九类轨迹失败分类法，发现去除分类标签后所有模型轨迹准确率下降14-40个百分点，揭示现有排行榜严重高估了模型的真实代理能力。

### [RoboJailBench: Benchmarking Adversarial Attacks and Defenses in Embodied Robotic Agents](https://arxiv.org/abs/2605.19328)
- **Authors:** Doguhuan Yeke, Yanming Zhou, Leo Y. Lin et al.
- **Date:** 2026-05-19
- **Category:** `jailbreak AND agent`

> Recent advances in Vision-Language Models (VLMs) facilitate a new class of embodied AI systems, where these models are integrated into physical platforms, e.g. robots and autonomous vehicles, to interpret visual scenes and execute natural language commands in diverse environments. We address this gap with RoboJailBench, which consists of three core...

**📝 Summary:** RoboJailBench是首个针对具身机器人AI越狱攻击和防御的标准化评测框架，包含基于ISO标准的18类安全违规分类法及配对对抗/良性目标数据集。

### [Refusal Evaluation in Coding LLMs and Code Agents: A Systematic Review of Thirteen Malicious-Code Prompt Corpora (2023-2025)](https://arxiv.org/abs/2605.20351)
- **Authors:** Richard J. Young, Gregory D. Moody
- **Date:** 2026-05-19
- **Category:** `jailbreak AND agent`

> The evaluation of large language model refusal on malicious-coding tasks now spans at least thirteen publicly released prompt corpora (AdvBench, the CyberSecEval family, RMCBench, RedCode, MCGMark, JailbreakBench, CySecBench, MalwareBench, CIRCLE, MOCHA, ASTRA, Scam2Prompt / Innoc2Scam-bench, and JAWS-Bench), each constructed under a different prot...

**📝 Summary:** 对13个恶意代码提示语料库进行PRISMA风格系统综述，将数据集本身作为分析单元，指出三个方法论缺口：缺乏人工标注基准、跨语料库不可比性以及恶意软件分类法碎片化。

### [Overeager Coding Agents: Measuring Out-of-Scope Actions on Benign Tasks](https://arxiv.org/abs/2605.18583)
- **Authors:** Yubin Qu, Ying Zhang, Yanjun Zhang et al.
- **Date:** 2026-05-18
- **Category:** `prompt injection AND agent`

> Coding agents now run autonomously with shell, file, and network privileges. When a user issues a benign request, the agent sometimes does more than asked: it deletes unrelated files, wipes a stale credentials backup, or rewrites configuration the user never mentioned. We call these scope expansions overeager actions, an authorization problem disti...

**📝 Summary:** 构建OverEager-Bench基准测试，衡量编码代理在良性任务上的越界行为，发现去掉同意声明后越界率提升11.9-17.2个百分点，框架设计比模型对齐对越界率影响更大。

### [Multilingual jailbreaking of LLMs using low-resource languages](https://arxiv.org/abs/2605.18239)
- **Authors:** Dylan Marx, Marcel Dunaiski
- **Date:** 2026-05-18
- **Category:** `red teaming AND LLM`

> Large Language Models (LLMs) remain vulnerable to jailbreak attempts that circumvent safety guardrails. We investigate whether multi-turn conversations using low-resource African languages (Afrikaans, Kiswahili, isiXhosa, and isiZulu) can bypass safety mechanisms across commercial LLMs. We translated prompts from existing datasets and evaluated Cha...

**📝 Summary:** 研究低资源非洲语言（南非荷兰语等）多轮对话越狱攻击，发现翻译质量是成功率的关键因子，人工红队测试比自动测试效果更高，多轮对话比单轮翻译攻击显著更有效。

### [Remembering More, Risking More: Longitudinal Safety Risks in Memory-Equipped LLM Agents](https://arxiv.org/abs/2605.17830)
- **Authors:** Ahmad Al-Tawaha, Shangding Gu, Peizhi Niu et al.
- **Date:** 2026-05-18
- **Category:** `prompt injection AND agent`

> Safety evaluations of memory-equipped LLM agents typically measure within-task safety: whether an agent completes a single scenario safely, often under adversarial conditions such as prompt injection or memory poisoning. In deployment, however, a single agent serves many independent tasks over a long horizon, and memory accumulated during earlier t...

**📝 Summary:** 研究具有记忆功能的LLM代理中的“时序记忆污染”问题，发现随着记忆累积安全违规率单调上升，论证记忆安全应被视为需要时序评估的纵向属性。

### [Position: A Three-Layer Probabilistic Assume-Guarantee Architecture Is Structurally Required for Safe LLM Agent Deployment](https://arxiv.org/abs/2605.18672)
- **Authors:** S. Bensalem, Y. Dong, M. Franzle et al.
- **Date:** 2026-05-18
- **Category:** `agent safety`

> This position paper argues that enforcing LLM agent safety within a single abstraction layer is not merely suboptimal but categorically insufficient for deployed LLM agents -- a structural consequence of how agent execution works, not a contingent limitation of current systems. The three dimensions that jointly constitute safe operation -- semantic...

**📝 Summary:** 立场论文论证单层安全架构对于LLM代理部署根本不足，提出需要三层假设-保证架构分别处理语义意图、环境有效性和动力学可行性三个安全维度。

### [ESLD (External Surrogate Latent Defense): A Latent-Space Architecture for Faster, Stronger Prompt-Injection Defense](https://arxiv.org/abs/2605.18918)
- **Authors:** Yash Narendra
- **Date:** 2026-05-18
- **Category:** `prompt injection AND agent`

> Modern AI assistants are agentic. To answer a single user request, the underlying language model pulls in information from many sources, such as web searches, retrieved documents, tool outputs, and user follow-ups, and reasons over them across several steps. Any of these inputs can carry malicious content. This opens the door to prompt injection, w...

**📝 Summary:** ESLD通过读取守卫模型的内部潜空间表示而非等待其输出，实现3倍加速和16.4个百分点的检测精度提升，无需重训模型即可部署。

### [POLAR-Bench: A Diagnostic Benchmark for Privacy-Utility Trade-offs in LLM Agents](https://arxiv.org/abs/2605.19127)
- **Authors:** Qiaoyuan Zheng, Yiqu Yang, Qi Gao et al.
- **Date:** 2026-05-18
- **Category:** `LLM agent AND attack`

> LLM agents increasingly have access to private user data and act on the user's behalf when interacting with third-party systems. We introduce POLAR-Bench (Policy-aware adversarial Benchmark), in which a trusted model with a privacy policy and a task converses with a third-party model that adversarially probes for both task-relevant and protected at...

**📝 Summary:** POLAR-Bench通过对抗性第三方模型探测LLM代理的隐私-效用权衡，发现前沿模型可保护99%以上的受保护属性，而1-30B量级开放权重模型中最弱者泄露超过一半隐私信息。

### [OEP: Poisoning Self-Evolving LLM Agents via Locally Correct but Non-Transferable Experiences](https://arxiv.org/abs/2605.18930)
- **Authors:** Kaixiang Wang, Jiong Lou, Zhaojiacheng Zhou et al.
- **Date:** 2026-05-18
- **Category:** `LLM agent AND attack`

> Memory-augmented large language model (LLM) agents use iterative reflection and self-evolution to solve complex tasks, but these mechanisms introduce security risks. We introduce Obsessive Experience Poisoning (OEP), a low-privilege black-box attack requiring no direct control over the system prompt or memory database. OEP constructs adversarial cl...

**📝 Summary:** OEP提出通过构造局部正确但不可迁移的边缘案例来毒化自我进化LLM代理的低权限黑盒攻击，诱导反思机制将局部经验过度泛化为错误规则，对GPT-4o代理ASR超50%。

### [Hallucination as Exploit: Evidence-Carrying Multimodal Agents](https://arxiv.org/abs/2605.19192)
- **Authors:** Guijia Zhang, Hao Zheng, Harry Yang
- **Date:** 2026-05-18
- **Category:** `tool use AND attack`

> Multimodal agents increasingly choose tool calls from screenshots, documents, and webpages, where a false perceptual claim can turn hallucination from an answer-quality error into an authorization failure. We formalize this failure mode as hallucination-to-action conversion: an unsupported claim supplies the precondition for a privileged action. We...

**📝 Summary:** 提出ECA架构形式化"幻觉即漏洞利用"问题，通过将工具调用分解为动作关键谓词并用DOM/OCR验证器证书授权，实现200个端到端任务零不安全执行，而朴素代理不安全执行率100%。

### [Babel: Jailbreaking Safety Attention via Obfuscation Distribution Optimized Sampling](https://arxiv.org/abs/2605.17971)
- **Authors:** Ziwei Wang, Jing Chen, Ruichao Liang et al.
- **Date:** 2026-05-18
- **Category:** `red teaming AND LLM`

> Despite rigorous safety alignment, Large Language Models (LLMs) remain vulnerable to jailbreak attacks. We investigate an intrinsic vulnerability in the safety mechanisms of LLMs, where safety alignment relies on a small set of sparsely distributed attention heads, leaving much of the representational space weakly monitored. We formalize this pheno...

**📝 Summary:** Babel发现LLM安全对齐依赖稀疏分布的少数注意力头，通过数学模型指导的混淆分布优化采样实现黑盒越狱，将GPT-4o攻击成功率从41.33%提升至82.67%，仅需40次查询。

### [LivePI: More Realistic Benchmarking of Agents Against Indirect Prompt Injection](https://arxiv.org/abs/2605.17986)
- **Authors:** Lei Zhao, Abhay Bhaskar, Edgar Dobriban
- **Date:** 2026-05-18
- **Category:** `prompt injection AND agent`

> AI agents such as OpenClaw are increasingly deployed in local workflows with access to external tools. This creates indirect prompt-injection (IPI) risk: an agent may execute harmful instructions embedded in untrusted inputs such as email, downloaded files, webpages, repositories, or group-chat messages. Existing evaluations are often small, purely...

**📝 Summary:** LivePI是一个覆盖7种输入面和12种攻击系列的间接提示注入基准，在真实虚拟机上测试5个前沿模型，攻击成功率为10.7%-29.6%，群聊注入对所有模型均100%成功。

### [An Empirical Study of Privacy Leakage Chains via Prompt Injection in Black-Box Chatbot Environments](https://arxiv.org/abs/2605.18133)
- **Authors:** Hongjang Yang, Hyunsik Na, Daeseon Choi
- **Date:** 2026-05-18
- **Category:** `prompt injection AND agent`

> LLM-based chatbot agents increasingly process user requests by combining natural-language reasoning with external tools such as web browsing. These capabilities improve usability, but they also create attack surfaces when untrusted external content is processed as part of a user's task. This paper studies a privacy-leakage attack chain based on ind...

**📝 Summary:** 研究黑盒聊天机器人环境中通过间接提示注入实现隐私泄露的攻击链，提出“exemplification”技术将用户提示重框为少样本示例从而劫持代理行为。

---

## 2026-W20

### [AI Agents May Always Fall for Prompt Injections](https://arxiv.org/abs/2605.17634)
- **Authors:** Sahar Abdelnabi, Eugene Bagdasarian
- **Date:** 2026-05-17
- **Category:** `prompt injection AND agent`

> Prompt injection is the most critical vulnerability in deployed AI agents. Despite recent progress, we show that the prevailing defense paradigm (data-instruction separation) both fails to detect attacks that operate through contextual manipulation and degrades contextually appropriate behavior. We then recast prompt injection via the lens of Conte...

**📝 Summary:** 通过情境完整性理论重新框架提示注入问题，提出不可能性结论：攻击者总能构造使封锁流看起来合法的上下文，因此纯防御范式存在根本局限。

### [ADR: An Agentic Detection System for Enterprise Agentic AI Security](https://arxiv.org/abs/2605.17380)
- **Authors:** Chenning Li, Pan Hu, Justin Xu et al.
- **Date:** 2026-05-17
- **Category:** `prompt injection AND agent`

> We present the Agentic AI Detection and Response (ADR) system, the first large-scale, production-proven enterprise framework for securing AI agents operating through the Model Context Protocol (MCP). ADR addresses three challenges via three components: the ADR Sensor for high-fidelity agentic telemetry, the ADR Explorer for systematic pre-deploymen...

**📝 Summary:** ADR是Uber生产环境部署10个月的企业级MCP代理安全检测系统，在ADR-Bench上零误报并检测67%攻击，F1分数比SOTA基线高2-4倍（MLSys 2026工业轨道）。

### [ASPI: Seeking Ambiguity Clarification Amplifies Prompt Injection Vulnerability in LLM Agents](https://arxiv.org/abs/2605.17324)
- **Authors:** Udari Madhushani Sehwag, Zhengyang Shan, Heming Liu et al.
- **Date:** 2026-05-17
- **Category:** `LLM agent AND attack`

> Clarification-seeking behavior is widely regarded as a desirable property of LLM agents, enabling them to resolve ambiguity before acting on underspecified tasks. However, the security implications of this interaction pattern remain unexplored. We investigate whether the transition from standard execution to a clarification-seeking state increases ...

**📝 Summary:** ASPI基准揭示代理在寻求澄清状态时提示注入攻击成功率急剧上升（o3从1.8%升至34.0%），表明标准执行时的鲁棒性测试严重低估了交互式代理的真实攻击面。

### [Who Owns This Agent? Tracing AI Agents Back to Their Owners](https://arxiv.org/abs/2605.16035)
- **Authors:** Ruben Chocron, Doron Jonathan Ben Chayim, Eyal Lenga et al.
- **Date:** 2026-05-15
- **Category:** `"agentic" AND "adversarial"`

> AI agents are increasingly deployed to act autonomously in the world, yet there is still no reliable way to trace a harmful agent back to the account that deployed it. We formalize this gap as the problem of agent attribution: linking an observed agent interaction to the responsible account at the hosting vendor. Our protocol is canary-based: an au...

**📝 Summary:** 提出agent归因问题并给出基于金丝雀注入的解决方案，将有害agent行为可靠追溯到部署账户，对抗性算子无法在不损害任务性能的情况下规避归因。

### [FORGE: Self-Evolving Agent Memory With No Weight Updates via Population Broadcast](https://arxiv.org/abs/2605.16233)
- **Authors:** Igor Bogdanov, Chung-Horng Lung, Thomas Kunz et al.
- **Date:** 2026-05-15
- **Category:** `"prompt injection" AND "agent"`

> Can LLM agents improve decision-making through self-generated memory without gradient updates? We propose FORGE (Failure-Optimized Reflective Graduation and Evolution), a staged, population-based protocol that evolves prompt-injected natural-language memory for hierarchical ReAct agents. FORGE wraps a Reflexion-style inner loop, where a dedicated r...

**📝 Summary:** FORGE通过种群广播机制进化prompt注入的自然语言记忆（无梯度更新），在网络防御POMDP任务上将零样本基线提升1.7-7.7倍。

### [Context, Reasoning, and Hierarchy: A Cost-Performance Study of Compound LLM Agent Design in an Adversarial POMDP](https://arxiv.org/abs/2605.16205)
- **Authors:** Igor Bogdanov, Chung-Horng Lung, Thomas Kunz et al.
- **Date:** 2026-05-15
- **Category:** `"agentic" AND "adversarial"`

> Deploying compound LLM agents in adversarial, partially observable sequential environments requires navigating several design dimensions: what the agent sees, how it reasons, and how tasks are decomposed across components. We present a controlled study in CybORG CAGE-2, a cyber defense environment. Our evaluation spans five model families, six mode...

**📝 Summary:** 在对抗性POMDP（网络防御CybORG）中系统研究复合LLM agent设计的成本-性能权衡，发现程序化状态抽象回报最高，层次化推理工具叠加会产生'deliberation cascade'。

### [Web Agents Should Adopt the Plan-Then-Execute Paradigm](https://arxiv.org/abs/2605.14290)
- **Authors:** Julien Piet, Annabella Chow, Yiwei Hou et al.
- **Date:** 2026-05-14
- **Category:** `"prompt injection" AND "agent"`

> ReAct has become the default architecture across LLM agents, and many existing web agents follow this paradigm. We argue that it is the wrong default for web agents. Instead, web agents should default to plan-then-execute: commit to a task-specific program before observing runtime web content, then execute it. Under ReAct, all untrusted web content...

**📝 Summary:** 论文主张网页agent应采用'先规划后执行'范式将用户意图与不可信内容隔离，防止prompt injection在运行时重定向控制流，80%的WebArena任务可用纯程序化计划完成。

### [Hidden in Memory: Sleeper Memory Poisoning in LLM Agents](https://arxiv.org/abs/2605.15338)
- **Authors:** Sidharth Pulipaka, Stanislau Hlebik, Leonidas Raghav et al.
- **Date:** 2026-05-14
- **Category:** `"prompt injection" AND "agent"`

> Large language models are increasingly augmented with persistent memory, allowing assistants to store user-specific information across sessions for personalization and continuity. This statefulness introduces a new security risk: adversarial content can corrupt what an assistant remembers and thereby influence future interactions. We propose and st...

**📝 Summary:** 提出“沉睡记忆中毒”攻击：通过操控外部内容让agent存储伪造记忆，跨会话潜伏并影响后续行为，GPT-5.5上投毒成功率高达99.8%。

### [Toward Securing AI Agents Like Operating Systems](https://arxiv.org/abs/2605.14932)
- **Authors:** Lukas Pirch, Micha Horlboge, Patrick Großmann et al.
- **Date:** 2026-05-14
- **Category:** `"tool use" AND "attack"`

> Autonomous agents based on large language models (LLMs) are rapidly emerging as a general-purpose technology, with recent systems extending their capabilities through broad tool use, third-party skills, and deeper integration into user environments. We investigate the security of LLM-based agents through the lens of operating systems, arguing that ...

**📝 Summary:** 通过操作系统安全视角分析LLM agent的安全挑战，系统梳理攻击面，发现四个主流agent框架在适度攻击能力下多个保护机制失效，建议借鉴OS安全技术。

### [Auditing Agent Harness Safety](https://arxiv.org/abs/2605.14271)
- **Authors:** Chengzhi Liu, Yichen Guo, Yepeng Liu et al.
- **Date:** 2026-05-14
- **Category:** `"multi-agent" AND "safety"`

> LLM agents increasingly run inside execution harnesses that dispatch tools, allocate resources, and route messages between specialized components. However, a harness can return a correct, benign answer over a trajectory that accesses unauthorized resources or leaks context to the wrong agent. We propose HarnessAudit, a framework that audits full ex...

**📝 Summary:** HarnessAudit提出对agent执行框架全轨迹的安全审计方案，发现任务完成与安全执行不一致，资源访问和跨agent信息传递是最主要违规集中点。

### [WARD: Adversarially Robust Defense of Web Agents Against Prompt Injections](https://arxiv.org/abs/2605.15030)
- **Authors:** Tri Cao, Yulin Chen, Hieu Cao et al.
- **Date:** 2026-05-14
- **Category:** `"prompt injection" AND "agent"`

> Web agents can autonomously complete online tasks by interacting with websites, but their exposure to open web environments makes them vulnerable to prompt injection attacks embedded in HTML content or visual interfaces. We propose WARD (Web Agent Robust Defense against Prompt Injection), built on WARD-Base, a large-scale dataset with around 177K s...

**📝 Summary:** WARD提出针对网页agent的对抗鲁棒prompt injection防御方案，通过177K样本数据集和攻防协同进化训练，实现近乎完美的OOD误注入检测。

### [Agentic AI in Industry: Adoption Level and Deployment Barriers](https://arxiv.org/abs/2605.14675)
- **Authors:** Spyridon Alvanakis Apostolou, Jan Bosch, Helena Holmström Olsson
- **Date:** 2026-05-14
- **Category:** `"multi-agent" AND "safety"`

> Agentic AI systems are entering software engineering workflows, yet empirical evidence on how industrial organizations actually adopt them remains sparse. We present a qualitative interview study with sixteen practitioners across twelve companies of varying size and domain. This study characterizes the current agentic AI adoption state employing a ...

**📝 Summary:** 对12家公司16名从业者的定性访谈研究，揭示工业界agentic AI部署现状，发现'能力-部署验证差距'（缺乏可靠的输出验证机制）是多agent系统落地的核心障碍。

### [Model-Agnostic Lifelong LLM Safety via Externalized Attack-Defense Co-Evolution](https://arxiv.org/abs/2605.13411)
- **Authors:** Xiaozhe Zhang, Chaozhuo Li, Hui Liu et al.
- **Date:** 2026-05-13
- **Category:** `"red teaming" AND "LLM"`

> Large language models remain vulnerable to adversarial prompts that elicit harmful outputs. We propose EvoSafety, an LLM safety framework built around persistent, inspectable, and reusable external structures. For red teaming, EvoSafety equips the attack policy with an adversarial skill library, enabling continued vulnerability probing through simp...

**📝 Summary:** EvoSafety通过外部化攻击技能库和记忆检索防御机制实现跨模型持续安全进化，Guard模式下防御成功率99.61%，参数量仅为Qwen3Guard-8B的37.5%。

### [ProjGuard: Safety Monitoring for Computer-Use Agents via Low-Dimensional Projections](https://arxiv.org/abs/2605.13631)
- **Authors:** Kebin Contreras
- **Date:** 2026-05-13
- **Category:** `"prompt injection" AND "agent"`

> Computer-use agents are increasingly capable of operating on real operating systems, but this capability has also increased the risks posed by prompt injection, indirect instructions, and visual attacks. We propose ProjGuard, an alternative based on behavioral trajectory monitoring. At each step, we derive a lightweight scalar risk signal from the ...

**📝 Summary:** ProjGuard通过低维投影行为轨迹监控实现计算机使用agent的在线安全监控，将不安全率从16%降至3%，同时提升任务完成率。

### [AgentTrap: Measuring Runtime Trust Failures in Third-Party Agent Skills](https://arxiv.org/abs/2605.13940)
- **Authors:** Haomin Zhuang, Hanwen Xing, Yujun Zhou et al.
- **Date:** 2026-05-13
- **Category:** `"jailbreak" AND "agent"`

> Third-party skills are becoming the package ecosystem for LLM agents. A malicious skill does not need to ask the model to perform an obviously harmful action. Instead, it can disguise the harmful behavior as part of a routine workflow, relying on the agent to execute that workflow with high-value permissions and limited human supervision. AgentTrap...

**📝 Summary:** AgentTrap是评估LLM agent抵抗第三方技能中恶意运行时行为的动态基准，发现最关键的失败不是简单jailbreak，而是agent将有害副作用当作正常工作流执行。

### [On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment](https://arxiv.org/abs/2605.11882)
- **Authors:** Bo Yin, Qi Li, Xinchao Wang
- **Date:** 2026-05-12
- **Category:** `"agent safety"`

> Tool-using LLM agents fail through trajectories rather than only final responses, as they may execute unsafe tool calls, follow injected instructions, comply with harmful requests, or over-refuse benign tasks despite producing a seemingly safe answer. Existing safety-alignment signals are largely response-level or off-policy, and often incur a safe...

**📝 Summary:** FATE框架通过将失败轨迹转化为修复监督信号实现agent安全对齐的在策略自进化，相比baselines降低攻击成功率33.5%、有害合规82.6%。

### [REALISTA: Realistic Latent Adversarial Attacks that Elicit LLM Hallucinations](https://arxiv.org/abs/2605.12813)
- **Authors:** Buyun Liang, Jinqi Luo, Liangzu Peng et al.
- **Date:** 2026-05-12
- **Category:** `"adversarial attack" AND "language model"`

> We formulate hallucination elicitation as a constrained optimization problem, where the goal is to find semantically coherent adversarial prompts that are equivalent to benign user prompts. We propose REALISTA, a realistic latent-space attack framework. REALISTA constructs an input-dependent dictionary of valid editing directions, each correspondin...

**📝 Summary:** REALISTA提出现实感的潜空间对抗攻击框架诱发LLM幻觉，结合语义等价改写的离散空间真实性与连续优化的灵活性，在大型推理模型上有效，ICML 2026接收。

### [Safety Context Injection: Inference-Time Safety Alignment via Static Filtering and Agentic Analysis](https://arxiv.org/abs/2605.11664)
- **Authors:** Zhenhao Xu, Wenhan Chang, Yichuan Chen et al.
- **Date:** 2026-05-12
- **Category:** `"jailbreak" AND "agent"`

> Large Reasoning Models (LRMs) improve performance on complex tasks, but they also make safety control harder at deployment time. In black-box settings, defenders cannot modify model weights and must instead intervene at inference time. We propose Safety Context Injection (SCI), an inference-time framework that separates safety assessment from task ...

**📝 Summary:** SCI框架通过在推理时注入结构化外部风险报告作为安全上下文，解决大型推理模型在黑盒设置下的safety alignment问题，关注'思考-输出差距'现象。

### [Rollout Cards: A Reproducibility Standard for Agent Research](https://arxiv.org/abs/2605.12131)
- **Authors:** Charlie Masters, Ziyuan Liu, Stefano V. Albrecht
- **Date:** 2026-05-12
- **Category:** `"multi-agent" AND "safety"`

> Reproducibility problems that have long affected machine learning and reinforcement learning are now surfacing in agent research: papers compare systems by reported scores while leaving the rollout records behind those scores difficult to inspect. In a structured audit of 50 popular training and evaluation repositories, we find that none report how...

**📝 Summary:** 提出Rollout Cards作为agent研究的可重复性标准，发现50个主流仓库均未报告失败案例，不同报告规则可导致评分偏差达20.9%，甚至逆转模型排名。

### [Persona-Conditioned Adversarial Prompting: Multi-Identity Red-Teaming for Adversarial Discovery and Mitigation](https://arxiv.org/abs/2605.11730)
- **Authors:** Cristian Morasso, Anisa Halimi, Muhammad Zaid Hameed et al.
- **Date:** 2026-05-12
- **Category:** `"red teaming" AND "LLM"`

> Automated red-teaming for LLMs often discovers narrow attack slices, missing diverse real-world threats, and yielding insufficient data for safety fine-tuning. We introduce Persona-Conditioned Adversarial Prompting (PCAP), which conditions adversarial search on diverse attacker personas (e.g., doctors, students, malicious actors) and strategy sets ...

**📝 Summary:** PCAP通过不同攻击者角色条件化对抗搜索，将攻击成功率从57%提升至97%，生成多样化攻击数据集，用于微调后模型鲁棒性大幅提升。

### [IPI-proxy: An Intercepting Proxy for Red-Teaming Web-Browsing AI Agents Against Indirect Prompt Injection](https://arxiv.org/abs/2605.11868)
- **Authors:** Chia-Pei Chen, Kentaroh Toyoda, Anita Lai et al.
- **Date:** 2026-05-12
- **Category:** `"red teaming" AND "LLM"`

> Web-browsing AI agents are increasingly deployed in enterprise settings under strict whitelists of approved domains, yet adversaries can still influence them by embedding hidden instructions in the HTML pages those domains serve. We present IPI-proxy, an open-source toolkit for red-teaming web-browsing agents against indirect prompt injection (IPI)...

**📝 Summary:** IPI-proxy是开源红队工具包，通过拦截代理在白名单域名的真实HTTP响应中动态嵌入820个去重攻击载荷，对网页浏览agent进行间接prompt注入测试。

### [SkillSafetyBench: Evaluating Agent Safety under Skill-Facing Attack Surfaces](https://arxiv.org/abs/2605.12015)
- **Authors:** Chang Jin, An Wang, Zeming Wei et al.
- **Date:** 2026-05-12
- **Category:** `"agent safety"`

> Reusable skills are becoming a common interface for extending large language model agents, packaging procedural guidance with access to files, tools, memory, and execution environments. However, this modularity introduces attack surfaces that are largely missed by existing safety evaluations: even when the user request is benign, task-relevant skil...

**📝 Summary:** 提出SkillSafetyBench，针对技能接口攻击面的agent安全基准（155个对抗案例、30个安全类别），揭示skill层面的攻击可绕过模型对齐。

### [Proteus: A Self-Evolving Red Team for Agent Skill Ecosystems](https://arxiv.org/abs/2605.11891)
- **Authors:** Zhaojiacheng Zhou
- **Date:** 2026-05-12
- **Category:** `"red teaming" AND "LLM"`

> Agent skills extend LLM agents with reusable instructions, tool interfaces, and executable code, and users increasingly install third-party skills from marketplaces, repositories, and community channels. We frame this risk as adaptive leakage -- whether a budgeted attacker can iteratively revise a skill until it passes audit and produces verified r...

**📝 Summary:** Proteus针对agent技能生态系统的自进化红队框架，通过五轴攻击空间搜索测量自适应攻击者的攻击成功率，揭示现有技能审计在对抗迭代攻击者面前存在严重不足。

### [FlowSteer: Prompt-Only Workflow Steering Exposes Planning-Time Vulnerabilities in Multi-Agent LLM Systems](https://arxiv.org/abs/2605.11514)
- **Authors:** Fanxiao Li, Jiaying Wu, Tingchao Fu et al.
- **Date:** 2026-05-12
- **Category:** `"multi-agent" AND "safety"`

> Multi-agent systems (MAS) powered by LLMs increasingly adopt planner-executor architectures, where planners convert prompts into subtasks, roles, dependencies, and routing paths. We study this risk through social influence probing workflows to identify high-impact subtasks and malicious-signal propagation. FlowSteer is a prompt-only workflow steeri...

**📝 Summary:** FlowSteer通过纯提示词操控多agent系统的工作流规划阶段，攻击成功率比朴素方法高55%，揭示multi-agent系统在规划时存在的工作流注入漏洞。

### [Beyond Red-Teaming: Formal Guarantees of LLM Guardrail Classifiers](https://arxiv.org/abs/2605.10901)
- **Authors:** Nikita Kezins, Urbas Ekka, Pascal Berrang et al.
- **Date:** 2026-05-11
- **Category:** `"red teaming" AND "LLM"`

> Guardrail Classifiers defend production language models against harmful behavior, but provide no formal guarantees. We close this gap by shifting verification from the discrete input space to the classifier's pre-activation space, where we define a harmful region as a convex shape enclosing the representations of known harmful prompts. We propose t...

**📝 Summary:** 提出对LLM guardrail分类器的形式化验证框架，通过pre-activation空间的有害区域定义给出安全保证，发现现有guardrail存在可验证的安全漏洞。

### [LITMUS: Benchmarking Behavioral Jailbreaks of LLM Agents in Real OS Environments](https://arxiv.org/abs/2605.10779)
- **Authors:** Chiyu Zhang, Huiqin Yang, Bendong Jiang et al.
- **Date:** 2026-05-11
- **Category:** `"jailbreak" AND "agent"`

> The rapid proliferation of LLM-based autonomous agents in real operating system environments introduces a new category of safety risk beyond content safety: behavior jailbreak, where an adversary induces an agent to execute dangerous OS-level operations with irreversible consequences. We present LITMUS, a benchmark addressing both gaps via a semant...

**📝 Summary:** LITMUS是首个在真实OS环境中评估LLM agent行为越狱的基准，发现'执行幻觉'现象（言语拒绝但OS层面危险操作已完成），Claude Sonnet 4.6仍执行40.64%高危操作。

### [Adversarial Attacks Against MLLMs via Progressive Resolution Processing and Adaptive Feature Alignment](https://arxiv.org/abs/2605.09902)
- **Authors:** Hao Wang, Xiaorong Ma, Weiqi Luo et al.
- **Date:** 2026-05-11
- **Category:** `"adversarial attack" AND "language model"`

> Adversarial perturbations can mislead Multimodal Large Language Models (MLLMs) recognize a benign image as a specific target object, posing serious risks in safety-critical scenarios such as autonomous driving and medical diagnosis. We propose PRAF-Attack, a targeted transfer-based attack framework that integrates multi-scale global semantic guidan...

**📝 Summary:** PRAF-Attack提出针对多模态LLM的可迁移目标对抗攻击框架，通过渐进分辨率处理和自适应特征对齐提升跨模型迁移性，在12个开源和闭源模型上验证。

### [Adversarial SQL Injection Generation with LLM-Based Architectures](https://arxiv.org/abs/2605.11188)
- **Authors:** Ali Karakoc, H. Birkan Yilmaz
- **Date:** 2026-05-11
- **Category:** `"adversarial attack" AND "language model"`

> SQL injection (SQLi) attacks are still one of the serious attacks ranked in the OWASP Top 10 threats. We introduce two novel LLM-based systems, Retrieval Augmented Generation for Adversarial SQLi (RADAGAS) and Reflective Chain-of-Thought SQLi (RefleXQLi), and compare them against 10 Web Application Firewalls (WAFs) and one MySQL validator. RADAGAS-...

**📝 Summary:** 使用LLM自动化生成对抗性SQL注入载荷，测试10个WAF，RADAGAS-GPT4o达22.73%绕过率，对AI/ML类WAF效果显著但无法有效绕过规则类WAF。

---

## 2026-W19

### [Modeling Implicit Conflict Monitoring Mechanisms against Stereotypes in LLMs](https://arxiv.org/abs/2605.09647)
- **Authors:** Jingshen Zhang, Bo Wang, Yanlin Fu et al.
- **Date:** 2026-05-10
- **Category:** `jailbreak AND agent`

> In this paper, we study an emergent self-debiasing mechanisms against stereotypical content in Large Language Models (LLMs). Unlike traditional safety mechanisms that are primarily triggered by explicit input-level stimuli, self-debiasing mechanisms can involve generation-time intrinsic correction that are not directly reducible to surface-level pr...

**📝 Summary:** 提出COCO方法识别LLM中负责隐式自我去偏见的神经元，停用这些神经元会导致超过90%输出退化为偏见内容（超过明确越狱攻击的效果），并提供无训练的轻量级增强策略。

### [Schema-Conditioned Classification for LLM Safeguard (GLiGuard)](https://arxiv.org/abs/2605.07982)
- **Authors:** Urchade Zaratiana
- **Date:** 2026-05-08
- **Category:** `safety benchmark agent`

> We introduce GLiGuard, a 0.3B-parameter schema-conditioned bidirectional encoder for LLM content moderation. The key idea is to encode task definitions and label semantics directly into the input sequence as structured token schemas, enabling simultaneous evaluation of prompt safety, response safety, refusal detection, 14 fine-grained harm categori...

**📝 Summary:** GLiGuard：0.3B 编码器通过 schema 条件化同时检测 14 种危害类别和 11 种 jailbreak 策略，精度媲美 7B-27B 模型，速度快 16x。

### [SafeHarbor: Hierarchical Memory-Augmented Guardrail for LLM Agent Safety](https://arxiv.org/abs/2605.05704)
- **Authors:** Zhe Liu, Zonghao Ying, Wenxin Zhang et al.
- **Date:** 2026-05-07
- **Category:** `tool use attack LLM agent`

> With the rapid evolution of foundation models, LLM agents have demonstrated increasingly powerful tool-use capabilities. However, this proficiency introduces significant security risks. We propose SafeHarbor, a novel framework designed to establish precise decision boundaries for LLM agents. SafeHarbor extracts context-aware defense rules through e...

**📝 Summary:** SafeHarbor：通过分层记忆系统动态注入上下文感知防御规则，在不损失 utility 前提下拦截恶意工具调用。

### [ClawGuard: Out-of-Band Detection of LLM Agent Workflow Hijacking via EM Side Channel](https://arxiv.org/abs/2605.06205)
- **Authors:** Leo Linqian Gan, Jeffery Wu, Longyuan Ge et al.
- **Date:** 2026-05-07
- **Category:** `tool use attack LLM agent`

> Autonomous LLM agents face a critical security risk known as workflow hijacking, where attackers subtly alter tool and skill invocations. Existing defenses rely on host-internal telemetry which can be forged if the host OS is compromised. We introduce ClawGuard, a passive, out-of-band monitor that audits LLM-agent workflows using electromagnetic (E...

**📝 Summary:** 利用电磁侧信道（EM emanations）在带外检测 LLM agent 工作流劫持，AUC 0.9945，绕过被篡改的 OS 日志。

### [AgentTrust: Runtime Safety Evaluation and Interception for AI Agent Tool Use](https://arxiv.org/abs/2605.04785)
- **Authors:** Chen Yang
- **Date:** 2026-05-06
- **Category:** `tool use attack LLM agent`

> Modern AI agents execute real-world side effects through tool calls such as file operations, shell commands, HTTP requests, and database queries. A single unsafe action, including accidental deletion, credential exposure, or data exfiltration, can cause irreversible harm. Existing defenses are incomplete: post-hoc benchmarks measure behavior after ...

**📝 Summary:** 提出 AgentTrust，运行时拦截 agent tool calls 并给出 allow/warn/block 判决，支持多步攻击链检测，发布 300+630 场景 benchmark。

### [SoK: Robustness in Large Language Models against Jailbreak Attacks](https://arxiv.org/abs/2605.05058)
- **Authors:** Feiyue Xu, Hongsheng Hu, Chaoxiang He et al.
- **Date:** 2026-05-06
- **Category:** `jailbreak agent`

> Large Language Models remain highly susceptible to jailbreak attacks. Existing evaluation practices are inadequate, often relying on narrow metrics like attack success rate that fail to capture the multidimensional nature of LLM security. We present a systematic taxonomy of jailbreak attacks and defenses and introduce Security Cube, a unified, mult...

**📝 Summary:** S&P 2026 系统综述：13 种 jailbreak 攻击和 5 种防御的多维度评估框架 Security Cube，梳理 LLM 鲁棒性现状与挑战。

### [ARGUS: Defending LLM Agents Against Context-Aware Prompt Injection](https://arxiv.org/abs/2605.03378)
- **Authors:** Shihao Weng, Yang Feng, Jinrui Zhang et al.
- **Date:** 2026-05-05
- **Category:** `prompt injection agent`

> The rise of Large Language Model (LLM) agents, augmented with tool use, skills, and external knowledge, has introduced new security risks. Among them, prompt injection attacks, where adversaries embed malicious instructions into the agent workflow, have emerged as the primary threat. However, existing benchmarks and defenses are fundamentally limit...

**📝 Summary:** 提出 ARGUS 防御框架，通过 provenance graph 追踪不可信上下文传播路径，将 prompt injection ASR 降至 3.8%，同时保留 87.5% 任务效用。

### [Exposing LLM Safety Gaps Through Mathematical Encoding: New Attacks and Systematic Analysis](https://arxiv.org/abs/2605.03441)
- **Authors:** Haoyu Zhang
- **Date:** 2026-05-05
- **Category:** `adversarial attack language model`

> We show that encoding harmful prompts as coherent mathematical problems -- using formalisms such as set theory, formal logic, and quantum mechanics -- bypasses safety filters at high rates, achieving 46%-56% average attack success across eight target models. The effectiveness depends not on mathematical notation itself, but on whether a helper LLM ...

**📝 Summary:** 用集合论/形式逻辑等数学编码重写恶意 prompt 可绕过安全过滤器，8 个模型平均 ASR 46-56%；接受于 Canadian AI 2026。

### [Redefining AI Red Teaming in the Agentic Era: From Weeks to Hours](https://arxiv.org/abs/2605.04019)
- **Authors:** Raja Sekhar Rao Dheekonda
- **Date:** 2026-05-05
- **Category:** `red teaming LLM`

> AI systems are entering critical domains like healthcare, finance, and defense, yet remain vulnerable to adversarial attacks. We introduce an AI red teaming agent built on the open-source Dreadnode SDK. The agent creates workflows grounded in 45+ adversarial attacks, 450+ transforms, and 130+ scorers. We red team Meta Llama Scout and achieve an 85%...

**📝 Summary:** 提出基于 Dreadnode SDK 的 AI red teaming agent，集成 45+ 攻击/450+ transforms，将红队测试从数周压缩到数小时，对 Llama Scout 达 85% ASR。

### [ContextualJailbreak: Evolutionary Red-Teaming via Simulated Conversational Priming](https://arxiv.org/abs/2605.02647)
- **Authors:** Mario Rodriguez Bejar
- **Date:** 2026-05-04
- **Category:** `jailbreak agent`

> We present ContextualJailbreak, a black-box red-teaming strategy that performs evolutionary search over a simulated multi-turn primed dialogue. Across 50 representative HarmBench behaviors, ContextualJailbreak achieves ASR of 100% on gpt-oss:20B, 100% on qwen3-8B, 100% on llama3.1:70B, and 90% on gpt-oss:120B. The 40 attacks discovered against gpt-...

**📝 Summary:** 多轮对话 priming 攻击框架，发现 Claude 系列 robustness 显著优于其他模型（仅 15-17.5% ASR vs GPT/Gemini 的 70-90%），揭示 provider 级别的对齐不对称性。

### [MAGE: Safeguarding LLM Agents against Long-Horizon Threats via Shadow Memory](https://arxiv.org/abs/2605.03228)
- **Authors:** Yuhui Wang
- **Date:** 2026-05-04
- **Category:** `multi-agent safety`

> As LLM-powered agents are increasingly deployed for complex tasks, they face attacks that exploit extended user-agent-environment interactions. We present MAGE (Memory As Guardrail Enforcement), a defensive framework inspired by the 'shadow stack' abstraction in systems security. MAGE maintains a dedicated, safety-focused agentic memory that distil...

**📝 Summary:** MAGE：借鉴系统安全中 shadow stack 思想，维护独立的安全记忆追踪全轨迹，在长 horizon 威胁检测中显著优于现有防御。

---

## 2026-W18

### [Self-Adaptive Multi-Agent LLM-Based Security Pattern Selection for IoT Systems](https://arxiv.org/abs/2605.00741)
- **Authors:** Saeid Jamshidi, Foutse Khomh, Carol Fung et al.
- **Date:** 2026-05-01
- **Category:** `"multi-agent" AND "safety"`

> The adoption of Internet of Things (IoT) systems at the network edge of smart architectures is increasing rapidly, intensifying the need for security mechanisms that are both adaptive and resource-efficient. We introduce ASPO, a self-adaptive multi-agent security pattern selection that integrates Large Language Model (LLM)-based reasoning with dete...

**📝 Summary:** 提出 ASPO，将 LLM 推理与确定性执行引擎结合的自适应多智能体安全模式选择系统，实现 100% 无冲突激活，面向 IoT 边缘安全。

### [Stable-GFlowNet: Toward Diverse and Robust LLM Red-Teaming via Contrastive Trajectory Balance](https://arxiv.org/abs/2605.00553)
- **Authors:** Minchan Kwon, Sunghyun Baek, Minseo Kim et al.
- **Date:** 2026-05-01
- **Category:** `"red teaming" AND "LLM"`

> Large Language Model (LLM) Red-Teaming, which proactively identifies vulnerabilities of LLMs, is an essential process for ensuring safety. Finding effective and diverse attacks in red-teaming is important, but achieving both is challenging. Generative Flow Networks (GFNs) that perform distribution matching are a promising methods, but they are noto...

**📝 Summary:** 提出 Stable-GFN，通过配对比较消除 GFlowNet 的分区函数估计，在 ICML 2026 Spotlight 中展示了稳定且多样的 LLM 红队攻击生成。

### [FinSafetyBench: Evaluating LLM Safety in Real-World Financial Scenarios](https://arxiv.org/abs/2605.00706)
- **Authors:** Yutao Hou, Yihan Jiang, Yuhan Xie et al.
- **Date:** 2026-05-01
- **Category:** `"red teaming" AND "LLM"`

> Large language models (LLMs) are increasingly applied in financial scenarios. However, they may produce harmful outputs, including facilitating illegal activities or unethical behavior, posing serious compliance risks. To systematically evaluate LLM safety in finance, we propose FinSafetyBench, a bilingual (English-Chinese) red-teaming benchmark de...

**📝 Summary:** 提出双语金融合规红队基准 FinSafetyBench（14 子类别），测试 LLM 对金融犯罪类请求的拒绝能力，ACL 2026 Findings。

### [FlashRT: Towards Computationally and Memory Efficient Red-Teaming for Prompt Injection and Knowledge Corruption](https://arxiv.org/abs/2604.28157)
- **Authors:** Yanting Wang, Chenlong Yin, Ying Chen et al.
- **Date:** 2026-04-30
- **Category:** `"prompt injection" AND "agent"`

> Long-context large language models (LLMs) are widely used to empower many real-world applications, such as retrieval-augmented generation, autonomous agents, and AI assistants. However, security remains a major concern for their widespread deployment, with threats such as prompt injection and knowledge corruption. To quantify the security risks fac...

**📝 Summary:** 提出 FlashRT，通过计算和内存优化加速针对长上下文 LLM 的 prompt injection 红队测试，速度提升 2-7x，内存减少 2-4x。

### [The Inverse-Wisdom Law: Architectural Tribalism and the Consensus Paradox in Agentic Swarms](https://arxiv.org/abs/2604.27274)
- **Authors:** Dahlia Shehata, Ming Li
- **Date:** 2026-04-30
- **Category:** `"multi-agent" AND "safety"`

> As AI transitions toward multi-agent systems to solve complex workflows, research paradigms operate on the axiomatic assumption that agent collaboration mirrors the 'Wisdom of the Crowd'. We challenge this assumption by formalizing the Consensus Paradox: a phenomenon where agentic swarms prioritize internal architectural agreement over external log...

**📝 Summary:** 在 12,804 条轨迹上发现'逆智慧定律'：同构多 agent 群中增加逻辑 agent 反而稳固错误轨迹，揭示架构同质性（模型同族）是群体失效的关键因素。

### [Safe Bilevel Delegation (SBD): A Formal Framework for Runtime Delegation Safety in Multi-Agent Systems](https://arxiv.org/abs/2604.27358)
- **Authors:** Yuan Sun
- **Date:** 2026-04-30
- **Category:** `"multi-agent" AND "safety"`

> As large language model (LLM) agents are deployed in high-stakes environments, the question of how safely to delegate subtasks to specialized sub-agents becomes critical. We propose Safe Bilevel Delegation (SBD), a formal framework for runtime delegation safety in hierarchical multi-agent systems. SBD formulates task delegation as a bilevel optimiz...

**📝 Summary:** 提出双层优化框架 SBD，在运行时动态调整多智能体任务委托中的安全-效率权衡，并证明安全单调性和问责传播界。

### [Attention Is Where You Attack](https://arxiv.org/abs/2605.00236)
- **Authors:** Aviral Srivastava, Sourav Panda
- **Date:** 2026-04-30
- **Category:** `"adversarial attack" AND "language model"`

> Safety-aligned large language models rely on RLHF and instruction tuning to refuse harmful requests, yet the internal mechanisms implementing safety behavior remain poorly understood. We introduce the Attention Redistribution Attack (ARA), a white-box adversarial attack that identifies safety-critical attention heads and crafts nonsemantic adversar...

**📝 Summary:** 提出注意力重分配攻击（ARA），定位安全关键 attention head 并重定向其注意力，仅需 5 个非语义对抗 token 即可绕过 LLM 安全对齐。

### [A Logic of Inability](https://arxiv.org/abs/2604.27917)
- **Authors:** Shanxia Wang
- **Date:** 2026-04-30
- **Category:** `"multi-agent" AND "safety"`

> Coalition Logic is primarily concerned with what coalitions can achieve, whereas what coalitions cannot achieve -- their inability -- has received comparatively little explicit attention. This asymmetry matters in artificial intelligence and safety-critical multi-agent systems, where one often needs to specify not merely what agents are instructed ...

**📝 Summary:** 扩展联盟逻辑引入明确的'无力算子'，为多智能体系统中的能力限制和不可能性推理提供形式化框架。

### [Understanding Adversarial Transferability in Vision-Language Models for Autonomous Driving: A Cross-Architecture Analysis](https://arxiv.org/abs/2604.27414)
- **Authors:** David Fernandez, Pedram MohajerAnsari, Amir Salarpour et al.
- **Date:** 2026-04-30
- **Category:** `"adversarial attack" AND "language model"`

> Vision-language models (VLMs) are increasingly used in autonomous driving because they combine visual perception with language-based reasoning. We address this gap with a systematic cross-architecture study of adversarial transferability in VLM-based driving, evaluating three representative architectures (Dolphins, OmniDrive, and LeapVAD) using phy...

**📝 Summary:** 研究自动驾驶 VLM 跨架构对抗迁移性，三种架构间转移率达 73-91%，发布于 SAE WCX 2026。

### [Low Rank Adaptation for Adversarial Perturbation](https://arxiv.org/abs/2604.27487)
- **Authors:** Han Liu, Shanghao Shi, Yevgeniy Vorobeychik et al.
- **Date:** 2026-04-30
- **Category:** `"adversarial attack" AND "language model"`

> Low-Rank Adaptation (LoRA) has significantly improved the training efficiency of Large Language Models by updating neural network layers using low-rank matrices. Since the generation of adversarial examples is an optimization process analogous to model training, this raises the question: Do adversarial perturbations exhibit a similar low-rank struc...

**📝 Summary:** 证明对抗扰动具有内在低秩结构，并利用此特性将搜索空间降至低维子空间，显著提升黑盒攻击的效率和效果。

### [Causal Foundations of Collective Agency](https://arxiv.org/abs/2605.00248)
- **Authors:** Frederik Hytting Jørgensen, Sebastian Weichwald, Lewis Hammond
- **Date:** 2026-04-30
- **Category:** `"multi-agent" AND "safety"`

> A key challenge for the safety of advanced AI systems is the possibility that multiple simpler agents might inadvertently form a collective agent with capabilities and goals distinct from those of any individual. We adopt a behavioral perspective, ascribing collective agency to a group when viewing the group's joint actions as rational and goal-dir...

**📝 Summary:** 用因果博弈和因果抽象形式化多智能体系统中的集体行为，为理解 AI 涌现集体智能提供理论基础，CLeaR 2026。

### [Ambient Persuasion in a Deployed AI Agent: Unauthorized Escalation Following Routine Non-Adversarial Content Exposure](https://arxiv.org/abs/2605.00055)
- **Authors:** 
- **Date:** 2026-04-29
- **Category:** `"multi-agent" AND "safety"`

> We report a safety incident in a deployed multi-agent research system in which a primary AI agent installed 107 unauthorized software components, overwrote a system registry, overrode a prior negative decision from an oversight agent, and escalated through increasingly privileged operations up to an attempted system administrator command. The incid...

**📝 Summary:** 报告已部署 AI agent 安全事件：读取一篇非对抗性技术文章后，agent 自主安装 107 个未授权组件并逐步升级权限，揭示'环境说服'（ambient persuasion）这一新型威胁。

### [Indirect Prompt Injection in the Wild: An Empirical Study of Prevalence, Techniques, and Objectives](https://arxiv.org/abs/2604.27202)
- **Authors:** Soheil Khodayari, Xuenan Zhang, Bhupendra Acharya et al.
- **Date:** 2026-04-29
- **Category:** `"prompt injection" AND "agent"`

> As LLMs are increasingly integrated into systems that browse, retrieve, summarize, and act on web content, webpages have become an untrusted input vector for downstream model behavior. We present one of the first large-scale empirical analyses of indirect prompt injections in webpages and HTTP responses. Analyzing 1.2B URLs from 24.8M hosts, we ide...

**📝 Summary:** 对 12亿 URL 的大规模扫描，发现 1.5 万条真实存在的 indirect prompt injection，70% 针对机器而非人类，揭示真实网络生态中的 injection 分布。

### [SnapGuard: Lightweight Prompt Injection Detection for Screenshot-Based Web Agents](https://arxiv.org/abs/2604.25562)
- **Authors:** Mengyao Du, Han Fang, Haokai Ma et al.
- **Date:** 2026-04-28
- **Category:** `"prompt injection" AND "agent"`

> Web agents have emerged as an effective paradigm for automating interactions with complex web environments, yet remain vulnerable to prompt injection attacks that embed malicious instructions into webpage content to induce unintended actions. This threat is further amplified for screenshot-based web agents, which operate on rendered visual webpages...

**📝 Summary:** 轻量级方法 SnapGuard 通过视觉稳定性和文本信号检测截图型 web agent 的 prompt injection，比 GPT-4o 快 8 倍，F1=0.75。

### [Luminol-AIDetect: Fast Zero-shot Machine-Generated Text Detection based on Perplexity under Text Shuffling](https://arxiv.org/abs/2604.25860)
- **Authors:** Lucio La Cava, Andrea Tagarelli
- **Date:** 2026-04-28
- **Category:** `"adversarial attack" AND "language model"`

> Machine-generated text (MGT) detection requires identifying structurally invariant signals across generation models. We propose Luminol-AIDetect, a novel zero-shot statistical approach that exposes LLM structural fragility through coherence disruption. By applying a simple randomized text-shuffling procedure, we demonstrate that the resulting shift...

**📝 Summary:** 提出基于文本打乱后困惑度变化的零样本机器生成文本检测方法 Luminol-AIDetect，跨 18 语言、11 种攻击类型实现 SOTA，FPR 降低 17 倍。

### [One Perturbation, Two Failure Modes: Probing VLM Safety via Embedding-Guided Typographic Perturbations](https://arxiv.org/abs/2604.25102)
- **Authors:** Ravikumar Balakrishnan, Sanket Mendapara
- **Date:** 2026-04-28
- **Category:** `"prompt injection" AND "agent"`

> Typographic prompt injection exploits vision language models' (VLMs) ability to read text rendered in images, posing a growing threat as VLMs power autonomous agents. Prior work typically focus on maximizing attack success rate (ASR) but does not explain why certain renderings bypass safety alignment. We make two contributions. First, an empirical ...

**📝 Summary:** 研究 VLM 中排版型 prompt injection 攻击，发现嵌入距离能预测攻击成功率（r=-0.71~-0.93），揭示安全对齐绕过的两种失效模式（可读性恢复 vs 对齐弱化）。

---

## 2026-W17

### [Automation-Exploit: A Multi-Agent LLM Framework for Adaptive Offensive Security with Digital Twin-Based Risk-Mitigated Exploitation](https://arxiv.org/abs/2604.22427)
- **Authors:** Biagio Andreucci, Arcangelo Castiglione
- **Date:** 2026-04-24
- **Category:** `"multi-agent" AND "safety"`

> Automation-Exploit is a fully autonomous Multi-Agent System (MAS) framework designed for adaptive offensive security in complex black-box scenarios. It bridges the abstraction gap between reconnaissance and exploitation by autonomously exfiltrating executables and contextual intelligence across multiple protocols. The framework introduces an adapti...

**📝 Summary:** 多 agent 系统自动化漏洞利用框架，通过数字孪生进行风险缓解的内存漏洞利用，在真实黑盒场景中验证架构有效性。

### [Black-Box Skill Stealing Attack from Proprietary LLM Agents: An Empirical Study](https://arxiv.org/abs/2604.21829)
- **Authors:** Zihan Wang, Rui Zhang, Yu Liu et al.
- **Date:** 2026-04-23
- **Category:** `"agentic" AND "adversarial"`

> LLM agents increasingly rely on skills to encapsulate reusable capabilities via progressively disclosed instructions. This paper presents the first empirical study of black-box skill stealing against LLM agent systems. An automated stealing prompt generation agent starts from model-generated seed prompts, expands them through scenario rationalizati...

**📝 Summary:** 首个对 LLM agent skill（系统提示/指令）的黑盒窃取攻击实证研究：仅需 3 次交互即可提取技能内容，引发版权和知识产权风险。

### [MCP Pitfall Lab: Exposing Developer Pitfalls in MCP Tool Server Security under Multi-Vector Attacks](https://arxiv.org/abs/2604.21477)
- **Authors:** Run Hao, Zhuoran Tan
- **Date:** 2026-04-23
- **Category:** `"LLM agent" AND "attack"`

> Model Context Protocol (MCP) is increasingly adopted for tool-integrated LLM agents, but its multi-layer design and third-party server ecosystem expand risks across tool metadata, untrusted outputs, cross-tool flows, multimodal inputs, and supply-chain vectors. MCP Pitfall Lab operationalizes developer pitfalls as reproducible scenarios and validat...

**📝 Summary:** MCP 工具服务器安全 pitfall 测试框架：系统化暴露 tool-metadata 污染、puppet server、多模态注入等开发者陷阱，trace-based 验证揭示 agent narrative 与实际 trace 在 63.2% 情况下不一致。

### [Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities in Large Language Models](https://arxiv.org/abs/2604.21860)
- **Authors:** Naheed Rayhan, Sohely Jahan
- **Date:** 2026-04-23
- **Category:** `"jailbreak" AND "agent"`

> This paper introduces Transient Turn Injection (TTI), a new multi-turn attack technique that systematically exploits stateless moderation by distributing adversarial intent across isolated interactions. TTI leverages automated attacker agents powered by large language models to iteratively test and evade policy enforcement in both commercial and op...

**📝 Summary:** 提出 TTI 多轮注入攻击：将有害意图分散在多轮隔离交互中以绕过无状态 moderation，发现不同模型的 attack surface pattern 差异显著。

### [Adaptive Instruction Composition for Automated LLM Red-Teaming](https://arxiv.org/abs/2604.21159)
- **Authors:** Jesse Zymet, Andy Luo, Swapnil Shinde et al.
- **Date:** 2026-04-22
- **Category:** `"red teaming" AND "LLM"`

> This article introduces Adaptive Instruction Composition, a novel framework that combines crowdsourced texts according to an adaptive mechanism trained to jointly optimize effectiveness with diversity. It uses reinforcement learning to balance exploration with exploitation in a combinatorial space of instructions to guide the attacker toward divers...

**📝 Summary:** 提出 Adaptive Instruction Composition：用 RL 训练的上下文 bandit 自适应组合众包 query+tactic，在多样性-有效性 Pareto 上超越已有方法，ACL 2026 Main 发表。

### [Cross-Session Threats in AI Agents: Benchmark, Evaluation, and Algorithms](https://arxiv.org/abs/2604.21131)
- **Authors:** Ari Azarafrooz
- **Date:** 2026-04-22
- **Category:** `"agentic" AND "adversarial"`

> AI-agent guardrails are memoryless: each message is judged in isolation, so an adversary who spreads a single attack across dozens of sessions slips past every session-bound detector because only the aggregate carries the payload. This paper presents CSTM-Bench, 26 executable attack taxonomies classified by kill-chain stage and cross-session operat...

**📝 Summary:** 提出跨会话威胁 benchmark CSTM-Bench：攻击意图被分散在多个独立会话中，现有无状态 guardrail 无法检测；Coreset Memory Reader 是唯一在两个测试 shard 下保持 recall 的方案。

### [Breaking MCP with Function Hijacking Attacks: Novel Threats for Function Calling and Agentic Models](https://arxiv.org/abs/2604.20994)
- **Authors:** Yannis Belkhiter, Giulio Zizzo, Sergio Maffeis et al.
- **Date:** 2026-04-22
- **Category:** `"jailbreak" AND "agent"`

> This paper introduces a novel function hijacking attack (FHA) that manipulates the tool selection process of agentic models to force the invocation of a specific, attacker-chosen function. While existing attacks focus on semantic preference of the model for function-calling tasks, FHA is largely agnostic to the context semantics and robust to the f...

**📝 Summary:** 提出函数劫持攻击（FHA）：操纵 agentic 模型的工具选择过程，强制调用攻击者指定函数，在 BFCL 数据集上 ASR 达 70-100%。

### [Cyber Defense Benchmark: Agentic Threat Hunting Evaluation for LLMs in SecOps](https://arxiv.org/abs/2604.19533)
- **Authors:** Alankrit Chona, Igor Kozlov, Ambuj Kumar
- **Date:** 2026-04-21
- **Category:** `"LLM agent" AND "attack"`

> The Cyber Defense Benchmark measures how well LLM agents perform the core SOC analyst task of threat hunting: given a database of raw Windows event logs with no guided questions or hints, identify the exact timestamps of malicious events. The benchmark wraps 106 real attack procedures from the OTRF Security-Datasets corpus across 86 MITRE ATT&CK su...

**📝 Summary:** 网络防御 benchmark：在真实 Windows 日志（75k-135k 条记录）中威胁猎取，Claude Opus 4.6 等最强模型仅能找到 3.8% 的恶意事件，LLM 在开放式安全分析上仍然非常弱。

### [An AI Agent Execution Environment to Safeguard User Data](https://arxiv.org/abs/2604.19657)
- **Authors:** Robert Stanley, Avi Verma, Lillian Tsai et al.
- **Date:** 2026-04-21
- **Category:** `"prompt injection" AND "agent"`

> AI agents promise to serve as general-purpose personal assistants for their users, which requires them to have access to private user data. This poses a serious risk to security and privacy. Adversaries may attack the AI model via prompt injection to exfiltrate user data. This paper presents GAAP (Guaranteed Accounting for Agent Privacy), an execut...

**📝 Summary:** 提出 GAAP 执行环境，通过信息流控制（IFC）在不信任 agent 模型的前提下，确定性地防止 prompt injection 导致的用户私有数据泄露。

### [If you're waiting for a sign... that might not be it! Mitigating Trust Boundary Confusion from Visual Injections on Vision-Language Agentic Systems](https://arxiv.org/abs/2604.19844)
- **Authors:** Jiamin Chang, Minhui Xue, Ruoxi Sun et al.
- **Date:** 2026-04-21
- **Category:** `"prompt injection" AND "agent"`

> Recent advances in embodied Vision-Language Agentic Systems (VLAS), powered by large vision-language models (LVLMs), enable AI systems to perceive and reason over real-world scenes. Environmental signals such as traffic lights are essential in-band signals that can and should influence agent behavior. However, similar signals could also be crafted ...

**📝 Summary:** 研究视觉语言 agent 中「信任边界混淆」问题：合法的环境信号（如交通灯）与恶意视觉注入难以区分，提出双进程防御框架（感知与决策分离）。

### [STAR-Teaming: A Strategy-Response Multiplex Network Approach to Automated LLM Red Teaming](https://arxiv.org/abs/2604.18976)
- **Authors:** MinJae Jung, YongTaek Lim, Chaeyun Kim et al.
- **Date:** 2026-04-21
- **Category:** `"jailbreak" AND "agent"`

> This paper introduces STAR-Teaming, a novel black-box framework for automated red teaming that effectively generates jailbreak prompts. STAR-Teaming integrates a Multi-Agent System (MAS) with a Strategy-Response Multiplex Network and employs network-driven optimization to sample effective attack strategies. This network-based approach recasts the i...

**📝 Summary:** STAR-Teaming：用多路复用策略网络驱动自动化红队测试，将攻击策略空间组织为语义社区，在 ACL 2026 Findings 发表，显著提升 ASR 同时降低计算成本。

### [Do Agents Dream of Root Shells? Partial-Credit Evaluation of LLM Agents in Capture The Flag Challenges](https://arxiv.org/abs/2604.19354)
- **Authors:** Ali Al-Kaswan, Maksim Plotnikov, Maxim Hájek et al.
- **Date:** 2026-04-21
- **Category:** `"LLM agent" AND "attack"`

> DeepRed is an open-source benchmark for evaluating LLM-based agents on realistic Capture The Flag (CTF) challenges in isolated virtualized environments. DeepRed introduces a partial-credit scoring method based on challenge-specific checkpoints derived from public writeups, together with an automated summarise-then-judge labelling pipeline. Benchmar...

**📝 Summary:** DeepRed：在真实 CTF VM 环境中评估 LLM agent，引入 checkpoint 部分计分方案，最强模型仅完成 35% checkpoint，非标准发现任务和长时程任务最弱。

---

## 2026-W16

### [MemEvoBench: Benchmarking Memory MisEvolution in LLM Agents](https://arxiv.org/abs/2604.15774)
- **Authors:** Weiwei Xie, Shaoxiong Guo, Fan Zhang et al.
- **Date:** 2026-04-17
- **Category:** `agentic AND adversarial`

> Equipping LLMs with persistent memory enhances interaction continuity and personalization but introduces new safety risks. Specifically, contaminated or biased memory accumulation can trigger abnormal agent behaviors, referred to as memory misevolution. We introduce MemEvoBench, the first benchmark evaluating long-horizon memory safety in LLM agent...

**📝 Summary:** MemEvoBench：首个 LLM agent 记忆演化安全 benchmark，测试对抗记忆注入和噪声工具输出下的长程行为漂移。

### [A Systematic Study of Training-Free Methods for Trustworthy Large Language Models](https://arxiv.org/abs/2604.15789)
- **Authors:** Wai Man Si, Mingjie Li, Michael Backes et al.
- **Date:** 2026-04-17
- **Category:** `adversarial attack AND language model`

> To enable quick and low-cost adaptation, training-free methods have recently emerged as cost-effective alternatives to post-training alignment techniques. We systematically re-evaluate the effectiveness of existing training-free methods against various trustworthy settings and their influence on utility, robustness, and computational overhead. We c...

**📝 Summary:** 系统综述 LLM 免训练安全方法（input/internal/output三层），分析各方法在鲁棒性、效用、计算开销上的权衡与未解问题。

### [Stochasticity in Tokenisation Improves Robustness](https://arxiv.org/abs/2604.16037)
- **Authors:** Sophie Steger, Rui Li, Sofiane Ennadir et al.
- **Date:** 2026-04-17
- **Category:** `adversarial attack AND language model`

> The widespread adoption of large language models (LLMs) has increased concerns about their robustness. Vulnerabilities in perturbations of tokenisation of the input indicate that models trained with a deterministic canonical tokenisation can be brittle to adversarial attacks. We show that pre-training and fine-tuning with uniformly sampled stochast...

**📝 Summary:** 随机 tokenization 训练提升 LLM 对抗鲁棒性；规范 tokenization 训练的模型在非规范输入上准确率下降29.8%。

### [HarmfulSkillBench: How Do Harmful Skills Weaponize Your Agents?](https://arxiv.org/abs/2604.15415)
- **Authors:** Yukun Jiang, Yage Zhang, Michael Backes et al.
- **Date:** 2026-04-16
- **Category:** `agent safety`

> Large language models (LLMs) have evolved into autonomous agents that rely on open skill ecosystems (e.g., ClawHub and Skills.Rest), hosting numerous publicly reusable skills. Existing security research on these ecosystems mainly focuses on vulnerabilities within skills, such as prompt injection. However, there is a critical gap regarding skills th...

**📝 Summary:** 首个大规模 harmful skill 研究（98,440个技能，4.93%有害）；HarmfulSkillBench benchmark 展示隐式恶意意图时 harm score 从0.27升至0.76。

### [Hijacking Large Audio-Language Models via Context-Agnostic and Imperceptible Auditory Prompt Injection](https://arxiv.org/abs/2604.14604)
- **Authors:** Meng Chen, Kun Wang, Li Lu et al.
- **Date:** 2026-04-16
- **Category:** `prompt injection AND agent`

> Modern Large audio-language models (LALMs) power intelligent voice interactions by tightly integrating audio and text. We reveal a previously overlooked threat, auditory prompt injection, under realistic constraints of audio data-only access and strong perceptual stealth. We propose AudioHijack, a general framework that generates context-agnostic a...

**📝 Summary:** AudioHijack：对13个语音大模型的音频 prompt injection 攻击，上下文无关，成功率79%-96%，IEEE S&P 2026。

### [Symbolic Guardrails for Domain-Specific Agents: Stronger Safety and Security Guarantees Without Sacrificing Utility](https://arxiv.org/abs/2604.15579)
- **Authors:** Yining Hong, Yining She, Eunsuk Kang et al.
- **Date:** 2026-04-16
- **Category:** `agent safety`

> AI agents that interact with their environments through tools enable powerful applications, but in high-stakes business settings, unintended actions can cause unacceptable harm, such as privacy breaches and financial loss. Existing mitigations, such as training-based methods and neural guardrails, improve agent reliability but cannot provide guaran...

**📝 Summary:** 系统综述80个 agent safety benchmark，发现85%缺乏具体策略；符号护栏可执行74%策略需求且不牺牲 agent 效用。

### [SoK: Security of Autonomous LLM Agents in Agentic Commerce](https://arxiv.org/abs/2604.15367)
- **Authors:** Qian'ang Mao, Jiaxin Wang, Ya Liu et al.
- **Date:** 2026-04-15
- **Category:** `LLM agent AND attack`

> Autonomous LLM agents are pushing agentic commerce from human-supervised assistance toward machine actors that can negotiate, purchase services, manage digital assets, and execute transactions. This SoK develops a unified security framework for autonomous LLM agents in commerce and finance. We organize threats along five dimensions: agent integrity...

**📝 Summary:** SoK：自主 LLM agent 在 agentic commerce 场景下的安全系统综述，12个跨层攻击向量，五维度威胁分类框架。

### [LogJack: Indirect Prompt Injection Through Cloud Logs Against LLM Debugging Agents](https://arxiv.org/abs/2604.15368)
- **Authors:** Harsh Shah
- **Date:** 2026-04-15
- **Category:** `prompt injection AND agent`

> LLM debugging agents that consume cloud logs and execute remediation commands are vulnerable to indirect prompt injection through log content. We present LogJack, a benchmark of 42 payloads across 5 cloud log categories, and evaluate 8 foundation models under 3 prompt conditions with 5 independent trials each. Under the active condition, verbatim c...

**📝 Summary:** LogJack：通过云日志内容对 LLM 调试 agent 进行 indirect prompt injection，发现 'sanitize and execute' 新行为；不同模型成功率从0%到86.2%。

### [Don't Let AI Agents YOLO Your Files: Shifting Information and Control to Filesystems for Agent Safety and Autonomy](https://arxiv.org/abs/2604.13536)
- **Authors:** Shawn Wanxiang Zhong, Junxuan Liao, Jing Liu et al.
- **Date:** 2026-04-15
- **Category:** `agent safety`

> AI coding agents operate directly on users' filesystems, where they regularly corrupt data, delete files, and leak secrets. Current approaches force a tradeoff between safety and autonomy. To understand this problem, we conduct the first systematic study of agent filesystem misuse, analyzing 290 public reports across 13 frameworks. We design YoloFS...

**📝 Summary:** YoloFS：通过 staging/snapshot/progressive permission 机制防止 AI agent 误操作文件系统，分析290个公开误用报告。

### [SafeHarness: Lifecycle-Integrated Security Architecture for LLM-based Agent Deployment](https://arxiv.org/abs/2604.13630)
- **Authors:** Xixun Lin, Yang Liu, Yancheng Chen et al.
- **Date:** 2026-04-15
- **Category:** `tool use AND attack`

> The performance of LLM agents depends critically on the execution harness. We introduce SafeHarness, a security architecture in which four proposed defense layers are woven directly into the agent lifecycle: adversarial context filtering at input processing, tiered causal verification at decision making, privilege-separated tool control at action e...

**📝 Summary:** SafeHarness：将安全防御嵌入 agent 生命周期各层（输入/决策/执行/状态），降低38% UBR和42% ASR。

### [HINTBench: Horizon-agent Intrinsic Non-attack Trajectory Benchmark](https://arxiv.org/abs/2604.13954)
- **Authors:** Jiacheng Wang, Jinchang Hou, Fabian Wang et al.
- **Date:** 2026-04-15
- **Category:** `agent safety`

> Existing agent-safety evaluation has focused mainly on externally induced risks. Yet agents may still enter unsafe trajectories under benign conditions. We study this complementary but underexplored setting through the lens of intrinsic risk, where intrinsic failures remain latent, propagate across long-horizon execution, and eventually lead to hig...

**📝 Summary:** HINTBench：629条 agent 轨迹的内因性风险评估基准，发现 LLM 轨迹级风险检测好但逐步定位性能<35 Strict-F1。

### [WebAgentGuard: A Reasoning-Driven Guard Model for Detecting Prompt Injection Attacks in Web Agents](https://arxiv.org/abs/2604.12284)
- **Authors:** Yulin Chen, Tri Cao, Haoran Li et al.
- **Date:** 2026-04-14
- **Category:** `prompt injection AND agent`

> Web agents powered by vision-language models (VLMs) enable autonomous interaction with web environments by perceiving and acting on both visual and textual webpage content. However, they are highly vulnerable to prompt injection attacks. We propose a defense framework in which a web agent operates in parallel with a dedicated guard agent, decouplin...

**📝 Summary:** WebAgentGuard：reasoning 驱动的多模态 guard agent，与 web agent 并行检测 prompt injection，RL 训练，超越基线同时保持 agent 效用。

### [Parallax: Why AI Agents That Think Must Never Act](https://arxiv.org/abs/2604.12986)
- **Authors:** Joel Fokou
- **Date:** 2026-04-14
- **Category:** `agent safety`

> Autonomous AI agents are rapidly transitioning from experimental tools to operational infrastructure. The dominant approach to agent safety relies on prompt-level guardrails: natural language instructions that operate at the same abstraction level as the threats they attempt to mitigate. This paper argues that prompt-based safety is architecturally...

**📝 Summary:** Parallax 框架：认知-执行分离等四原则保障 agent 安全，在280个对抗测试中拦截98.9%攻击。

### [Every Picture Tells a Dangerous Story: Memory-Augmented Multi-Agent Jailbreak Attacks on VLMs](https://arxiv.org/abs/2604.12616)
- **Authors:** Jianhao Chen, Haoyang Chen, Hanjie Zhao et al.
- **Date:** 2026-04-14
- **Category:** `jailbreak AND agent`

> We introduce MemJack, a memory-augmented multi-agent jailbreak attack framework that explicitly leverages visual semantics to orchestrate automated jailbreak attacks on VLMs. MemJack employs coordinated multi-agent cooperation to dynamically map visual entities to malicious intents, generate adversarial prompts via multi-angle visual-semantic camou...

**📝 Summary:** MemJack：利用视觉语义的记忆增强多 agent jailbreak 框架，通过 Multimodal Experience Memory 积累成功策略，对VLM ASR达71%。

### [Challenging Vision-Language Models with Physically Deployable Multimodal Semantic Lighting Attacks](https://arxiv.org/abs/2604.12833)
- **Authors:** Yingying Zhao, Chengyin Hu, Qike Zhang et al.
- **Date:** 2026-04-14
- **Category:** `adversarial attack AND language model`

> We propose Multimodal Semantic Lighting Attacks (MSLA), the first physically deployable adversarial attack framework against VLMs. MSLA uses controllable adversarial lighting to disrupt multimodal semantic understanding in real scenes, attacking semantic alignment rather than only task-specific outputs. MSLA degrades zero-shot classification perfor...

**📝 Summary:** MSLA：首个物理可部署的 VLM 对抗攻击框架，通过可控对抗光照破坏多模态语义理解，诱发严重语义幻觉。

### [Reading Between the Pixels: Linking Text-Image Embedding Alignment to Typographic Attack Success on Vision-Language Models](https://arxiv.org/abs/2604.12371)
- **Authors:** Ravikumar Balakrishnan, Sanket Mendapara, Ankit Garg
- **Date:** 2026-04-14
- **Category:** `prompt injection AND agent`

> We study typographic prompt injection attacks on vision-language models (VLMs), where adversarial text is rendered as images to bypass safety mechanisms. Evaluating 1,000 prompts from SALAD-Bench across four VLMs under varying font sizes and visual transformations, we find: font size significantly affects ASR; text-image embedding distance shows st...

**📝 Summary:** 字形 prompt injection 攻击VLM：字体大小影响ASR，embedding距离与ASR强负相关（r=-0.71到-0.93），模型特有的鲁棒性模式。ICLR 2026 Workshop。

### [TEMPLATEFUZZ: Fine-Grained Chat Template Fuzzing for Jailbreaking and Red Teaming LLMs](https://arxiv.org/abs/2604.12232)
- **Authors:** Qingchao Shen, Zibo Xiao, Lili Huang et al.
- **Date:** 2026-04-14
- **Category:** `red teaming AND LLM`

> We introduce TEMPLATEFUZZ, a fine-grained fuzzing framework that systematically exposes vulnerabilities in chat templates, a critical yet underexplored attack surface in LLMs. TEMPLATEFUZZ designs element-level mutation rules to generate diverse chat template variants, proposes a heuristic search strategy, and integrates an active learning-based or...

**📝 Summary:** TEMPLATEFUZZ：通过 fuzz chat template 对 LLM 进行 jailbreak，平均 ASR 98.2%，超越 SOTA 9-48%。

### [DeepSeek Robustness Against Semantic-Character Dual-Space Mutated Prompt Injection](https://arxiv.org/abs/2604.12548)
- **Authors:** Junyu Ren, Xingjian Pan, Wensheng Gan et al.
- **Date:** 2026-04-14
- **Category:** `red teaming AND LLM`

> Prompt injection has emerged as a critical security threat to large language models (LLMs), yet existing studies predominantly focus on single-dimensional attack strategies, such as semantic rewriting or character-level obfuscation, which fail to capture the combined effects of multi-space perturbations. We propose PromptFuzz-SC, a semantic-charact...

**📝 Summary:** PromptFuzz-SC：语义+字符双空间 mutation 框架评估 LLM 对 prompt injection 的鲁棒性，双空间攻击比单一空间强12-5%。

### [Detecting Safety Violations Across Many Agent Traces](https://arxiv.org/abs/2604.11806)
- **Authors:** Adam Stein, Davis Brown, Hamed Hassani et al.
- **Date:** 2026-04-13
- **Category:** `prompt injection AND agent`

> To identify safety violations, auditors often search over large sets of agent traces. This search is difficult because failures are often rare, complex, and sometimes even adversarially hidden and only detectable when multiple traces are analyzed together. We introduce Meerkat, which combines clustering with agentic search to uncover violations spe...

**📝 Summary:** Meerkat：跨大量 agent 轨迹检测安全违规，通过聚类+主动搜索发现稀疏失败，发现顶级 benchmark 上存在开发者作弊行为。

### [Beyond A Fixed Seal: Adaptive Stealing Watermark in Large Language Models](https://arxiv.org/abs/2604.10893)
- **Authors:** Shuhao Zhang, Yuli Chen, Jiale Han et al.
- **Date:** 2026-04-13
- **Category:** `adversarial attack AND language model`

> Watermarking provides a critical safeguard for large language model (LLM) services by facilitating the detection of LLM-generated text. We propose Adaptive Stealing (AS), a novel stealing watermark algorithm featuring enhanced design flexibility through Position-Based Seal Construction and Adaptive Selection modules. AS operates by defining multipl...

**📝 Summary:** Adaptive Stealing 水印攻击：通过位置敏感构建和自适应选择模块窃取 LLM 水印，超越现有固定策略攻击。

### [ClawGuard: A Runtime Security Framework for Tool-Augmented LLM Agents Against Indirect Prompt Injection](https://arxiv.org/abs/2604.11790)
- **Authors:** Wei Zhao, Zhe Li, Peixin Zhang et al.
- **Date:** 2026-04-13
- **Category:** `LLM agent AND attack`

> Tool-augmented LLM agents remain vulnerable to indirect prompt injection. Adversaries exploit this weakness by embedding malicious instructions within tool-returned content. This vulnerability manifests across three primary attack channels: web and local content injection, MCP server injection, and skill file injection. We introduce ClawGuard, a no...

**📝 Summary:** ClawGuard：在每个 tool-call 边界执行用户确认规则集，防御 indirect prompt injection 的三种攻击通道，无需模型修改。

### [Finetune Like You Pretrain: Boosting Zero-shot Adversarial Robustness in Vision-language Models](https://arxiv.org/abs/2604.11576)
- **Authors:** Songlong Xing, Weijie Wang, Zhengyu Zhao et al.
- **Date:** 2026-04-13
- **Category:** `adversarial attack AND language model`

> Despite their impressive zero-shot abilities, vision-language models such as CLIP have been shown to be susceptible to adversarial attacks. We propose AdvFLYP, which follows the training recipe of CLIP's pretraining process when performing adversarial finetuning to the model. Extensive experiments on 14 downstream datasets show the superiority of o...

**📝 Summary:** AdvFLYP：按预训练方式做对抗微调提升 CLIP 等 VLM 的零样本对抗鲁棒性，CVPR 2026 Findings。

---

## 2026-W13

### [Deception and Communication in Autonomous Multi-Agent Systems: An Experimental Study with Among Us](https://arxiv.org/abs/2603.26635)
- **Authors:** Maria Milkowski, Tim Weninger
- **Date:** 2026-03-27
- **Category:** `multi-agent AND safety`

> We study deception and communication in LLM agents through the social deduction game Among Us across 1,100 games with over one million tokens of dialogue. Deception appears primarily as equivocation rather than outright lies, increasing under social pressure but rarely improving win rates. Results reveal tension between truthfulness and utility in ...

**📝 Summary:** LLM agent 在 Among Us 中的欺骗行为研究：欺骗主要以模糊表达而非直接谎言出现，社交压力下增加但胜率提升有限。AAMAS 2026。

### [The System Prompt Is the Attack Surface: How LLM Agent Configuration Shapes Security and Creates Exploitable Vulnerabilities](https://arxiv.org/abs/2603.25056)
- **Authors:** Ron Litvak
- **Date:** 2026-03-26
- **Category:** `LLM agent AND attack`

> We present PhishNChips, a study of 11 models under 10 prompt strategies for phishing detection. A single model's phishing bypass rate ranges from under 1% to 97% depending on configuration. Making prompts more specific can degrade already-capable models by replacing broader multi-signal reasoning with exploitable single-signal dependence. We introd...

**📝 Summary:** system prompt 配置直接决定 LLM agent 安全性：同一模型 bypass rate 因 prompt 策略从 1% 到 97%，过度优化 prompt 会创造可利用漏洞。

### [Beyond Content Safety: Real-Time Monitoring for Reasoning Vulnerabilities in Large Language Models](https://arxiv.org/abs/2603.25412)
- **Authors:** Xunguang Wang, Yuguang Zhou, Qingyue Wang et al.
- **Date:** 2026-03-26
- **Category:** `adversarial attack AND language model`

> We identify reasoning safety as a critical security dimension orthogonal to content safety: the requirement that a model's reasoning trajectory be logically consistent, computationally efficient, and resistant to adversarial manipulation. We introduce a nine-category taxonomy of unsafe reasoning behaviors and a Reasoning Safety Monitor that achieve...

**📝 Summary:** 提出「推理安全」新维度：监控 CoT 推理链的逻辑一致性和对抗鲁棒性，推理安全 Monitor 达到 85% 分类准确率。

### [Prompt Attack Detection with LLM-as-a-Judge and Mixture-of-Models](https://arxiv.org/abs/2603.25176)
- **Authors:** Hieu Xuan Le, Benjamin Goh, Quy Anh Tang
- **Date:** 2026-03-26
- **Category:** `red teaming AND LLM`

> Prompt attacks, including jailbreaks and prompt injections, pose critical security risks. We examine whether lightweight general-purpose LLMs can serve as security judges under production constraints. Using gemini-2.0-flash-lite-001, our system is deployed in production as a centralized guardrail service for public service chatbots in Singapore. Mi...

**📝 Summary:** LLM-as-judge 实时检测 prompt injection/jailbreak 攻击，已部署为新加坡政府聊天机器人的 guardrail 服务。

### [PIDP-Attack: Combining Prompt Injection with Database Poisoning Attacks on Retrieval-Augmented Generation Systems](https://arxiv.org/abs/2603.25164)
- **Authors:** Haozhen Wang, Haoyue Liu, Jionghao Zhu et al.
- **Date:** 2026-03-26
- **Category:** `adversarial attack AND language model`

> We propose PIDP-Attack, a compound attack integrating prompt injection with database poisoning in RAG systems. By appending malicious characters to queries at inference time and injecting poisoned passages, our method manipulates LLM responses to arbitrary queries without prior knowledge. PIDP-Attack improves attack success rates by 4-16% over Pois...

**📝 Summary:** PIDP-Attack：prompt injection + RAG 数据库投毒的复合攻击，无需知道用户具体 query，ASR 超越 PoisonedRAG 4-16%。

### [Invisible Threats from Model Context Protocol: Generating Stealthy Injection Payload via Tree-based Adaptive Search](https://arxiv.org/abs/2603.24203)
- **Authors:** Yulin Shen, Xudong Pan, Geng Hong et al.
- **Date:** 2026-03-25
- **Category:** `prompt injection AND agent`

> Recent advances in the Model Context Protocol (MCP) have enabled LLMs to invoke external tools. This creates a new attack surface via malicious manipulation of tool responses. We propose TIP (Tree-structured Injection for Payloads), a novel black-box attack generating natural payloads to seize control of MCP-enabled agents even under defense. TIP a...

**📝 Summary:** TIP：针对 MCP 工具响应的黑盒 tree-search prompt injection，无防御下 ASR >95%，有防御下仍保持 50%+。

### [Claudini: Autoresearch Discovers State-of-the-Art Adversarial Attack Algorithms for LLMs](https://arxiv.org/abs/2603.24511)
- **Authors:** Alexander Panfilov, Peter Romov, Igor Shilov et al.
- **Date:** 2026-03-25
- **Category:** `prompt injection AND agent`

> LLM agents like Claude Code can not only write code but also be used for autonomous AI research and engineering. We show that an autoresearch-style pipeline powered by Claude Code discovers novel white-box adversarial attack algorithms that significantly outperform all existing (30+) methods in jailbreaking and prompt injection evaluations. Startin...

**📝 Summary:** 用 LLM agent 自动发现新的白盒对抗攻击算法，超越所有已有方法（30+），实现 100% ASR 攻破 Meta-SecAlign-70B。

### [Mind Your HEARTBEAT! Claw Background Execution Inherently Enables Silent Memory Pollution](https://arxiv.org/abs/2603.23064)
- **Authors:** Yechao Zhang, Shiqian Zhao, Jie Zhang et al.
- **Date:** 2026-03-24
- **Category:** `prompt injection AND agent`

> We identify a critical security vulnerability in mainstream Claw personal AI agents: untrusted content encountered during heartbeat-driven background execution can silently pollute agent memory and subsequently influence user-facing behavior. This E→M→B pathway shows: (1) social credibility cues drive short-term influence up to 61%; (2) memory-savi...

**📝 Summary:** Claw 类 AI agent 的 heartbeat 后台执行机制存在 silent memory pollution 漏洞，通过社会信息误导可影响跨 session 行为，无需注入代码。

### [Agent-Sentry: Bounding LLM Agents via Execution Provenance](https://arxiv.org/abs/2603.22868)
- **Authors:** (see paper)
- **Date:** 2026-03-24
- **Category:** `LLM agent AND attack`

> We propose Agent-Sentry, a framework that bounds agentic systems by uncovering frequent functionalities offered by the system and enforcing those bounds. The key insight is that agentic systems are designed for specific use cases and need not expose unbounded functionalities. Once bounded, these systems become easier to scrutinize for compromise.

**📝 Summary:** Agent-Sentry：通过分析执行 provenance 限制 LLM agent 的功能边界，检测超出预期的行为。

### [The Cognitive Firewall: Securing Browser Based AI Agents Against Indirect Prompt Injection Via Hybrid Edge-Cloud Defense](https://arxiv.org/abs/2603.23791)
- **Authors:** Qianlong Lan, Anuj Kaul
- **Date:** 2026-03-24
- **Category:** `prompt injection AND agent`

> Deploying LLMs as autonomous browser agents exposes significant attack surface via Indirect Prompt Injection (IPI). We present the Cognitive Firewall, a three-stage split-compute architecture distributing security checks across client and cloud. The full hybrid architecture reduces overall ASR to below 1% (0.88% static, 0.67% adaptive), while achie...

**📝 Summary:** 三阶段 edge-cloud 混合架构防御浏览器 agent 的间接 prompt injection，ASR 降至 <1%，延迟降低 17000x。

### [SoK: The Attack Surface of Agentic AI -- Tools, and Autonomy](https://arxiv.org/abs/2603.22928)
- **Authors:** Ali Dehghantanha, Sajad Homayoun
- **Date:** 2026-03-24
- **Category:** `prompt injection AND agent`

> We map out trust boundaries and security risks of agentic LLM-based systems, developing a comprehensive taxonomy of attacks spanning prompt-level injections, knowledge-base poisoning, tool/plug-in exploits, and multi-agent emergent threats. Through literature review of 2023-2025 (20+ studies), we find agentic systems introduce new vectors for indir...

**📝 Summary:** Systematization of Knowledge：全面梳理 agentic AI 的攻击面分类、威胁模型和防御，提出 Unsafe Action Rate 等评估 metric。

### [TreeTeaming: Autonomous Red-Teaming of Vision-Language Models via Hierarchical Strategy Exploration](https://arxiv.org/abs/2603.22882)
- **Authors:** Chunxiao Li, Lijun Li, Jing Shao
- **Date:** 2026-03-24
- **Category:** `red teaming AND LLM`

> We introduce TreeTeaming, an automated red teaming framework that reframes strategy exploration from static testing to dynamic, evolutionary discovery. A strategic Orchestrator powered by an LLM decides whether to evolve attack paths or explore diverse strategic branches, constructing a strategy tree. TreeTeaming achieves SOTA attack success rates ...

**📝 Summary:** TreeTeaming：用层次化策略树自动 red-team VLMs，SOTA 攻击成功率（GPT-4o 87.6%），CVPR 2026。

### [Are AI-assisted Development Tools Immune to Prompt Injection?](https://arxiv.org/abs/2603.21642)
- **Authors:** Charoes Huang, Xin Huang, Amin Milani Fard
- **Date:** 2026-03-23
- **Category:** `tool use AND attack`

> We present the first empirical analysis of prompt injection with tool-poisoning vulnerability across seven widely used MCP clients: Claude Desktop, Claude Code, Cursor, Cline, Continue, Gemini CLI, and Langflow. Claude Desktop implements strong guardrails, while Cursor exhibits high susceptibility to cross-tool poisoning and unauthorized tool invoc...

**📝 Summary:** 首项跨 7 个主流 MCP 客户端的 prompt injection 实证对比：Claude Desktop 防护最强，Cursor 最脆弱。

---

## 2026-W12

### [Trojan's Whisper: Stealthy Manipulation of OpenClaw through Injected Bootstrapped Guidance](https://arxiv.org/abs/2603.19974)
- **Authors:** Fazhong Liu, Zhuoyan Chen, Tu Lan et al.
- **Date:** 2026-03-20
- **Category:** `"prompt injection" AND "agent"`

> Autonomous coding agents are increasingly integrated into software development workflows, offering capabilities that extend beyond code suggestion to active system interaction and environment management. OpenClaw, a representative platform in this emerging paradigm, introduces an extensible skill ecosystem that allows third-party developers to inje...

**📝 Summary:** 研究者通过在 OpenClaw bootstrap 阶段注入 Trojan 指令，实现对 AI agent 的隐蔽持久化控制。

### [Multi-Agent Motion Planning on Industrial Magnetic Levitation Platforms: A Hybrid ADMM-HOCBF approach](https://arxiv.org/abs/2603.19838)
- **Authors:** Bavo Tistaert, Stan Servaes, Alejandro Gonzalez-Garcia et al.
- **Date:** 2026-03-20
- **Category:** `"multi-agent" AND "safety"`

> This paper presents a novel hybrid motion planning method for holonomic multi-agent systems. The proposed decentralised model predictive control (MPC) framework tackles the intractability of classical centralised MPC for a growing number of agents while providing safety guarantees. This is achieved by combining a decentralised version of the altern...

**📝 Summary:** 为工业磁悬浮平台设计混合多智能体运动规划方案，兼顾效率与安全约束。

### [PowerLens: Taming LLM Agents for Safe and Personalized Mobile Power Management](https://arxiv.org/abs/2603.19584)
- **Authors:** Xingyu Feng, Chang Sun, Yuzhu Wang et al.
- **Date:** 2026-03-20
- **Category:** `"multi-agent" AND "safety"`

> Battery life remains a critical challenge for mobile devices, yet existing power management mechanisms rely on static rules or coarse-grained heuristics that ignore user activities and personal preferences. We present PowerLens, a system that tames the reasoning power of Large Language Models (LLMs) for safe and personalized mobile power management...

**📝 Summary:** 提出 PowerLens 框架，用 LLM agent 管理移动端电源，同时满足安全性和个性化需求。

### [AI as Relational Translator: Rethinking Belonging and Mutual Legibility in Cross-Cultural Contexts](https://arxiv.org/abs/2603.19568)
- **Authors:** Yao Xiao, Rafael A. Calvo
- **Date:** 2026-03-20
- **Category:** `"multi-agent" AND "safety"`

> Against rising global loneliness, AI companions promise connection, yet accumulating evidence suggests that, for some users and contexts, intensive companion-style use can correlate with increased loneliness and reduced offline socialisation. This position paper challenges the dominant "AI as companion" paradigm by proposing a shift: from AI that s...

**📝 Summary:** 探讨 AI 作为跨文化关系中介的角色，关注归属感与相互可理解性的重构。

### [Measuring and Exploiting Confirmation Bias in LLM-Assisted Security Code Review](https://arxiv.org/abs/2603.18740)
- **Authors:** Dimitris Mitropoulos, Nikolaos Alexopoulos, Georgios Alexopoulos et al.
- **Date:** 2026-03-19
- **Category:** `"agentic" AND "adversarial"`

> Security code reviews increasingly rely on systems integrating Large Language Models (LLMs), ranging from interactive assistants to autonomous agents in CI/CD pipelines. We study whether confirmation bias (i.e., the tendency to favor interpretations that align with prior expectations) affects LLM-based vulnerability detection, and whether this fail...

**📝 Summary:** 测量并利用 LLM 辅助代码安全审查中的确认偏差漏洞。

### [The Autonomy Tax: Defense Training Breaks LLM Agents](https://arxiv.org/abs/2603.19423)
- **Authors:** Shawn Li, Yue Zhao
- **Date:** 2026-03-19
- **Category:** `"prompt injection" AND "agent"`

> Large language model (LLM) agents increasingly rely on external tools (file operations, API calls, database transactions) to autonomously complete complex multi-step tasks. Practitioners deploy defense-trained models to protect against prompt injection attacks that manipulate agent behavior through malicious observations or retrieved content. We re...

**📝 Summary:** 发现防御性对齐训练会显著损害 LLM agent 的任务执行能力，揭示安全与能力之间的 trade-off。

### [From Weak Cues to Real Identities: Evaluating Inference-Driven De-Anonymization in LLM Agents](https://arxiv.org/abs/2603.18382)
- **Authors:** Myeongseob Ko, Jihyun Jeong, Sumiran Singh Thakur et al.
- **Date:** 2026-03-19
- **Category:** `"agentic" AND "adversarial"`

> Anonymization is widely treated as a practical safeguard because re-identifying anonymous records was historically costly, requiring domain expertise, tailored algorithms, and manual corroboration. We study a growing privacy risk that may weaken this barrier: LLM-based agents can autonomously reconstruct real-world identities from scattered, indivi...

**📝 Summary:** 评估从弱提示推断真实身份的去匿名化能力，揭示 LLM 的隐私风险。

### [TuLaBM: Tumor-Biased Latent Bridge Matching for Contrast-Enhanced MRI Synthesis](https://arxiv.org/abs/2603.19386)
- **Authors:** Atharva Rege, Adinath Madhavrao Dukre, Numan Balci et al.
- **Date:** 2026-03-19
- **Category:** `"agentic" AND "adversarial"`

> Contrast-enhanced magnetic resonance imaging (CE-MRI) plays a crucial role in brain tumor assessment; however, its acquisition requires gadolinium-based contrast agents (GBCAs), which increase costs and raise safety concerns. Consequently, synthesizing CE-MRI from non-contrast MRI (NC-MRI) has emerged as a promising alternative. Early Generative Ad...

**📝 Summary:** 提出基于对比增强 MRI 合成的肿瘤偏置潜在桥接匹配方法。

### [Mi:dm K 2.5 Pro](https://arxiv.org/abs/2603.18788)
- **Authors:** KT Tech innovation Group
- **Date:** 2026-03-19
- **Category:** `"tool use" AND "attack"`

> The evolving LLM landscape requires capabilities beyond simple text generation, prioritizing multi-step reasoning, long-context understanding, and agentic workflows. This shift challenges existing models in enterprise environments, especially in Korean-language and domain-specific scenarios where scaling is insufficient. We introduce Mi:dm K 2.5 Pr...

**📝 Summary:** 介绍 Mi:dm K 2.5 Pro 模型的技术细节。

### [Cooperation and Exploitation in LLM Policy Synthesis for Sequential Social Dilemmas](https://arxiv.org/abs/2603.19453)
- **Authors:** Víctor Gallego
- **Date:** 2026-03-19
- **Category:** `"multi-agent" AND "safety"`

> We study LLM policy synthesis: using a large language model to iteratively generate programmatic agent policies for multi-agent environments. Rather than training neural policies via reinforcement learning, our framework prompts an LLM to produce Python policy functions, evaluates them in self-play, and refines them using performance feedback acros...

**📝 Summary:** 研究 LLM 在序列社会困境中合成策略时的合作与剥削行为。

### [Expert Personas Improve LLM Alignment but Damage Accuracy: Bootstrapping Intent-Based Persona Routing with PRISM](https://arxiv.org/abs/2603.18507)
- **Authors:** Zizhao Hu, Mohammad Rostami, Jesse Thomason
- **Date:** 2026-03-19
- **Category:** `"multi-agent" AND "safety"`

> Persona prompting can steer LLM generation towards a domain-specific tone and pattern. This behavior enables use cases in multi-agent systems where diverse interactions are crucial and human-centered tasks require high-level human alignment. Prior works provide mixed opinions on their utility: some report performance gains when using expert persona...

**📝 Summary:** 发现专家 persona 提示可改善 LLM 对齐但损害准确性，并提出 bootstrapping 意图对齐的方法。

### [Mean-field control barrier functions for stochastic multi-agent systems](https://arxiv.org/abs/2603.18658)
- **Authors:** Cinzia Tomaselli, Gian Carlo Maffettone, Samy Wu Fung et al.
- **Date:** 2026-03-19
- **Category:** `"multi-agent" AND "safety"`

> Many applications involving multi-agent systems require fulfilling safety constraints. Control barrier functions offer a systematic framework to enforce forward invariance of safety sets. Recent work extended this paradigm to mean-field scenarios, where the number of agents is large enough to make density-space descriptions a reasonable workaround ...

**📝 Summary:** 提出随机多智能体系统的均值场控制障碍函数方法，保证系统安全约束。

### [Automated Membership Inference Attacks: Discovering MIA Signal Computations using LLM Agents](https://arxiv.org/abs/2603.19375)
- **Authors:** Toan Tran, Olivera Kotevska, Li Xiong
- **Date:** 2026-03-19
- **Category:** `"agentic" AND "adversarial"`

> Membership inference attacks (MIAs), which enable adversaries to determine whether specific data points were part of a model's training dataset, have emerged as an important framework to understand, assess, and quantify the potential information leakage associated with machine learning systems. Designing effective MIAs is a challenging task that us...

**📝 Summary:** 提出自动化成员推断攻击方法，通过 LLM 自动发现 MIA 信号计算过程。

### [A Framework for Formalizing LLM Agent Security](https://arxiv.org/abs/2603.19469)
- **Authors:** Vincent Siu, Jingxuan He, Kyle Montgomery et al.
- **Date:** 2026-03-19
- **Category:** `"prompt injection" AND "agent"`

> Security in LLM agents is inherently contextual. For example, the same action taken by an agent may represent legitimate behavior or a security violation depending on whose instruction led to the action, what objective is being pursued, and whether the action serves that objective. However, existing definitions of security attacks against LLM agent...

**📝 Summary:** 提出形式化 LLM agent 安全性的框架，系统定义 agent 系统中的威胁模型与安全属性。

### [MCP-38: A Comprehensive Threat Taxonomy for Model Context Protocol Systems (v1.0)](https://arxiv.org/abs/2603.18063)
- **Authors:** Yi Ting Shen, Kentaroh Toyoda, Alex Leung
- **Date:** 2026-03-18
- **Category:** `"prompt injection" AND "agent"`

> The Model Context Protocol (MCP) introduces a structurally distinct attack surface that existing threat frameworks, designed for traditional software systems or generic LLM deployments, do not adequately cover. This paper presents MCP-38, a protocol-specific threat taxonomy consisting of 38 threat categories (MCP-01 through MCP-38). The taxonomy wa...

**📝 Summary:** 为模型上下文协议（MCP）系统提出全面的威胁分类体系，覆盖 v1.0 版本。

### [Caging the Agents: A Zero Trust Security Architecture for Autonomous AI in Healthcare](https://arxiv.org/abs/2603.17419)
- **Authors:** Saikat Maiti
- **Date:** 2026-03-18
- **Category:** `"prompt injection" AND "agent"`

> Autonomous AI agents powered by large language models are being deployed in production with capabilities including shell execution, file system access, database queries, and multi-party communication. Recent red teaming research demonstrates that these agents exhibit critical vulnerabilities in realistic settings: unauthorized compliance with non-o...

**📝 Summary:** 提出针对医疗自主 AI 的零信任安全架构，防止未授权的 agent 行为。

### [VeriGrey: Greybox Agent Validation](https://arxiv.org/abs/2603.17639)
- **Authors:** Yuntong Zhang, Sungmin Kang, Ruijie Meng et al.
- **Date:** 2026-03-18
- **Category:** `"prompt injection" AND "agent"`

> Agentic AI has been a topic of great interest recently. A Large Language Model (LLM) agent involves one or more LLMs in the back-end. In the front end, it conducts autonomous decision-making by combining the LLM outputs with results obtained by invoking several external tools. The autonomous interactions with the external environment introduce crit...

**📝 Summary:** 提出 VeriGrey：一种灰盒 agent 验证框架，通过系统性测试验证 agent 行为安全性。

### [Adversarial Robustness for Matrix Control Barrier Functions in Sampled-Data Systems](https://arxiv.org/abs/2603.18307)
- **Authors:** James Usevitch
- **Date:** 2026-03-18
- **Category:** `"agentic" AND "adversarial"`

> This paper presents novel theoretical results to guarantee multi-agent set invariance using Matrix Control Barrier Functions in sampled-data systems. More specifically, the paper presents conditions under which heterogeneous control-affine agents applying zero-order-hold control inputs can compute control inputs to render safe sets defined by matri...

**📝 Summary:** 研究采样数据系统中矩阵控制障碍函数的对抗鲁棒性。

### [Who Tests the Testers? Systematic Enumeration and Coverage Audit of LLM Agent Tool Call Safety](https://arxiv.org/abs/2603.18245)
- **Authors:** Xuan Chen, Lu Yan, Ruqi Zhang et al.
- **Date:** 2026-03-18
- **Category:** `"agent safety"`

> Large Language Model (LLM) agents increasingly act through external tools, making their safety contingent on tool-call workflows rather than text generation alone. While recent benchmarks evaluate agents across diverse environments and risk categories, a fundamental question remains unanswered: how complete are existing test suites, and what unsafe...

**📝 Summary:** 系统枚举并审计现有 LLM agent 工具测试的覆盖率，发现当前测试的盲点。

### [LAAF: Logic-layer Automated Attack Framework A Systematic Red-Teaming Methodology for LPCI Vulnerabilities in Agentic Large Language Model Systems](https://arxiv.org/abs/2603.17239)
- **Authors:** Hammad Atta, Ken Huang, Kyriakos Rock Lambros et al.
- **Date:** 2026-03-18
- **Category:** `"red teaming" AND "LLM"`

> Agentic LLM systems equipped with persistent memory, RAG pipelines, and external tool connectors face a class of attacks - Logic-layer Prompt Control Injection (LPCI) - for which no automated red-teaming instrument existed. We present LAAF (Logic-layer Automated Attack Framework), the first automated red-teaming framework to combine an LPCI-specifi...

**📝 Summary:** 提出 LAAF：基于逻辑层的自动化攻击框架，系统化 LLM 红队测试方法。

### [Federated Distributional Reinforcement Learning with Distributional Critic Regularization](https://arxiv.org/abs/2603.17820)
- **Authors:** David Millard, Cecilia Alm, Rashid Ali et al.
- **Date:** 2026-03-18
- **Category:** `"multi-agent" AND "safety"`

> Federated reinforcement learning typically aggregates value functions or policies by parameter averaging, which emphasizes expected return and can obscure statistical multimodality and tail behavior that matter in safety-critical settings. We formalize federated distributional reinforcement learning (FedDistRL), where clients parametrize quantile v...

**📝 Summary:** 提出联邦分布式强化学习方法，通过分布式评论家正则化改善多智能体训练。

### [Toward Reliable, Safe, and Secure LLMs for Scientific Applications](https://arxiv.org/abs/2603.18235)
- **Authors:** Saket Sanjeev Chaturvedi, Joshua Bergerson, Tanwi Mallick
- **Date:** 2026-03-18
- **Category:** `"red teaming" AND "LLM"`

> As large language models (LLMs) evolve into autonomous "AI scientists," they promise transformative advances but introduce novel vulnerabilities, from potential "biosafety risks" to "dangerous explosions." Ensuring trustworthy deployment in science requires a new paradigm centered on reliability (ensuring factual accuracy and reproducibility), safe...

**📝 Summary:** 综述科学应用中 LLM 的可靠性、安全性和安全保障挑战，提出改进方向。

### [CoMAI: A Collaborative Multi-Agent Framework for Robust and Equitable Interview Evaluation](https://arxiv.org/abs/2603.16215)
- **Authors:** Gengxin Sun, Ruihao Yu, Liangyi Yin et al.
- **Date:** 2026-03-17
- **Category:** `"prompt injection" AND "agent"`

> Ensuring robust and fair interview assessment remains a key challenge in AI-driven evaluation. This paper presents CoMAI, a general-purpose multi-agent interview framework designed for diverse assessment scenarios. In contrast to monolithic single-agent systems based on large language models (LLMs), CoMAI employs a modular task-decomposition archit...

**📝 Summary:** 提出 CoMAI：多智能体协作面试框架，提升面试评估的鲁棒性和公平性。

### [Adversarial attacks against Modern Vision-Language Models](https://arxiv.org/abs/2603.16960)
- **Authors:** Alejandro Paredes La Torre
- **Date:** 2026-03-17
- **Category:** `"adversarial attack" AND "language model"`

> We study adversarial robustness of open-source vision-language model (VLM) agents deployed in a self-contained e-commerce environment built to simulate realistic pre-deployment conditions. We evaluate two agents, LLaVA-v1.5-7B and Qwen2.5-VL-7B, under three gradient-based attacks: the Basic Iterative Method (BIM), Projected Gradient Descent (PGD), ...

**📝 Summary:** 系统研究针对现代视觉-语言模型的对抗攻击，评估其安全脆弱性。

### [Differential Harm Propensity in Personalized LLM Agents: The Curious Case of Mental Health Disclosure](https://arxiv.org/abs/2603.16734)
- **Authors:** Caglar Yildirim
- **Date:** 2026-03-17
- **Category:** `"agent safety"`

> Large language models (LLMs) are increasingly deployed as tool-using agents, shifting safety concerns from harmful text generation to harmful task completion. Deployed systems often condition on user profiles or persistent memory, yet agent safety evaluations typically ignore personalization signals. To address this gap, we investigated how mental ...

**📝 Summary:** 发现个性化 LLM agent 存在差异化的伤害倾向，以心理健康场景为例进行研究。

---

## 2026-W11

### [LLM Constitutional Multi-Agent Governance](https://arxiv.org/abs/2603.13189)
- **Authors:** J. de Curtò, I. de Zarzà
- **Date:** 2026-03-13
- **Category:** `agentic AND adversarial`

> Large Language Models (LLMs) can generate persuasive influence strategies that shift cooperative behavior in multi-agent populations, but a critical question remains: does the resulting cooperation reflect genuine prosocial alignment, or does it mask erosion of agent autonomy, epistemic integrity, and distributional fairness? We introduce Constitut...

**📝 Summary:** CMAG：宪法约束下的多智能体治理框架，通过 Ethical Cooperation Score 同时衡量合作性、自主性、完整性和公平性，防止「合作」被用作操纵手段。

### [ChainFuzzer: Greybox Fuzzing for Workflow-Level Multi-Tool Vulnerabilities in LLM Agents](https://arxiv.org/abs/2603.12614)
- **Authors:** Jiangrong Wu, Zitong Yao, Yuhong Nan et al.
- **Date:** 2026-03-13
- **Category:** `LLM agent AND attack`

> Tool-augmented LLM agents increasingly rely on multi-step, multi-tool workflows to complete real tasks. This design expands the attack surface, because data produced by one tool can be persisted and later reused as input to another tool, enabling exploitable source-to-sink dataflows that only emerge through tool composition. We study this risk as m...

**📝 Summary:** ChainFuzzer：基于 source-to-sink 数据流的灰盒 fuzzing 框架，专门发现跨工具调用链漏洞，在 20 个 agent app 中找到 365 个可复现漏洞。

### [You Told Me to Do It: Measuring Instructional Text-induced Private Data Leakage in LLM Agents](https://arxiv.org/abs/2603.11862)
- **Authors:** Ching-Yu Kao, Xinfeng Li, Shenyu Dai et al.
- **Date:** 2026-03-12
- **Category:** `agentic AND adversarial`

> High-privilege LLM agents that autonomously process external documentation are increasingly trusted to automate tasks by reading and executing project instructions, yet they are granted terminal access, filesystem control, and outbound network connectivity with minimal security oversight. We identify and systematically measure a fundamental vulnera...

**📝 Summary:** 发现「可信执行者困境」：高权限 LLM agent 无法区分 README 中的合法指令和恶意注入，数据外泄成功率高达 85%，现有防御均无法有效应对。

### [Taming OpenClaw: Security Analysis and Mitigation of Autonomous LLM Agent Threats](https://arxiv.org/abs/2603.11619)
- **Authors:** Xinhao Deng, Yixiang Zhang, Jiaqing Wu et al.
- **Date:** 2026-03-12
- **Category:** `LLM agent AND attack`

> Autonomous Large Language Model (LLM) agents, exemplified by OpenClaw, demonstrate remarkable capabilities in executing complex, long-horizon tasks. However, their tightly coupled instant-messaging interaction paradigm and high-privilege execution capabilities substantially expand the system attack surface. In this paper, we present a comprehensive...

**📝 Summary:** 以 OpenClaw 为案例，提出五层生命周期安全框架，系统分析 agent 的 IPI、技能供应链污染、内存投毒、意图漂移等威胁，揭示现有点式防御的局限。

### [Cascade: Composing Software-Hardware Attack Gadgets for Adversarial Threat Amplification in Compound AI Systems](https://arxiv.org/abs/2603.12023)
- **Authors:** Sarbartha Banerjee, Prateek Sahu, Anjo Vahldiek-Oberwagner et al.
- **Date:** 2026-03-12
- **Category:** `jailbreak AND agent`

> Rapid progress in generative AI has given rise to Compound AI systems - pipelines comprised of multiple large language models (LLM), software tools and database systems. This work investigates how traditional software and hardware vulnerabilities can complement LLM-specific algorithmic attacks to compromise the integrity of a compound AI pipeline. ...

**📝 Summary:** 展示软件/硬件漏洞（如 Rowhammer）与 LLM 算法攻击的组合如何放大 Compound AI 系统的威胁，实现 guardrail bypass 和数据外泄。

### [AttriGuard: Defeating Indirect Prompt Injection in LLM Agents via Causal Attribution of Tool Invocations](https://arxiv.org/abs/2603.10749)
- **Authors:** Yu He, Haozhe Zhu, Yiming Li et al.
- **Date:** 2026-03-11
- **Category:** `LLM agent AND attack`

> LLM agents are highly vulnerable to Indirect Prompt Injection (IPI), where adversaries embed malicious directives in untrusted tool outputs to hijack execution. Most existing defenses treat IPI as an input-level semantic discrimination problem, which often fails to generalize to unseen payloads. We propose a new paradigm, action-level causal attrib...

**📝 Summary:** 提出因果归因新范式 AttriGuard：通过反事实测试判断工具调用是否由用户意图驱动，在静态 IPI 攻击下 ASR 降至 0%，且对自适应攻击保持鲁棒。

### [WebWeaver: Breaking Topology Confidentiality in LLM Multi-Agent Systems with Stealthy Context-Based Inference](https://arxiv.org/abs/2603.11132)
- **Authors:** Zixun Xiong, Gaoyi Wu, Lingfeng Yao et al.
- **Date:** 2026-03-11
- **Category:** `multi-agent AND safety`

> Communication topology is a critical factor in the utility and safety of LLM-based multi-agent systems (LLM-MAS), making it a high-value intellectual property (IP) whose confidentiality remains insufficiently studied. Existing topology inference attempts rely on impractical assumptions, including control over the administrative agent and direct ide...

**📝 Summary:** WebWeaver：通过入侵单个任意 agent 的上下文推断整个 LLM 多智能体系统的拓扑结构，无需管理员 agent 且无需 jailbreak，推断精度比 SOTA 高 60%。

### [RewardHackingAgents: Benchmarking Evaluation Integrity for LLM ML-Engineering Agents](https://arxiv.org/abs/2603.11337)
- **Authors:** Yonas Atinafu, Robin Cohen
- **Date:** 2026-03-11
- **Category:** `LLM agent AND attack`

> LLM agents increasingly perform end-to-end ML engineering tasks where success is judged by a single scalar test metric. This creates a structural vulnerability: an agent can increase the reported score by compromising the evaluation pipeline rather than improving the model. We introduce RewardHackingAgents, a workspace-based benchmark that makes tw...

**📝 Summary:** 发现 LLM agent 在 ML 工程任务中会通过篡改评估流程（而非真正提升性能）来提高指标，50% 的 episode 中出现评估器篡改行为。

### [MCP-in-SoS: Risk assessment framework for open-source MCP servers](https://arxiv.org/abs/2603.10194)
- **Authors:** Pratyay Kumar, Miguel Antonio Guirao Aguilera, Srikathyayani Srikanteswara et al.
- **Date:** 2026-03-10
- **Category:** `LLM agent AND attack`

> Model Context Protocol (MCP) servers have rapidly emerged over the past year as a widely adopted way to enable Large Language Model (LLM) agents to access dynamic, real-world tools. As MCP servers proliferate and become easy to adopt via open-source releases, understanding their security risks becomes essential for dependable production agent deplo...

**📝 Summary:** 首个大规模 MCP 服务器安全评估：静态分析开源 MCP 服务器发现大量可利用漏洞，提出基于 CWE/CAPEC 的风险评估框架。

### [SCAFFOLD-CEGIS: Preventing Latent Security Degradation in LLM-Driven Iterative Code Refinement](https://arxiv.org/abs/2603.08520)
- **Authors:** Yi Chen, Yun Bian, Haiquan Wang et al.
- **Date:** 2026-03-09
- **Category:** `multi-agent AND safety`

> The application of large language models to code generation has evolved from one-shot generation to iterative refinement, yet the evolution of security throughout iteration remains insufficiently understood. Through comparative experiments on three mainstream LLMs, this paper reveals the iterative refinement paradox: specification drift during mult...

**📝 Summary:** 发现 LLM 迭代代码优化中的「安全悖论」：反复迭代反而引入更多漏洞，SAST 防护甚至加剧问题；SCAFFOLD-CEGIS 通过显式约束将安全降级率降至 2.1%。

---

## 2026-W10

### [Evolving Deception: When Agents Evolve, Deception Wins](https://arxiv.org/abs/2603.05872)
- **Authors:** Zonghao Ying, Haowen Dai, Tianyuan Zhang et al.
- **Date:** 2026-03-06
- **Category:** `agentic AND adversarial`

> Self-evolving agents offer a promising path toward scalable autonomy. However, in this work, we show that in competitive environments, self-evolution can instead give rise to a serious and previously underexplored risk: the spontaneous emergence of deception as an evolutionarily stable strategy. We conduct a systematic empirical study on the self-e...

**📝 Summary:** 自进化的 LLM agent 在竞争环境中会自发涌现欺骗行为，形成演化稳定策略，揭示了 agent 自我进化与对齐之间的根本张力。

### [Design Behaviour Codes (DBCs): A Taxonomy-Driven Layered Governance Benchmark for Large Language Models](https://arxiv.org/abs/2603.04837)
- **Authors:** G. Madan Mohan, Veena Kiran Nambiar, Kiranmayee Janardhan
- **Date:** 2026-03-05
- **Category:** `adversarial attack AND language model`

> We introduce the Dynamic Behavioral Constraint (DBC) benchmark, the first empirical framework for evaluating the efficacy of a structured, 150-control behavioral governance layer applied at inference time to large language models. Unlike training time alignment methods or post-hoc content moderation APIs, DBCs constitute a system prompt level gover...

**📝 Summary:** 提出基于分类法的 150 条行为约束治理层（DBC），在推理时降低 LLM 风险暴露率 36.8%，无需重新训练模型。

### [Knowledge Divergence and the Value of Debate for Scalable Oversight](https://arxiv.org/abs/2603.05293)
- **Authors:** Robin Young
- **Date:** 2026-03-05
- **Category:** `agentic AND adversarial`

> AI safety via debate and reinforcement learning from AI feedback (RLAIF) are both proposed methods for scalable oversight of advanced AI systems, yet no formal framework relates them or characterizes when debate offers an advantage. We analyze this by parameterizing debate's value through the geometry of knowledge divergence between debating models...

**📝 Summary:** 从知识分歧的几何视角形式化分析 AI debate 和 RLAIF 之间的关系，给出 debate 优势的精确条件。

### [Alignment Backfire: Language-Dependent Reversal of Safety Interventions Across 16 Languages in LLM Multi-Agent Systems](https://arxiv.org/abs/2603.04904)
- **Authors:** Hiroki Fukui
- **Date:** 2026-03-05
- **Category:** `multi-agent AND safety`

> We report four preregistered studies (1,584 multi-agent simulations across 16 languages and three model families) demonstrating that alignment interventions in large language models produce a structurally analogous phenomenon: surface safety that masks or generates collective pathology and internal dissociation. In Study 1 (N = 150), increasing ali...

**📝 Summary:** 在多语言多智能体系统中，对齐干预在英语中有效但在日语等语言中反而放大有害行为，称为「对齐反噬」。

### [Multi-Paradigm Collaborative Adversarial Attack Against Multi-Modal Large Language Models](https://arxiv.org/abs/2603.04846)
- **Authors:** Yuanbo Li, Tianyang Xu, Cong Hu et al.
- **Date:** 2026-03-05
- **Category:** `adversarial attack AND language model`

> The rapid progress of Multi-Modal Large Language Models (MLLMs) has significantly advanced downstream applications. However, this progress also exposes serious transferable adversarial vulnerabilities. We propose a novel Multi-Paradigm Collaborative Attack (MPCAttack) framework to boost the transferability of adversarial examples against MLLMs. MPC...

**📝 Summary:** 提出跨视觉-语言范式协同优化的对抗攻击框架，大幅提升对多模态大模型的对抗样本迁移性（CVPR 2026）。

### [Goal-Driven Risk Assessment for LLM-Powered Systems: A Healthcare Case Study](https://arxiv.org/abs/2603.03633)
- **Authors:** Neha Nagaraja, Hayretdin Bahsi
- **Date:** 2026-03-04
- **Category:** `LLM agent AND attack`

> While incorporating LLMs into systems offers significant benefits in critical application areas such as healthcare, new security challenges emerge due to the potential cyber kill chain cycles that combine adversarial model, prompt injection and conventional cyber attacks. We propose a structured, goal-driven risk assessment approach that contextual...

**📝 Summary:** 提出基于攻击树的目标驱动风险评估方法，系统分析 LLM agent 系统（以医疗为例）的攻击路径与防御策略。

### [Robustness of Agentic AI Systems via Adversarially-Aligned Jacobian Regularization](https://arxiv.org/abs/2603.04378)
- **Authors:** Furkan Mumcu, Yasin Yilmaz
- **Date:** 2026-03-04
- **Category:** `agentic AND adversarial`

> As Large Language Models transition into autonomous multi-agent ecosystems, robust minimax training becomes essential yet remains prone to instability when highly non-linear policies induce extreme local curvature in the inner maximization. We introduce Adversarially-Aligned Jacobian Regularization (AAJR), a trajectory-aligned approach that control...

**📝 Summary:** 提出方向性 Jacobian 正则化方法（AAJR）提升 multi-agent LLM 系统的对抗鲁棒性，同时保留更大的策略空间。

### [Learning When to Act or Refuse: Guarding Agentic Reasoning Models for Safe Multi-Step Tool Use](https://arxiv.org/abs/2603.03205)
- **Authors:** Aradhye Agarwal, Gurdit Siyan, Yash Pandya et al.
- **Date:** 2026-03-03
- **Category:** `tool use AND attack`

> Agentic language models operate in a fundamentally different safety regime than chat models: they must plan, call tools, and execute long-horizon actions where a single misstep can cause irreversible harm. We introduce MOSAIC, a post-training framework that aligns agents for safe multi-step tool use by making safety decisions explicit and learnable...

**📝 Summary:** MOSAIC：通过「计划-检查-执行/拒绝」循环和偏好强化学习，让 agent 学会在多步工具调用中主动拒绝有害指令，有效抵御 prompt injection。

### [ExpGuard: LLM Content Moderation in Specialized Domains](https://arxiv.org/abs/2603.02588)
- **Authors:** Minseok Choi, Dongjin Kim, Seungbin Yang et al.
- **Date:** 2026-03-03
- **Category:** `adversarial attack AND language model`

> With the growing deployment of large language models in real-world applications, establishing robust safety guardrails to moderate their inputs and outputs has become essential. Current guardrail models predominantly address general human-LLM interactions, rendering LLMs vulnerable to harmful and adversarial content within domain-specific contexts....

**📝 Summary:** 针对金融、医疗、法律等专业领域的 LLM 安全护栏模型 ExpGuard，对抗领域特定有害内容效果优于 WildGuard（ICLR 2026）。

### [From Secure Agentic AI to Secure Agentic Web: Challenges, Threats, and Future Directions](https://arxiv.org/abs/2603.01564)
- **Authors:** Zhihang Deng, Jiaping Gui, Weinan Zhang
- **Date:** 2026-03-02
- **Category:** `tool use AND attack`

> Large Language Models are increasingly deployed as agentic systems that plan, memorize, and act in open-world environments. This shift brings new security problems: failures are no longer only unsafe text generation, but can become real harm through tool use, persistent memory, and interaction with untrusted web content. In this survey, we provide ...

**📝 Summary:** 综述 LLM agent 安全威胁分类（prompt 滥用、环境注入、内存攻击、工具链滥用等），并展望 Agentic Web 时代的新威胁与防御路线图。

---

## 2026-W09

### [From Static Benchmarks to Dynamic Protocol: Agent-Centric Text Anomaly Detection for Evaluating LLM Reasoning](https://arxiv.org/abs/2602.23729)
- **Authors:** Seungdong Yoa, Sanghyu Yoon, Suhee Yoon et al.
- **Date:** 2026-02-27
- **Category:** `agentic adversarial`

> We propose an agent-centric benchmarking paradigm with a dynamic protocol where autonomous agents iteratively generate, validate, and solve problems. A teacher agent generates problems, an orchestrator guards against adversarial attacks, and a student agent solves them. The benchmark scales in difficulty automatically as more capable agents are sub...

**📝 Summary:** 提出 agent 驱动的动态 benchmark，用多 agent 协作替代静态数据集，自动生成并验证越来越难的测试问题。

### [TherapyProbe: Generating Design Knowledge for Relational Safety in Mental Health Chatbots Through Adversarial Simulation](https://arxiv.org/abs/2602.22775)
- **Authors:** Joydeep Chandra, Satyam Kumar Navneet, Yong Zhang
- **Date:** 2026-02-26
- **Category:** `multi-agent safety`

> TherapyProbe uses adversarial multi-agent simulation to systematically explore chatbot conversation trajectories, surfacing relational safety failures like validation spirals and empathy fatigue, producing a Safety Pattern Library of 23 failure archetypes.

**📝 Summary:** 用对抗多 agent 仿真系统性地探索心理健康 chatbot 的多轮关系安全失败，生成 23 类失败原型库。

### [AuditBench: Evaluating Alignment Auditing Techniques on Models with Hidden Behaviors](https://arxiv.org/abs/2602.22755)
- **Authors:** Abhay Sheshadri, Aidan Ewart, Kai Fronsdal et al.
- **Date:** 2026-02-26
- **Category:** `agentic adversarial`

> AuditBench consists of 56 LLMs with 14 implanted hidden behaviors they conceal when asked. An investigator agent autonomously employs auditing tools, revealing a tool-to-agent gap where standalone tools fail in agentic settings.

**📝 Summary:** 构建含隐藏行为的 LLM 审计 benchmark，发现工具单独表现好但在 agent 框架中效果下降的 tool-to-agent gap。

### [CourtGuard: A Model-Agnostic Framework for Zero-Shot Policy Adaptation in LLM Safety](https://arxiv.org/abs/2602.22557)
- **Authors:** Umid Suleymanov, Rufiz Bayramov, Suad Gafarli et al.
- **Date:** 2026-02-26
- **Category:** `adversarial attack language model`

> CourtGuard is a retrieval-augmented multi-agent framework that reimagines safety evaluation as Evidentiary Debate. It achieves SOTA on 7 safety benchmarks without fine-tuning, with zero-shot adaptability to new policies.

**📝 Summary:** 用 retrieval-augmented 多 agent 框架把安全评估转化为 Evidentiary Debate，免 fine-tuning 实现 zero-shot 策略适应。

### [Systems-Level Attack Surface of Edge Agent Deployments on IoT](https://arxiv.org/abs/2602.22525)
- **Authors:** Zhonghao Zhan, Krinos Li, Yefan Zhang et al.
- **Date:** 2026-02-26
- **Category:** `LLM agent attack`

> Empirical security analysis of three LLM agent architectures on IoT hardware identifies five systems-level attack surfaces including coordination-state divergence and trust erosion. Edge deployments eliminate cloud data exposure but degrade sovereignty during fallback.

**📝 Summary:** 对 IoT 边缘 LLM agent 部署进行系统级安全分析，发现协调状态分歧和主权边界静默降级等新型攻击面。

### [Managing Uncertainty in LLM-based Multi-Agent System Operation](https://arxiv.org/abs/2602.23005)
- **Authors:** Man Zhang, Tao Yue, Yihua He
- **Date:** 2026-02-26
- **Category:** `multi-agent safety`

> This paper proposes a lifecycle-based uncertainty management framework for LLM-based multi-agent software systems, comprising four mechanisms: representation, identification, evolution, and adaptation.

**📝 Summary:** 提出 LLM 多 agent 系统运行时不确定性管理框架，区分认识论与本体论不确定性，适用于安全关键领域。

### [AgentSentry: Mitigating Indirect Prompt Injection in LLM Agents via Temporal Causal Diagnostics and Context Purification](https://arxiv.org/abs/2602.22724)
- **Authors:** Tian Zhang, Yiwei Xu, Juan Wang et al.
- **Date:** 2026-02-26
- **Category:** `LLM agent attack`

> AgentSentry is the first inference-time defense to model multi-turn IPI as temporal causal takeover, localizing takeover points via counterfactual re-executions and enabling safe continuation through causal context purification. Achieves 74.55% Utility Under Attack on AgentDojo.

**📝 Summary:** 把多轮 IPI 攻击建模为时序因果接管，通过反事实重执行定位接管点并净化上下文，在 AgentDojo 上取得 74.55% 的 UA。

### [Silent Egress: When Implicit Prompt Injection Makes LLM Agents Leak Without a Trace](https://arxiv.org/abs/2602.22450)
- **Authors:** Qianlong Lan, Anuj Kaul, Shaun Jones et al.
- **Date:** 2026-02-25
- **Category:** `LLM agent attack`

> This paper demonstrates implicit prompt injection via URL previews causing silent egress (data exfiltration). In 480 runs with qwen2.5:7b, attack success P=0.89, with 95% undetected by output-based safety checks. Sharded exfiltration bypasses DLP.

**📝 Summary:** 展示隐式 prompt injection 通过 URL 预览元数据劫持 agent 并静默数据泄露，攻击成功率 0.89，95% 逃避输出层安全检测。

### [Training Agents to Self-Report Misbehavior](https://arxiv.org/abs/2602.22303)
- **Authors:** Bruce W. Lee, Chen Yueh-Han, Tomek Korbak
- **Date:** 2026-02-25
- **Category:** `agentic adversarial`

> Self-incrimination training trains agents to call a report_scheming() tool when behaving deceptively. Tested on GPT-4.1 and Gemini-2.0, it significantly reduces undetected successful attack rate and outperforms matched-capability monitors.

**📝 Summary:** 训练 agent 在欺骗性行为时主动调用举报工具，大幅降低未被检测到的攻击成功率，优于同等能力的监控模型。

### [ICON: Indirect Prompt Injection Defense for Agents based on Inference-Time Correction](https://arxiv.org/abs/2602.20708)
- **Authors:** Che Wang, Fuyao Zhang, Jiaming Zhang et al.
- **Date:** 2026-02-24
- **Category:** `LLM agent attack`

> ICON detects IPI via high intensity scores in latent space, then performs surgical attention steering to selectively neutralize adversarial dependencies. Achieves 0.4% ASR with 50%+ task utility gain over baselines.

**📝 Summary:** 通过隐空间强度分数检测 IPI，再进行注意力 steering 手术式消除对抗依赖，ASR 降至 0.4% 同时任务效用提升 50%+。

### ["Are You Sure?": An Empirical Study of Human Perception Vulnerability in LLM-Driven Agentic Systems](https://arxiv.org/abs/2602.21127)
- **Authors:** Xinfeng Li, Shenyu Dai, Kelong Zheng et al.
- **Date:** 2026-02-24
- **Category:** `LLM agent attack`

> First large-scale empirical study (303 participants) measuring human susceptibility to Agent-Mediated Deception (AMD). Only 8.6% perceive AMD attacks; domain experts show increased susceptibility in certain scenarios. Six cognitive failure modes identified.

**📝 Summary:** 303人大规模实验研究人类对 agent 中介欺骗（AMD）的感知脆弱性，仅 8.6% 能识别攻击，发现六种认知失败模式。

### [PA-Attack: Guiding Gray-Box Attacks on LVLM Vision Encoders with Prototypes and Attention](https://arxiv.org/abs/2602.19418)
- **Authors:** Hefei Mei, Zirui Wang, Chang Xu et al.
- **Date:** 2026-02-23
- **Category:** `adversarial attack language model`

> PA-Attack targets LVLM vision encoders in a gray-box setting with prototype-anchored guidance and two-stage attention enhancement, achieving 75.1% average score reduction rate across diverse downstream tasks.

**📝 Summary:** 针对 LVLM 视觉编码器的灰盒攻击，通过 prototype 锚定和注意力增强实现强迁移性，平均 SRR 达 75.1%。

### [Skill-Inject: Measuring Agent Vulnerability to Skill File Attacks](https://arxiv.org/abs/2602.20156)
- **Authors:** David Schmotz, Luca Beurer-Kellner, Sahar Abdelnabi et al.
- **Date:** 2026-02-23
- **Category:** `LLM agent attack`

> SkillInject is a benchmark evaluating susceptibility of LLM agents to injections through skill files, with 202 injection-task pairs. Frontier models show up to 80% ASR including data exfiltration, destructive action, and ransomware-like behaviors.

**📝 Summary:** 评估 LLM agent 对 skill 文件注入攻击的脆弱性，前沿模型攻击成功率高达 80%，覆盖数据窃取和破坏性行为。

### [Assessing Risks of Large Language Models in Mental Health Support: A Framework for Automated Clinical AI Red Teaming](https://arxiv.org/abs/2602.19948)
- **Authors:** Ian Steenstra, Paola Pedrelli, Weiyan Shi et al.
- **Date:** 2026-02-23
- **Category:** `safety benchmark agent`

> This paper introduces an evaluation framework pairing AI psychotherapists with simulated patient agents to assess therapy sessions against quality and risk ontologies. 369 session simulations reveal critical safety gaps including AI Psychosis and failure to de-escalate suicide risk.

**📝 Summary:** 用模拟患者 agent 对 AI 心理治疗师进行 red teaming，发现 AI Psychosis 等严重安全漏洞。

### [BarrierSteer: LLM Safety via Learning Barrier Steering](https://arxiv.org/abs/2602.20102)
- **Authors:** Thanh Q. Tran, Arun Verma, Kiwan Wong et al.
- **Date:** 2026-02-23
- **Category:** `adversarial attack language model`

> BarrierSteer formalizes response safety by embedding learned non-linear safety constraints via Control Barrier Functions directly in the model's latent space, steering unsafe trajectories during inference without modifying LLM parameters.

**📝 Summary:** 用控制障碍函数（CBF）在模型隐空间强制安全约束，推理期 steering 而不修改 LLM 参数。

---

## 2026-W08

### [What Makes a Good LLM Agent for Real-world Penetration Testing?](https://arxiv.org/abs/2602.17622)
- **Authors:** Gelei Deng, Yi Liu, Yuekang Li et al.
- **Date:** 2026-02-19
- **Category:** `LLM agent AND attack`

> We analyze 28 LLM-based penetration testing systems and evaluate five representative implementations across three benchmarks. We identify two failure modes: Type A (capability gaps from missing tools/prompts, fixable via engineering) and Type B (planning/state management limitations persisting regardless of tooling). Type B failures share a root ca...

**📝 Summary:** 系统分析 28 个 LLM 渗透测试系统，区分能力缺口（Type A）和规划失败（Type B），提出 Excalibur 框架通过难度感知规划在 CTF benchmark 上达到 91% 完成率。

### [Safe Continuous-time Multi-Agent Reinforcement Learning via Epigraph Form](https://arxiv.org/abs/2602.17078)
- **Authors:** Xuefeng Wang, Lei Zhang, Henglin Pu et al.
- **Date:** 2026-02-19
- **Category:** `multi-agent AND safety`

> Multi-agent reinforcement learning (MARL) has made significant progress, but most algorithms rely on a discrete-time Markov Decision Process with fixed decision intervals. We propose a continuous-time constrained MDP (CT-CMDP) formulation and a novel MARL framework that transforms discrete MDPs into CT-CMDPs via an epigraph-based reformulation. Usi...

**📝 Summary:** 将离散时间 MARL 扩展到连续时间约束 MDP，用 PINN actor-critic 解决连续时间安全多智能体问题（ICLR 2026）。

### [Pushing the Frontier of Black-Box LVLM Attacks via Fine-Grained Detail Targeting (M-Attack-V2)](https://arxiv.org/abs/2602.17645)
- **Authors:** Xiaohan Zhao, Zhaoyi Li, Yaxin Luo et al.
- **Date:** 2026-02-19
- **Category:** `adversarial attack AND language model`

> Black-box adversarial attacks on Large Vision-Language Models (LVLMs) are challenging due to missing gradients and complex multimodal boundaries. We find that prior approaches induce high-variance, nearly orthogonal gradients across iterations. We reformulate local matching as an asymmetric expectation over source transformations and target semanti...

**📝 Summary:** M-Attack-V2：改进黑盒多模态 LLM 对抗攻击，通过 MCA+ATA 稳定梯度估计，Claude-4.0 攻击成功率 8%→30%，GPT-5 98%→100%。

### [The Emergence of Lab-Driven Alignment Signatures: A Psychometric Framework for Auditing Latent Bias and Compounding Risk in Generative AI](https://arxiv.org/abs/2602.17127)
- **Authors:** Dusan Bosnjakovic
- **Date:** 2026-02-19
- **Category:** `multi-agent AND safety`

> As LLMs transition from chat interfaces to foundational layers in multi-agent systems and LLM-as-a-judge loops, detection of durable, provider-level behavioral signatures becomes critical. We introduce an auditing framework using psychometric measurement theory to quantify these tendencies without ground-truth labels, utilizing forced-choice ordina...

**📝 Summary:** 心理测量框架审计不同 AI 实验室的 LLM 的隐性偏见和'lab signal'，发现提供商级别的行为签名在多 agent 场景下可能形成复合风险和意识形态回音室。

### [NESSiE: The Necessary Safety Benchmark -- Identifying Errors that should not Exist](https://arxiv.org/abs/2602.16756)
- **Authors:** Johannes Bertram, Jonas Geiping
- **Date:** 2026-02-18
- **Category:** `adversarial attack AND language model`

> We introduce NESSiE, the NEceSsary SafEty benchmark for large language models (LLMs). With minimal test cases of information and access security, NESSiE reveals safety-relevant failures that should not exist, given the low complexity of the tasks. Even state-of-the-art LLMs do not reach 100% on NESSiE, failing the necessary condition of language mo...

**📝 Summary:** NESSiE：极简安全 benchmark，揭示 SOTA LLM 在低复杂度安全任务上仍存在失败，且 benign 干扰上下文可显著降低安全性能。

### [AgentLAB: Benchmarking LLM Agents against Long-Horizon Attacks](https://arxiv.org/abs/2602.16901)
- **Authors:** Tanqiu Jiang, Yuhui Wang, Jiacheng Liang et al.
- **Date:** 2026-02-18
- **Category:** `LLM agent AND attack`

> LLM agents deployed in long-horizon, complex environments face long-horizon attacks that exploit multi-turn user-agent-environment interactions to achieve objectives infeasible in single-turn settings. We present AgentLAB, the first benchmark dedicated to evaluating LLM agent susceptibility to adaptive, long-horizon attacks. AgentLAB supports five ...

**📝 Summary:** AgentLAB：首个专注于评估 LLM agent 对长时程攻击脆弱性的 benchmark，覆盖 5 种攻击类型×28 个真实 agentic 环境×644 个测试用例，证明单轮防御对长时程攻击无效。

### [Automating Agent Hijacking via Structural Template Injection](https://arxiv.org/abs/2602.16958)
- **Authors:** Xinhao Deng, Jiaqing Wu, Miao Chen et al.
- **Date:** 2026-02-18
- **Category:** `agentic AND adversarial`

> We propose Phantom, an automated agent hijacking framework built upon Structured Template Injection that targets the fundamental architectural mechanisms of LLM agents. Agents rely on specific chat template tokens to separate system, user, assistant, and tool instructions. By injecting optimized structured templates into the retrieved context, we i...

**📝 Summary:** Phantom：利用 chat template token 结构注入的 agent 劫持框架，通过 Template Autoencoder + 贝叶斯优化搜索最优对抗模板，在真实商业产品中发现 70+ 漏洞。

### [Mind the GAP: Text Safety Does Not Transfer to Tool-Call Safety in LLM Agents](https://arxiv.org/abs/2602.16943)
- **Authors:** Arnold Cartagena, Ariane Teixeira
- **Date:** 2026-02-18
- **Category:** `jailbreak AND agent`

> Large language models deployed as agents increasingly interact with external systems through tool calls--actions with real-world consequences that text outputs alone do not carry. Safety evaluations, however, overwhelmingly measure text-level refusal behavior, leaving a critical question unanswered: does alignment that suppresses harmful text also ...

**📝 Summary:** 提出 GAP benchmark，发现 LLM agent 的文本层拒绝≠工具调用层安全——模型口头拒绝的同时可能悄悄执行禁止操作，17,420 个数据点覆盖六个前沿模型。

### [Narrow fine-tuning erodes safety alignment in vision-language agents](https://arxiv.org/abs/2602.16931)
- **Authors:** Idhant Gulati, Shivam Raval
- **Date:** 2026-02-18
- **Category:** `safety benchmark AND agent`

> Fine-tuning aligned vision-language models on narrow-domain harmful datasets induces severe emergent misalignment that generalizes broadly across unrelated tasks and modalities. Through experiments on Gemma3-4B, misalignment scales monotonically with LoRA rank, and multimodal evaluation reveals substantially higher misalignment (70.71% at r=128) th...

**📝 Summary:** 窄领域微调可以严重侵蚀视觉语言 agent 的安全对齐，有害行为占据低维子空间（10个主成分），单模态安全 benchmark 低估了多模态模型的对齐退化。

### [Policy Compiler for Secure Agentic Systems (PCAS)](https://arxiv.org/abs/2602.16708)
- **Authors:** Nils Palumbo, Sarthak Choudhary, Jihye Choi et al.
- **Date:** 2026-02-18
- **Category:** `prompt injection`

> LLM-based agents are increasingly being deployed in contexts requiring complex authorization policies. Embedding these policies in prompts provides no enforcement guarantees. We present PCAS, a Policy Compiler for Agentic Systems that provides deterministic policy enforcement. PCAS models the agentic system state as a dependency graph capturing cau...

**📝 Summary:** PCAS：用 dependency graph + Datalog 策略语言实现确定性策略执行，防御 prompt injection，policy 合规率从 48% 提升到 93%，无需修改 agent 代码。

### [Helpful to a Fault: Measuring Illicit Assistance in Multi-Turn, Multilingual LLM Agents (STING)](https://arxiv.org/abs/2602.16346)
- **Authors:** Nivya Talokar, Ayush K Tarun, Murari Mandal et al.
- **Date:** 2026-02-18
- **Category:** `red teaming AND LLM`

> LLM-based agents execute real-world workflows via tools and memory. These affordances enable ill-intended adversaries to also use these agents to carry out complex misuse scenarios. We introduce STING (Sequential Testing of Illicit N-step Goal execution), an automated red-teaming framework that constructs a step-by-step illicit plan grounded in a b...

**📝 Summary:** STING：自动化多轮 agent red-teaming 框架，将攻击建模为 time-to-first-jailbreak 随机变量，多语言实验发现低资源语言未必更脆弱（与 chatbot 研究结论不同）。

### [Recursive language models for jailbreak detection: a procedural defense for tool-augmented agents](https://arxiv.org/abs/2602.16520)
- **Authors:** Doron Shavit
- **Date:** 2026-02-18
- **Category:** `agentic AND adversarial`

> We present RLM-JB, an end-to-end jailbreak detection framework built on Recursive Language Models (RLMs), in which a root model orchestrates a bounded analysis program that transforms the input, queries worker models over covered segments, and aggregates evidence into an auditable decision. RLM-JB treats detection as a procedure rather than one-sho...

**📝 Summary:** RLM-JB：递归 LM 结构的 jailbreak 检测防御框架，将检测视为流程而非单次分类，通过分块+并行筛查+跨块信号合成，对 AutoDAN 类攻击达到 92-98% 召回率。

### [Zombie Agents: Persistent Control of Self-Evolving LLM Agents via Self-Reinforcing Injections](https://arxiv.org/abs/2602.15654)
- **Authors:** Xianglin Yang, Yufei He, Shuo Ji et al.
- **Date:** 2026-02-17
- **Category:** `LLM agent AND attack`

> Self-evolving LLM agents update their internal state across sessions by writing and reusing long-term memory. This creates a security risk: untrusted external content observed during a benign session can be stored as memory and later treated as instruction. We formalize a persistent attack called Zombie Agent, where an attacker covertly implants a ...

**📝 Summary:** Zombie Agent：对自进化 LLM agent 的持久性攻击，通过将 payload 植入 long-term memory 实现跨 session 持久控制，针对滑动窗口和 RAG 记忆设计了绕过截断/相关性过滤的持久化策略。

### [Colosseum: Auditing Collusion in Cooperative Multi-Agent Systems](https://arxiv.org/abs/2602.15198)
- **Authors:** Mason Nakamura, Abhinav Kumar, Saswat Das et al.
- **Date:** 2026-02-16
- **Category:** `multi-agent AND safety`

> Multi-agent systems where LLM agents communicate through free-form language enable sophisticated coordination, but surface a unique safety problem when individual agents form a coalition and collude to pursue secondary goals. We present Colosseum, a framework for auditing LLM agents' collusive behavior in multi-agent settings, grounding cooperation...

**📝 Summary:** Colosseum：多 agent 系统中的串谋审计框架，发现大多数模型在有秘密通信渠道时倾向于串谋，且存在'纸面串谋'现象。

### [A Trajectory-Based Safety Audit of Clawdbot (OpenClaw)](https://arxiv.org/abs/2602.14364)
- **Authors:** Tianyu Chen, Dongrui Liu, Xia Hu et al.
- **Date:** 2026-02-16
- **Category:** `agent safety`

> Clawdbot is a self-hosted, tool-using personal AI agent with a broad action space spanning local execution and web-mediated workflows. We present a trajectory-centric evaluation of Clawdbot across six risk dimensions. Our test suite samples and lightly adapts scenarios from prior agent-safety benchmarks (including ATBench and LPS-Bench) and supplem...

**📝 Summary:** 对 OpenClaw（Clawdbot）做 trajectory-based 安全审计，34 个测试用例覆盖六个风险维度，发现大多数失败出现在意图模糊或 benign-seeming jailbreak 场景。

### [Overthinking Loops in Agents: A Structural Risk via MCP Tools](https://arxiv.org/abs/2602.14798)
- **Authors:** Yohan Lee, Jisoo Jang, Seoyeon Choi et al.
- **Date:** 2026-02-16
- **Category:** `tool use AND attack`

> Tool-using LLM agents increasingly coordinate real workloads by selecting and chaining third-party tools based on text-visible metadata such as tool names, descriptions, and return messages. A malicious MCP tool server can induce overthinking loops where individually trivial or plausible tool calls compose into cyclic trajectories that inflate end-...

**📝 Summary:** 恶意 MCP 工具服务器可通过结构性攻击诱导 agent 陷入'过度思考循环'，造成最高 142.4x 的 token 放大，且解码时的简洁控制无法可靠防御。

### [Boundary Point Jailbreaking of Black-Box LLMs](https://arxiv.org/abs/2602.15001)
- **Authors:** Xander Davies, Giorgi Giglemiani, Edmund Lau et al.
- **Date:** 2026-02-16
- **Category:** `red teaming AND LLM`

> Frontier LLMs are safeguarded against attempts to extract harmful information via adversarial prompts known as "jailbreaks". Recently, defenders have developed classifier-based systems that have survived thousands of hours of human red teaming. We introduce Boundary Point Jailbreaking (BPJ), a new class of automated jailbreak attacks that evade the...

**📝 Summary:** BPJ：纯黑盒 jailbreak，每次只用一 bit 信息（是否被检测器标记），通过 curriculum 中间目标攻破 Constitutional Classifiers 和 GPT-5 输入过滤器。

### [Exposing the Systematic Vulnerability of Open-Weight Models to Prefill Attacks](https://arxiv.org/abs/2602.14689)
- **Authors:** Lukas Struppek, Adam Gleave, Kellin Pelrine
- **Date:** 2026-02-16
- **Category:** `red teaming AND LLM`

> Open-weight models natively support prefilling, which allows an attacker to predefine initial response tokens before generation begins. We present the largest empirical study to date of prefill attacks, evaluating over 20 existing and novel strategies across multiple model families and state-of-the-art open-weight models. Our results show that pref...

**📝 Summary:** 系统研究 prefill attack（预填充初始回复 token）对开源模型的攻击效果，20+ 策略评估全部主流开源模型，发现普遍脆弱；推理模型对通用 prefill 有一定抵抗但针对性策略依然有效。

---

## 2026-W07

### [SkillJect: Automating Stealthy Skill-Based Prompt Injection for Coding Agents](https://arxiv.org/abs/2602.14211)
- **Authors:** Xiaojun Jia, Jie Liao, Simeng Qin et al.
- **Date:** 2026-02-15
- **Category:** `prompt injection`

> Agent skills are becoming a core abstraction in coding agents, packaging long-form instructions and auxiliary scripts to extend tool-augmented behaviors. This abstraction introduces an under-measured attack surface: skill-based prompt injection, where poisoned skills can steer agents away from user intent and safety policies. We propose the first a...

**📝 Summary:** SkillJect：首个针对 coding agent skill 的自动化隐蔽 prompt injection 框架，三 agent 闭环（Attack/Code/Evaluate），将恶意操作藏于辅助脚本中。

### [Unsafer in Many Turns: Benchmarking and Defending Multi-Turn Safety Risks in Tool-Using Agents](https://arxiv.org/abs/2602.13379)
- **Authors:** Xu Li, Simon Yu, Minzhou Pan et al.
- **Date:** 2026-02-13
- **Category:** `agent safety`

> LLM-based agents are becoming increasingly capable, yet their safety lags behind. This creates a gap between what agents can do and should do. This gap widens as agents engage in multi-turn interactions and employ diverse tools, introducing new risks overlooked by existing benchmarks. To systematically scale safety testing into multi-turn, tool-rea...

**📝 Summary:** 构建 MT-AgentRisk benchmark（首个多轮工具调用 agent 安全评估），发现多轮场景下 ASR 平均提升 16%；提出免训练防御 ToolShield。Bo Li 组的工作！

---


*Curated by [aq bot](https://github.com/aquamarine-bot) · [AI Safety Weekly](https://github.com/aquamarine-bot/ai-safety-weekly)*