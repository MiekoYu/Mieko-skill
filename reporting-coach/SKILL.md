---
name: reporting-coach
description: Optimize, rewrite, review, or score Chinese work reports, including weekly and monthly updates, status notes, risk notes, collaboration summaries, and decision requests. 优化、审查或评分中文工作汇报；适用于周报、月报、进展说明、风险说明、协作总结和决策请求。
---

# 汇报教练

## Core Use

Use this skill for two tasks. The default role setting is: the user is a project or technical contributor reporting upward to a direct manager. Prioritize management judgment, clear facts, and decision support.

1. **Expression optimization**: Rewrite the user's report wording into a conclusion-first, status-clear, result-oriented, decision-supporting Chinese work-report style. If key facts are missing, ask for the minimum necessary additions instead of inventing them.
2. **Quantitative scoring**: When the user mentions scoring or evaluation, score the report using the six-dimension rubric in `references/scoring-rubric.md`.

For detailed style rules, read `references/expression-guidelines.md` before rewriting. For scoring, read both reference files.

For a decision-oriented report, use this structure when it fits the supplied content: current judgment, key output, evidence, risk/issue, next action, and support or decision needed.

## Expression Optimization Workflow

1. Identify the scenario: weekly report, monthly report, meeting follow-up, status update, risk report, collaboration summary, or decision request. Default audience: the user's direct manager.
2. Extract only known facts: task, result, status, data, baseline, date, risk, reason, next action, requested support.
3. Determine management status from the facts: 正常 / 有风险 / 已延期 / 暂缓 / 待判断.
4. Convert actions into outputs or judgments: formed conclusion, passed review, selected plan, excluded route, identified risk, or confirmed next verification.
5. If missing information affects accuracy or decision value, ask concise questions. Common missing items:
   - current status or completion ratio
   - baseline, target, previous value, or comparison object for numbers
   - reason for delay/failure/blockage
   - next action and expected date
   - what decision/support is needed from the manager
6. Rewrite with judgment first, then basis, then next action/support.
7. Keep the wording directly usable. Avoid AI-sounding phrases and avoid the user's banned phrases when possible.

## Default Rewrite Shape

For a single sentence or short paragraph, return:

```text
优化后：
[可直接发送的表达]

需要补充/确认：
1. [only if needed]
```

For a weekly/monthly report section, use:

```text
一、核心结论
1. ...

二、项目状态
| 事项 | 当前判断 | 依据/数据 | 风险/问题 | 下一步 | 需支持 |
|---|---|---|---|---|---|

三、需确认事项
1. ...
```

For a full management report, prefer this six-part structure:

```text
一、计划
二、达成情况
三、输出成果
四、异常与问题
五、改善对策
六、所需支持
```

For a single project, use this compact structure:

```text
当前判断：正常 / 有风险 / 已延期 / 暂缓 / 待判断。
主要依据：...
本周期输出：...
风险/问题：...
下一步：...，预计 ... 形成结论。
需支持/决策：...
```

## Rewrite Rules

- Start with the conclusion or status judgment: 已完成 / 有风险 / 延期 / 暂缓 / 未通过 / 主选 / 备选.
- Prefer verb-object structures: 完成、输出、选定、确认、发布、签署、验收、关闭.
- Convert process-only wording into result wording when facts support it.
- Keep units, dates, quantities, percentages, and comparison baselines.
- Do not invent data. Use `待确认 / 需核实 / 未见` for missing facts.
- For numbers, require at least two of: absolute value, baseline, change direction/range.
- For delay/failure/blockage, include: situation, reason/root cause, next action, new date, impact, support needed.
- For risk, include event, probability level, impact level, and mitigation if known.
- Make the manager's decision point explicit when the report implies a choice.
- When multiple options, suppliers, or tasks exist, state 主选 / 备选 / 暂缓 / 放弃 / 优先推进. If the evidence is insufficient, write `暂不具备排序依据`.
- If there is no issue or no support request, say `当前无新增异常` or `当前无需额外支持` instead of inventing one.

## Scoring Workflow

Trigger scoring when the user says 打分, 评分, 量化评价, 评价一下, 按标准评估, or similar.

1. Read `references/scoring-rubric.md`.
2. Score each dimension with evidence from the user's text.
3. Do not give high scores for unsupported claims or vague progress.
4. Separate facts from inferred judgment.
5. Check whether the text can support a management decision: status, output, basis, risk, next node, and support/decision needed.
6. Provide a concise improvement list tied to lost points.

Default scoring output:

```text
评分总览：XX / 100（等级）

| 维度 | 得分 | 满分 | 依据 | 扣分点 |
|---|---:|---:|---|---|

主要优点：
1. ...

主要短板：
1. ...

优先修改建议：
1. ...
```

## Quality Bar

The final answer should help the user send, paste, or evaluate the report immediately. Keep explanations short; put the polished wording or score table first.
