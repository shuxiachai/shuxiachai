# Jingbo Chai · 柴靖博

**AI Agent / RAG 工程实践 · Open-source AI tools**

我开发有来源、可复核的 AI 研究工具，也开发本地优先的实用软件。这里展示我的项目、真实评测与工程实现。  
I build AI tools with traceable evidence, explicit evaluation and recoverable workflows.

悉尼大学计算机硕士 · Master of Computer Science @ The University of Sydney · **2027 届**

**[看论文报告样例](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/examples/car-t-solid-tumors/commercialization_report.md) · [看 Bushfire 89 秒演示](https://github.com/shuxiachai/BushfireReadyGPT/blob/f3228799be3808c99d0f14cb5c9904aea5e076d9/docs/assets/bushfire-ready-gpt-demo.webm) · [打开在线任务管理工具](https://shuxiachai.github.io/LeyLineBook/) · [联系我](mailto:shuxiachai@163.com)**

报告样例与下方截图来自已公开的历史版本；它们展示产品流程，不代表当前版本的完整验收。

## 精选作品 / Selected projects

### [Academic Commercialization Agent](https://github.com/shuxiachai/academic-commercialization-agent)

**从研究主题或论文，生成带来源的商业化评估报告草稿。**  
Turn a research topic or paper into a cited commercialization report and scorecard.

<a href="https://github.com/shuxiachai/academic-commercialization-agent/blob/main/examples/car-t-solid-tumors/commercialization_report.md">
  <img src="https://raw.githubusercontent.com/shuxiachai/academic-commercialization-agent/9e0116d496c9bdf866bc0d914cac2763d92ad244/assets/screenshot-results.png" alt="Academic Commercialization Agent 历史版本的报告与评分界面" width="800">
</a>

面向研究初筛：查看证据与可靠性提示，导出报告，并在任务中断后恢复执行。报告草稿仍需人工核查。

**[直接看报告（历史样例）](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/examples/car-t-solid-tumors/commercialization_report.md) · [在线应用（访问码或 BYOK）](https://academic-commercialization-agent.up.railway.app) · [项目代码](https://github.com/shuxiachai/academic-commercialization-agent) · [工程案例](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/docs/portfolio-case-study.md)**

### [BushfireReadyGPT](https://github.com/shuxiachai/BushfireReadyGPT)

**把澳洲地区与准备场景，整理成有证据、可审核的山火准备报告草稿。**  
A local-first bushfire preparedness workflow with hybrid RAG and human review.

<a href="https://github.com/shuxiachai/BushfireReadyGPT/blob/f3228799be3808c99d0f14cb5c9904aea5e076d9/docs/assets/bushfire-ready-gpt-demo.webm">
  <img src="https://raw.githubusercontent.com/shuxiachai/BushfireReadyGPT/f3228799be3808c99d0f14cb5c9904aea5e076d9/docs/assets/create-report.png" alt="BushfireReadyGPT 历史版本的报告创建界面，点击观看 89 秒本地演示" width="640">
</a>

可查看资料与限制、审核草稿并导出文件。基于已注明来源的上游项目改造，用于作品展示与受控讨论，不用于实时火情、撤离或生命安全决策。

**[89 秒演示](https://github.com/shuxiachai/BushfireReadyGPT/blob/f3228799be3808c99d0f14cb5c9904aea5e076d9/docs/assets/bushfire-ready-gpt-demo.webm) · [报告样例（v0.6.0）](https://github.com/shuxiachai/BushfireReadyGPT/blob/main/examples/v0.6.0/cairns-council-report.md) · [项目代码](https://github.com/shuxiachai/BushfireReadyGPT) · [上游与贡献说明](https://github.com/shuxiachai/BushfireReadyGPT/blob/main/UPSTREAM.md)**

### [LeyLineBook / 地脉簿](https://github.com/shuxiachai/LeyLineBook)

**在电脑和手机上管理多个《原神》账号的日常与周期任务。**  
A local-first task manager with Windows desktop and offline PWA clients.

集中查看任务、记录完成情况，并通过备份在两端迁移数据。两端各自保存数据；工具不会连接或操作游戏本体。

**[立即打开 PWA](https://shuxiachai.github.io/LeyLineBook/) · [下载 Windows 版](https://github.com/shuxiachai/LeyLineBook/releases/latest) · [项目代码与使用说明](https://github.com/shuxiachai/LeyLineBook)**

<details>
<summary><strong>工程实现与评测 / Engineering details</strong></summary>

- **ACA — Agent workflows & runtime reliability:** deterministic retrieval freezes evidence before six LLM stages. Structured contracts, checkpoints and redacted tracing make failures inspectable. Recovery passed **30/30 offline fault-injection cases**, within the published protocol and limits. [Recovery evidence](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/docs/results-2026-08-23-checkpoint-fault-recovery.md).
- **Bushfire — Hybrid RAG & governed generation:** combines deterministic analysis, retrieval, model generation and human review. The historical **v0.6.0** structured-planning benchmark reports **MRR 0.922** over **68 answerable queries and 5 safety negatives**. Retrieval performance and report quality are evaluated separately. [Retrieval evaluation](https://github.com/shuxiachai/BushfireReadyGPT/blob/main/docs/benchmarks/rag-retrieval-v0.6.0.json).
- **LeyLineBook — Product delivery & data reliability:** backup migration, data validation, platform-specific credential boundaries, automated tests, Windows packaging and PWA deployment. [CI](https://github.com/shuxiachai/LeyLineBook/actions/workflows/ci.yml).

**Tools:** Python · FastAPI · Pydantic · SQL/SQLite · JavaScript · Docker · GitHub Actions · OpenTelemetry.

</details>

## 交流与机会 / Get in touch

关注这里的 Agent 可靠性、RAG 评测与开源工具实践；使用问题与改进建议欢迎提交到对应项目的 Issues。

面向 **2027 届 AI Agent、LLM 应用、Agent 平台与 AI 后端工程岗位**。  
Open to 2027 new-grad opportunities in AI Agent, LLM Application, Agent Platform and AI Backend engineering.

[shuxiachai@163.com](mailto:shuxiachai@163.com)
