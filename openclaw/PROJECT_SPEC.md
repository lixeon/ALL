# 项目介绍

## 1. 项目目的
Academic Lobster Lab 的目标是为 OpenClaw 配置一套“真实顶级学术团队”风格的 multi-agent 体系：
- 领导提出/筛选 idea
- 杰出学者统筹科研主线
- senior 主导主要科研任务并对质量负责
- junior 执行实验/复现/数据整理并保留证据链
- peer reviewers 以外部顶尖评审视角反复 reject/major/minor/accept
- reproducibility chair 独立审计证据链与可复现性，必要时阻断 release


## 2. 系统构成
### 2.1 9-agent 学术团队（核心）
- academy-lead
- distinguished-scholar
- senior-researcher-1
- senior-researcher-2
- junior-researcher-1
- junior-researcher-2
- peer-reviewer-1
- peer-reviewer-2
- reproducibility-chair

### 2.2 论文产出扩展
- paper-writer：论文主笔与版本迭代协调
- latex-editor：LaTeX 格式、编译、可提交产出

### 2.3 文献知识库
- 保存原始 PDF（真实性）
- OCR 输出 md/latex（可检索、可引用、可改稿）
- provenance（来源、时间、hash、状态）
- BibTeX（引用一致性）

## 3. 核心逻辑（从 idea 到 release）
1) idea_proposed（academy-lead）
2) program_defined（distinguished-scholar）
3) major_tasks_assigned（distinguished-scholar + seniors）
4) execution_in_progress（seniors + juniors）
5) internal_synthesis_ready（distinguished-scholar）
6) peer_review_round（peer reviewers）
7) revision_round（seniors + distinguished-scholar + paper-writer）
8) reproducibility_audit（reproducibility-chair）
9) release_ready（academy-lead + reproducibility-chair）

## 4. 核心工作流
### 4.1 论文迭代（Reject → Revision → Resubmit）
见：`templates/paper_iteration/paper_iteration_workflow.md`
以及 demo：`dossiers/examples/demo_paper_cycle/`

### 4.2 文献入库与治理
见：`knowledge_base/workflows/literature_intake_workflow.md`

## 5. 交付物与使用方式
- 角色行为：`agents/<role>/{SOUL,AGENTS,ROLE_CONTRACT,...}.md`
- 治理与模板：`templates/`
- 配置与约定：`config/`
- 证据包/示例：`dossiers/`
- 文献知识库：`knowledge_base/`
