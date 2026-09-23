# Jingbo Chai · 柴靖博

**AI Agent / RAG 开发者 · Open-source AI tools**

我开发 AI 研究工具、带证据的报告生成应用和本地效率软件，并公开它们的实现与评测。  
I build AI research tools, evidence-linked reporting workflows and local-first software.

悉尼大学计算机硕士 · Master of Computer Science @ The University of Sydney · **2027 届**

邮箱：`shuxiachai@163.com` · 微信：`SHUXIA_chai`

<a name="selected-projects"></a>
## 精选作品 / Selected projects

### ACA · 论文商业化评估助手

**从研究主题或论文，生成带来源的商业化评估报告草稿。**  
Turn a research topic or paper into a cited commercialization report and scorecard.

<img src="https://raw.githubusercontent.com/shuxiachai/academic-commercialization-agent/9e0116d496c9bdf866bc0d914cac2763d92ad244/assets/screenshot-results.png" alt="Academic Commercialization Agent 历史版本的报告与评分界面" width="800">

*历史版本界面与报告样例，用于展示产品流程。*

面向研究初筛：查看证据与可靠性提示，导出报告，并在任务中断后恢复执行。报告草稿仍需人工核查。

**[查看报告样例（历史版本）](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/examples/car-t-solid-tumors/commercialization_report.md) · [进入在线应用（需访问码或自备密钥）](https://academic-commercialization-agent.up.railway.app) · [查看源码](https://github.com/shuxiachai/academic-commercialization-agent)**

### BushfireReadyGPT · 山火准备报告助手

**把澳洲地区与准备场景，整理成有证据、可审核的山火准备报告草稿。**  
A local-first bushfire preparedness workflow with hybrid RAG and human review.

<img src="https://raw.githubusercontent.com/shuxiachai/BushfireReadyGPT/f3228799be3808c99d0f14cb5c9904aea5e076d9/docs/assets/create-report.png" alt="BushfireReadyGPT 历史版本的本地报告创建界面" width="640">

*本地流程截图与演示视频，不代表当前云端版本的完整验收。*

可查看资料与限制、审核草稿并导出文件。基于已注明来源的上游项目改造，用于作品展示与受控讨论，不用于实时火情、撤离或生命安全决策。

**[下载演示视频（89 秒 MP4）](https://raw.githubusercontent.com/shuxiachai/BushfireReadyGPT/25cdbab5bed51b410ede5f410a8aa70e2cdcfe72/docs/assets/bushfire-ready-gpt-demo.mp4) · [查看报告样例（v0.6.0）](https://github.com/shuxiachai/BushfireReadyGPT/blob/v0.6.0/examples/v0.6.0/cairns-council-report.md) · [查看源码](https://github.com/shuxiachai/BushfireReadyGPT)**

### 地脉簿 LeyLineBook · 多账号任务管理工具

**在电脑和手机上管理多个《原神》账号的日常与周期任务。**  
A local-first task manager with Windows desktop and offline PWA clients.

<img src="https://raw.githubusercontent.com/shuxiachai/LeyLineBook/bf6f5c28f52803f50746ada007f09059666295cf/docs/images/multi-account-desktop.png" alt="地脉簿多账号任务总览，展示三个合成演示账号的待办与完成情况" width="720">

*真实界面，使用合成演示账号与记录。*

集中查看任务、记录完成情况，并通过备份在两端迁移数据。两端各自保存数据；工具不会连接或操作游戏本体。

**[打开网页版（PWA）](https://shuxiachai.github.io/LeyLineBook/) · [下载 Windows 版](https://github.com/shuxiachai/LeyLineBook/releases/latest) · [查看源码与使用说明](https://github.com/shuxiachai/LeyLineBook)**

<details>
<summary><strong>工程实现与评测 / Engineering details</strong></summary>

- **ACA — Agent workflows & runtime reliability:** deterministic retrieval freezes evidence before six LLM stages. Structured contracts, checkpoints and redacted tracing make failures inspectable. Recovery passed **30/30 offline fault-injection cases**, within the published protocol and limits. [Recovery evidence](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/docs/results-2026-08-23-checkpoint-fault-recovery.md) · [Engineering case study](https://github.com/shuxiachai/academic-commercialization-agent/blob/main/docs/portfolio-case-study.md).
- **Bushfire — Hybrid RAG & governed generation:** combines deterministic analysis, retrieval, model generation and human review. The historical **v0.6.0** structured-planning benchmark reports **MRR 0.922** over **68 answerable queries and 5 safety negatives**. Retrieval performance and report quality are evaluated separately. [Retrieval evaluation](https://github.com/shuxiachai/BushfireReadyGPT/blob/main/docs/benchmarks/rag-retrieval-v0.6.0.json) · [Upstream and attribution](https://github.com/shuxiachai/BushfireReadyGPT/blob/main/UPSTREAM.md).
- **LeyLineBook — Product delivery & data reliability:** backup migration, data validation, platform-specific credential boundaries, automated tests, Windows packaging and PWA deployment. [CI](https://github.com/shuxiachai/LeyLineBook/actions/workflows/ci.yml).

**Tools:** Python · FastAPI · Pydantic · SQL/SQLite · JavaScript · Docker · GitHub Actions · OpenTelemetry.

</details>

## 交流与机会 / Opportunities

关注这里的 Agent 可靠性、RAG 评测与开源工具实践；使用问题与改进建议欢迎提交到对应项目的 Issues。

面向 **2027 届 AI Agent、LLM 应用、Agent 平台与 AI 后端工程岗位**。  
Open to 2027 new-grad opportunities in AI Agent, LLM Application, Agent Platform and AI Backend engineering.

