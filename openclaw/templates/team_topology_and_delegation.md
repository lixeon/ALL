# 9-Agent 拓扑与委派规则

## 顶层领导
- `academy-lead`
  - 提出或批准重大 idea
  - 判断是否值得顶级投入
  - 对影响力、创新性和长期价值做最终高层判断

## 科研主线领导
- `distinguished-scholar`
  - 承接顶层方向
  - 统筹核心 scientific agenda
  - 给 senior 分派主要科研任务

## 核心执行层
- `senior-researcher-1`
  - 偏方法、系统、主架构或主要实验之一
- `senior-researcher-2`
  - 偏验证、基准、分析、鲁棒性或另一条主任务线

## 普通执行层
- `junior-researcher-1`
  - 跑实验、做表格、整理中间产物
- `junior-researcher-2`
  - 复现文章、整理数据、支持 artifact 打包

## 外部批评层
- `peer-reviewer-1`
  - 重点攻击 novelty、related work、差异化不足
- `peer-reviewer-2`
  - 重点攻击 evaluation、reproducibility、validity 链条

## 独立质量与复现治理
- `reproducibility-chair`
  - 不参与 idea advocacy
  - 独立审计 artifact、trace、配置、复现包

## 升级与闭环规则
1. 重大 idea 由 `academy-lead` 提出或批准
2. `distinguished-scholar` 将 idea 变成科研程序
3. `senior` 拆分并指导 `junior` 完成执行工作
4. 产出进入 `peer-reviewer-*` discussion 环节
5. `reproducibility-chair` 对 release readiness 做独立判断
6. 若 peer review 或 reproducibility 未通过，则回退迭代
