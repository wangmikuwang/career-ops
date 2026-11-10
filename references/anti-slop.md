# Anti-Slop Reference

AI tell removal adapted for career materials. This file defines what makes writing detectable as AI-generated and how to fix it. Every output from this skill must pass the checks below before delivery.

## Required Inputs

Before running a quality check, have the draft text ready and know:
- What type of document it is (resume, cover letter, LinkedIn, message)
- Who the audience is (recruiter, hiring manager, connection)
- Whether the user is an ESL speaker (affects formality calibration)

---

## Why This Matters

| Finding | Tier |
|---------|------|
| 67% of hiring managers claim they can identify AI content | T2 |
| 33.5% claim detection within 20 seconds | T2 |
| 54% view unedited AI use negatively | T2 |
| 52% accept AI for proofreading/drafting if the final product is authentic | T2 |
| 20% consider AI use a red flag for immediate rejection | T2 |
| 80% of orgs using AI hiring tools don't reject without human review | T2 |

The line is clear: AI-assisted is acceptable. AI-obvious is not.

---

## The Familiarity Problem

AI selects high-probability token sequences. When thousands of applicants use AI, their materials converge on the same phrasing — creating "machine handwriting" that hiring managers recognize across hundreds of applications [T2].

The fix is not better prompting. It's injecting specificity that AI would never generate on its own: real project names, actual metrics, granular details from the user's experience.

---

## Generic Specificity

The most dangerous AI pattern. Text that is structurally correct and looks specific but contains no verifiable detail [T2].

| Generic Specific (bad) | Actually Specific (good) |
|------------------------|--------------------------|
| "Streamlined operational processes" | "Cut weekly inventory count from 6 hours to 90 minutes by switching to cycle counting" |
| "Led cross-functional team to improve outcomes" | "Ran the kitchen remodel with 3 contractors while keeping lunch service running — zero missed days" |
| "Leveraged data-driven insights to optimize performance" | "Built a Google Sheet that tracked peak hours; shifted one closer's shift 2 hours later, which dropped overtime 40%" |

The test: could a stranger verify this claim with a phone call? If not, it's generic specific.

---

## Banned Phrase List (Career Context)

These phrases appear in the majority of AI-generated career materials [T2, 30+ hiring manager interviews]:

### Resume and Cover Letter
- "Results-driven professional with a proven track record"
- "Spearheaded cross-functional initiatives"
- "Leveraging data-driven insights"
- "Passionate about delivering innovative solutions"
- "Dynamic leader with a demonstrated history of"
- "Self-motivated team player"
- "Detail-oriented professional"
- "Extensive experience in"

### LinkedIn
- "I help [audience] achieve [outcome] through [method]"
- "Thought leader in [industry]"
- "Driving innovation and transformation"

### Structural Tells
- Uniformly polished bullets with identical length
- Every bullet follows "Increased [metric] by [percentage] through [strategy]"
- "Corporate bland" tone with zero personality
- Throat-clearing openers ("In today's competitive landscape...")
- Excessive em dashes and semicolons in casual contexts

---

## The One Short Story Principle

The single most effective anti-slop technique [T2].

Every cover letter, every LinkedIn About section, every interview answer should contain at least one short story with a detail so specific that only the person who lived it could write it.

"I reorganized the stockroom" → slop.
"I reorganized the stockroom after a customer asked for a product I knew we had but couldn't find for 10 minutes while they waited. That week I color-coded the back wall by category and put the fast-movers at eye level." → passes.

The story doesn't need to be dramatic. It needs to be *theirs*.

---

## AI Detection Tools: Know the Limits

| Tool | False positive rate | Notes | Tier |
|------|-------------------|-------|------|
| Turnitin | 1-2% (higher for short texts) | Best for long-form | T1 |
| Originality.ai | 0.5-1.5% claimed; 68% detection on "humanized" text | Bypassed by rewriting | T1 |
| GPTZero | Up to 15% false positive | Flags formal/professional writing | T1 |
| Copyleaks | High on long-form, drops on <350 words | Cover letters = problem zone | T2 |

**ESL Warning**: Stanford research confirms AI detectors disproportionately flag ESL writers [T1]. The skill must not over-formalize text for non-native speakers — this increases false positive risk while simultaneously removing the authentic voice that makes writing pass human review.

---

## 中文套话表

The lists above are English. For Chinese materials, these are the equivalents: words that say nothing a reader can check, and that every AI-written Chinese resume shares.

### 空话动词与名词
赋能、抓手、闭环、沉淀、打通、拉通、对齐、颗粒度、组合拳、方法论、底层逻辑、顶层设计、链路、心智、生态、矩阵、势能、深耕、聚焦、助力、驱动、夯实、全方位、多维度、端到端、从 0 到 1（没有说明 0 是什么、1 是什么时）

### 自我评价
具有较强的沟通能力 / 学习能力 / 抗压能力、责任心强、吃苦耐劳、团队合作精神、对数据敏感、有 owner 意识、自驱力强、热爱互联网行业

### 句式
- "负责……，推动……，实现……" 三段式连用，每条 bullet 都一样长
- "通过……，使……提升了 X%" 全篇同构
- "在……的背景下" / "随着……的发展" 开头
- "不仅……更……"、"既……又……" 这类对仗
- 打招呼语里的 "您好，我对贵公司的××岗位非常感兴趣"

替换方法和英文一样：换成做了什么、对谁、用什么、数字从多少到多少。"负责用户增长，通过精细化运营实现 DAU 提升" 是空的；"把新用户次日推送从统一文案改成按注册渠道分 4 版，次留从 31% 到 36%（两周 A/B，各 2 万人）" 才能被核实。例子里的数字只是示范格式，实际数字只能来自用户。

---

## Checks

No numeric self-score. A writer grading its own draft passes every time, so the old 35/50 rubric measured nothing. Run these as pass/fail and fix every failure before delivering.

### 1. Phone-call test
For each achievement: could a stranger verify it with one phone call? "Improved efficiency" fails. "Reduced shrinkage from 2.1% to 0.8% in Q3" passes. If it fails, ask the user for the real detail. If they have none, leave the line plain or cut it. Never invent the detail.

### 2. Swap test
Swap in another company's or person's name. If the text still works, it fails.

### 3. Banned phrases
None from the English lists or the 中文套话表 above.

### 4. Deletion test
Delete each sentence in turn. Any the reader would not miss is filler; remove it.

### 5. Sameness
Bullets must not all share one length or one skeleton. The opening line states the point, not a windup.

### 6. Their words
Where the user described something in their own words, the draft keeps their vocabulary. Don't upgrade "搭了个表" to "构建数据看板体系".

---

## Quality Checklist by Document Type

### Resume
- [ ] No banned phrases in summary or bullet points
- [ ] At least one verifiable detail per role
- [ ] Bullet lengths vary (not all 1-line or all 2-line)
- [ ] Summary reads like a person, not a template

### Cover Letter
- [ ] Opens with a specific connection to the company or role
- [ ] Contains at least one short story
- [ ] No "I am writing to express my interest"
- [ ] Under 350 words (AI detectors struggle with short texts — keep it tight)

### LinkedIn Profile
- [ ] Headline uses natural language, not keyword spam
- [ ] About section front-loads a specific claim or story
- [ ] No "I help X achieve Y through Z" formula
- [ ] Recommendations reference specific projects or moments

### Outreach Messages
- [ ] Under 80 words
- [ ] References something specific about the recipient
- [ ] No "I'd love to pick your brain" or "Can I buy you a coffee?"
- [ ] Ends with a specific, low-effort ask
