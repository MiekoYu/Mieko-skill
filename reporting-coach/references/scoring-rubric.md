# 汇报表现量化评价规则

## Dimensions

| 维度 | 满分 | Definition | Top standard |
|---|---:|---|---|
| 结构清晰度 | 20 | 信息层级分明，读者可快速定位关键信息 | 概览 5 秒内传递全貌，正文分层无遗漏 |
| 数据量化度 | 20 | 关键结论有数字支撑，数字带基准线与变化方向 | 每个数字都可独立判断好坏，数据三要素齐全 |
| 问题坦诚度 | 20 | 失败/延期/阻塞不遮掩，有根因分析与下一步 | S-B-N 结构完整，问题分级准确，主动暴露 |
| 决策辅助力 | 20 | 汇报推动决策，不只是传递信息 | 上级读完可判断行动方向，无需追问 |
| 预期管理力 | 10 | 偏差伴有原因与新节点，风险有概率判断 | 不让上级突然收到坏消息 |
| 表达专业度 | 10 | 语言凝练、动词精准、语气得体 | A 级动词占比高，无模糊语，称呼/格式规范 |

Total: 100.

在项目或技术管理汇报场景中，评分必须反映文本是否支持决策，而不只评价是否通顺。

## Grades

| Grade | Score | Meaning |
|---|---:|---|
| S 卓越 | 90-100 | 可直接作为汇报范本 |
| A 优秀 | 80-89 | 显著高于平均水平，偶有小瑕疵 |
| B 良好 | 70-79 | 整体合格，有可识别提升空间 |
| C 待改进 | 60-69 | 基本完成汇报职能，但短板明显 |
| D 不合格 | <60 | 严重信息缺失或误导风险 |

## Scoring Guidance

### 结构清晰度 / 20

Score high when:
- opening overview gives core output, deviation, and next focus
- sections are stable and easy to scan
- tables have clear fields and no mixed logic
- 长篇管理汇报清楚区分计划、达成情况、输出成果、异常与问题、改善对策、所需支持

Deduct for:
- no overview
- achievements, risks, and plans mixed together
- reader must infer the main point
- missing denominator or unclear grouping labels
- no explicit current status for key projects

### 数据量化度 / 20

Score high when:
- data includes absolute value, baseline, and direction/range
- units are kept
- progress uses X/Y, percentage, or milestone chain with context
- comparisons specify target, previous period, competitor, or current plan

Deduct for:
- naked numbers without baseline
- percentages without denominator
- qualitative claims like "明显提升" without evidence
- missing units

### 问题坦诚度 / 20

Score high when:
- failures, delays, and blockages are stated directly
- S-B-N is complete
- root cause and next action are present
- impact is described
- issue reports include problem, impact, current judgment, action, expected date, and needed support when available

Deduct for:
- only saying "进行中/待确认"
- explaining a problem without next action
- hiding or softening failure
- blaming external parties without internal action
- reporting delay/failure without a new node or impact assessment

### 决策辅助力 / 20

Score high when:
- each key conclusion points to recommended action
- main/backup/pause choices are explicit
- support or decision needed from the manager is clear
- technical facts connect to product, cost, schedule, or business value
- the report answers: status, judgment, evidence, next node, and what the manager needs to confirm/coordinate/decide

Deduct for:
- only reporting status
- no recommendation after comparison
- no support request when support is clearly needed
- too much execution detail without "so what"
- multiple suppliers/options listed without 主选、备选、暂缓/放弃, unless the text clearly says evidence is insufficient

### 预期管理力 / 10

Score high when:
- dates are concrete
- deviations have reason and new date
- risks include probability and impact
- future milestones are stated

Deduct for:
- "预计/有望" without confidence or risk
- no new node after delay
- risk appears only after it becomes a problem

### 表达专业度 / 10

Score high when:
- concise verb-object sentences dominate
- A-level verbs are used for real outputs
- tone is direct and non-performative
- format is consistent

Deduct for:
- AI-sounding phrases
- vague verbs and filler
- over-compression that removes necessary facts
- inconsistent naming, date format, or status labels

## 管理汇报评分上限

Apply these caps after dimension scoring:

| Condition | Maximum score |
|---|---:|
| No current status/judgment for the main item | 79 |
| Has issues/delay but no reason and no next action | 74 |
| Lists options or collaboration paths but gives no recommendation and no reason for not ranking | 78 |
| Contains quantitative claims with missing units or no baseline throughout | 82 |
| Cannot support a management decision after reading once | 76 |
| Fabricates or overstates conclusions beyond supplied facts | 69 |

Use the cap only when it is lower than the raw score, and explain the cap in the扣分点 or short note.

## Output Requirements

Use this structure unless the user asks otherwise:

```text
评分总览：XX / 100（X 级）

| 维度 | 得分 | 满分 | 核心依据 | 主要扣分点 |
|---|---:|---:|---|---|

主要优点：
1. ...

主要短板：
1. ...

优先修改建议：
1. ...

如触发封顶规则：
封顶说明：...
```

If the supplied text is too short to score reliably, say so, provide a provisional score range, and list the missing information needed for a firm score.
