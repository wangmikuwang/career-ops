# Research Scout Reference

Live web research protocol. Load this file when the user needs information the reference files don't hold or hold only as a stale US snapshot: specific company data, uncovered industries, salary figures, current market conditions, or anything outside the United States.

## Activation Triggers

- **Specific company research**: culture, recent news, team structure, hiring patterns for a named employer
- **Salary data**: any role, location, or seniority. The reference files hold no salary figures.
- **Current market conditions**: the tables in market-data.md are a US snapshot from around early 2026
- **Non-US markets**: for China, read `china.md` first for where to look
- **Uncovered industries**: sectors the reference files don't mention

Stable material (frameworks, principles, how to structure an answer) needs no search.

---

## Search Protocol

### Step 1 — Search with Specificity

Never search for broad topics. Construct narrow, specific queries.

- **Wrong**: "software engineer salary"
- **Right**: "senior backend engineer salary Berlin 2026 Levels.fyi"
- **Wrong**: "产品经理 薪资"
- **Right**: "[公司名] 产品经理 [职级] 总包 2026 OfferShow"

Use at least two different queries per topic to reduce single-source risk.

### Step 2 — Evaluate Source Quality

| Source type | Trust level | Example |
|-------------|-------------|---------|
| Named organization with published methodology | High | 国家统计局, BLS, a company's own filings or careers page |
| Publication with editorial oversight | Medium-high | Established business and trade press |
| Named practitioner with verifiable experience | Medium | Signed posts by people who hold or held the role |
| Self-reported aggregates | Low-medium | OfferShow, Levels.fyi, Glassdoor, 看准网. Useful, but report sample size and date |
| Anonymous posts and forums | Low | 脉脉职言, 牛客 threads, 小红书, Reddit. Leads to check, not facts |

Discard anything without an identifiable source. Several anonymous posts repeating one claim are still one unverified claim.

### Step 3 — Compare with the Reference Files

- For time-sensitive or non-US questions, a recent finding from a named source outranks the reference tables. Those tables are mostly T2 vendor surveys of the US market, frozen at the time the upstream repo was written.
- If the finding and the table disagree, show both with their dates and say which applies to the user's market.
- Stable T1 findings (structured interviews predict performance, unexplained gaps cost callbacks) stay the default unless a stronger study contradicts them.

### Step 4 — Present with Source and Date

Every finding from search carries its source name and date, and sample size where the source gives one. Example:

```
OfferShow 上该职级近半年有 7 条自报记录（截至 2026-10），总包集中在 A–B 区间。样本很少，只能当参考。
```

One claim, one source. Don't merge a reference-table figure and a search figure into a single number.

### Step 5 — Honest Fallback

If no reliable source is found:
- Say so: "这个我查不到可靠数据。"
- Do NOT generate plausible-sounding estimates, averages, or statistics.
- Say where the user could look, including sources behind a login you can't read (脉脉, OfferShow 小程序, 内部朋友).
- Offer to proceed with what is known.

---

## Recency Rules

| Age of data | Action |
|-------------|--------|
| Within 12 months | Current. Use with source and date |
| 1-3 years old | Use with caveat: "as of [year]" |
| Older than 3 years | Discard for market data, salary, and trend claims |
| Any age | Acceptable for stable facts (company founding date, methodology descriptions) |

The same rule applies to the reference files themselves: their market tables pass the 12-month mark in early 2027 and should be treated as "as of 2025–2026" after that.

---

## Quality Checklist

- [ ] Every finding has a source name and date
- [ ] Self-reported and anonymous sources are labelled as such, with sample size
- [ ] No statistic was generated, estimated, or extrapolated
- [ ] Disagreements with the reference tables are shown, not silently resolved
- [ ] Recency rules applied
- [ ] US data is never presented as describing another market
