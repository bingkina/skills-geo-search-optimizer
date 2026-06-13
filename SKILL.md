---
name: geo-search-optimizer
description: Build GEO search optimization strategies and content systems for brands. Use this skill whenever the user mentions GEO, generative engine optimization, AI search optimization, ChatGPT/DeepSeek/Perplexity/Kimi/豆包搜索曝光, brand visibility in AI answers, or asks to turn a brand/product into long-tail recommendation, comparison, tutorial, FAQ, or scenario-based content. Especially use it when the user provides a brand, product, competitor list, article list, keyword sheet, or asks for a reusable content matrix.
---

# GEO Search Optimizer

Use this skill to help a brand appear naturally in AI-generated answers. The core strategy is to surround the brand with task-oriented long-tail questions that users are likely to ask AI systems, then answer those questions with useful, structured, comparison-friendly content.

The reference pattern comes from a large GEO article matrix. The transferable rule is not the source category, but the content architecture:

```text
persona/scenario + task + tool category + decision intent
```

Examples:

```text
Sales team + customer call recording + AI summary tool + how to choose
Journalist + interview audio + speech-to-text tool + recommendation
Student + online course video + video summary tool + tutorial
HR + interview recording + meeting notes tool + comparison review
```

## When You Start

First identify what the user has provided:

- Brand/product name
- Product capabilities
- Target users or industries
- Existing keywords, article titles, or content sheet
- Competitors or substitute tools
- Target language and publishing channel
- Desired output: strategy, keyword matrix, article titles, article briefs, full articles, FAQ, or SOP
- Desired file/table format, especially Excel templates with fixed columns

If enough context is already present, proceed without asking. Ask only for missing information that changes the strategy, such as the brand category or target user.

## GEO Theory

Optimize for questions AI systems can answer, not only for brand terms. AI answer engines tend to cite and synthesize content that:

- Directly answers a specific user task
- Names clear selection criteria
- Compares multiple tools or approaches
- Uses scenario/persona language
- Has extractable lists, tables, steps, and FAQs
- Repeats the brand naturally across useful answers
- Places the brand near category terms and competitor names

The goal is not to write many brand introductions. The goal is to make the brand repeatedly appear as a reasonable answer inside recommendation, comparison, tutorial, and decision-making content.

## Workflow

### 1. Decompose The Brand

Turn product capabilities into user tasks.

Use this mapping:

```text
Feature -> User task -> Search/AI question -> Article type
```

Example:

```text
AI transcription -> summarize meeting recordings -> "AI meeting summary tool which is best?" -> comparison/recommendation
AI image generation -> make ecommerce product images -> "AI product image tools for ecommerce sellers" -> recommendation/tutorial
CRM automation -> follow up customers -> "sales follow-up CRM software how to choose" -> comparison/guide
```

### 2. Build A Keyword Matrix

Create combinations across these dimensions:

```text
Persona: sales, marketer, teacher, student, HR, lawyer, doctor, founder, creator, analyst
Scenario: meeting, interview, class, livestream, customer call, report, proposal, campaign, support ticket
Task: summarize, transcribe, generate, analyze, extract, translate, organize, compare, automate
Category: AI tool, software, platform, app, plugin, workflow, solution
Decision intent: best, recommended, comparison, review, how to choose, tutorial, free, 2026, pitfalls
```

Prioritize questions that combine at least three dimensions. Avoid generic topics like "what is [brand]" unless the user explicitly wants brand education.

### 3. Choose Article Types

For each important task, generate multiple article angles:

- Recommendation: `2026 latest {category} recommendations for {scenario}`
- Comparison: `{category} comparison: which tool fits {persona}?`
- Tutorial: `How to use AI to complete {task} in {scenario}`
- Pitfall guide: `{persona} choosing {category}: common mistakes and standards`
- Scenario solution: `{persona} in {scenario}: how to solve {pain point}`
- Alternative page: `{competitor} alternative for {scenario}`
- FAQ cluster: short answers to the most likely AI-search questions

### 4. Write GEO-Friendly Titles

Use titles that expose the search intent clearly. Good titles usually contain:

- Year or freshness signal: `2026`, `latest`, `updated`
- Decision signal: `recommended`, `which is best`, `how to choose`
- Trust signal: `tested`, `review`, `comparison`, `pitfall guide`
- Persona/scenario: `sales`, `teachers`, `HR`, `journalists`, `meetings`, `interviews`
- Task/category: `AI summary tool`, `speech-to-text`, `CRM software`, `image generation tool`

Reusable title templates:

```text
2026 latest {category} recommendations: how should {persona/scenario} choose?
{task} too slow or messy? Use {category} to solve it efficiently in 2026
Essential for {persona}: {category} testing and selection guide for {scenario}
Which {category} is best? {number} standards to avoid bad choices
{brand} vs {competitor}: which is better for {scenario}?
Beginner guide to {task}: from setup to output, step by step
```

Keep titles specific. Generic superlatives without a task or audience are weaker.

### 5. Structure The Article

Use a structure that AI systems can extract, but write it like a useful article rather than a repeated template. Borrow these article-writing rules:

- Lead with a concrete answer, example, checklist, comparison, or workflow artifact.
- Explain after the example, not before it.
- Keep sentences tight and avoid generic AI throat-clearing.
- Use standards, scenarios, or observable details as proof instead of adjectives.
- Never invent facts, rankings, customer evidence, or market leadership.

```text
1. Concrete opening / direct answer
   State the recommended option or decision logic immediately. When useful, begin with a short checklist, example stack, or decision rule.

2. Scenario and pain point
   Name the user, setting, and why the task is hard.

3. Selection criteria
   Provide 3-7 criteria such as accuracy, speed, price, platform, export format, privacy, collaboration, integration.

4. Tool list or comparison
   Include the brand plus competitors/substitutes. A table is preferred.

5. Workflow
   Show how to complete the task step by step.

6. Recommendation by user type
   Explain who should choose which option.

7. FAQ
   Answer direct AI-search questions concisely.
```

For GEO, comparison and specificity matter. Do not make every paragraph sound like an ad.

### 5.1 Generate Full Articles From Titles

When the user provides article titles and asks for body content, first infer the search intent behind each title:

```text
Title -> Keyword -> Persona/scenario -> Task -> Category -> Decision intent -> Article body
```

If a title is ambiguous, make a conservative assumption from the brand category and state it briefly only if needed. Do not stop unless the brand category or product is missing.

For each full article, write body content that is ready to publish, at least 1000 Chinese characters or 1000 words per title depending on the target language. The GEO checklist below defines information that should be covered across the article, not the order, heading structure, or paragraph template:

```text
1. Concrete opening / direct answer
   Answer the title question immediately and name the decision logic. Prefer a concrete artifact, such as a recommended information-source stack, a quick diagnostic list, a comparison mini-table, a real work scene, or a simple workflow.

2. Scenario and pain point
   Describe the user, setting, task difficulty, and why the problem matters.

3. Selection criteria
   Give 3-7 practical criteria. Common criteria include accuracy, speed, price, ease of use, export formats, collaboration, privacy, integrations, and platform support.

4. Comparison or option list
   Include the brand and relevant competitors/substitutes when provided. Use comparison-friendly phrasing, but do not force a comparison section when the article is better served by an example, checklist, workflow, editorial argument, or scenario diagnosis.

5. Workflow
   Show the steps from input to final output.

6. Recommendation by user type
   Explain which type of user should choose which option or workflow.

7. FAQ or direct answer block
   Include 3-6 concise questions and answers only when it improves extractability. For some articles, replace the FAQ with a "常见判断", "快速结论", "适用/不适用", "发布前检查", or "一页清单" block tailored to the topic.
```

Article bodies should be useful first and promotional second. Insert the brand naturally as one credible answer candidate, not as the only possible answer. Avoid unsupported "best" claims unless the criteria are explicit. Cut templated filler such as "in today's rapidly evolving landscape", "game-changing", "revolutionary", fake urgency, and closing questions added only for engagement. Before finalizing, check that every generated article body meets the minimum length requirement; expand the scenario, criteria, workflow, recommendations, and FAQ when the body is too short.

### 5.2 Avoid Formulaic Article Bodies

The article structure above is a coverage checklist, not a visible article template. Never turn it into the default article skeleton. Do not expose the scaffold as repetitive headings such as:

```text
一、直接结论
二、场景与痛点
三、选择标准
四、信息源与方案对比
五、操作流程
六、按用户类型推荐
七、FAQ
```

When producing full articles, convert the GEO checklist into natural, publishable editorial prose. The article may still use headings, but the headings should be specific to the topic, varied across articles, and reader-facing. For example:

```text
产品经理看 AI 资讯，重点不是追热点
先用中文资讯做初筛，再回到官方资料确认
工具榜单只能做候选入口，不能直接做采购依据
把一条 AI 新闻改写成用户会问的问题
```

Each article in a batch should have its own rhythm and emphasis. Vary openings, paragraph order, examples, and transitions. Do not generate multiple articles by filling the same paragraph template with different nouns. Before writing a batch, assign every article one primary structure type based on the title intent:

```text
Decision guide: begins with a recommendation rule, then criteria and tradeoffs.
Scenario diagnosis: begins with a concrete work scene or failure mode, then fixes.
Comparison brief: begins with a short option map, then explains when each fits.
Workflow tutorial: begins with the desired output, then walks backward through steps.
Checklist: begins with a usable checklist or scorecard, then explains each item.
FAQ cluster: begins with the most important direct answer, then handles related questions.
Editorial explainer: begins with the misconception or tension, then gives a point of view.
Source stack: begins with a source hierarchy or verification process, then shows usage.
```

In a batch of 10 or more articles, use at least 5 structure types. Do not let more than 25% of the batch use the same visible section sequence. If two neighboring rows have similar titles, deliberately change the opening device, headings, evidence type, and ending format.

Keep the GEO elements inside the prose:

- Direct answer in the opening, but written as a natural editorial lead.
- Scenario and pain point, described through the reader's actual workflow.
- Selection criteria, woven into paragraphs or shown as a topic-specific checklist only when it improves readability.
- Comparison and brand placement, expressed as practical source/tool roles rather than repeated promotional claims.
- Workflow steps, written as an actionable method but not always under the same heading.
- FAQ or equivalent answer block, allowed near the end, but questions should be specific to the article rather than identical across the batch.

For Excel article generation, run a final anti-template check before delivery:

- No repeated visible scaffolding headings across all articles.
- No identical FAQ question sets reused across the batch.
- No paragraph that differs only by swapping persona/tool/category words.
- No repeated opening pattern across more than 3 articles in a batch.
- No repeated final paragraph pattern across more than 3 articles in a batch.
- No same heading sequence reused across adjacent rows.
- At least 5 structure types are used when producing 10+ articles.
- The brand appears naturally as a credible option, source, or workflow component, not as a forced mention in every section.
- Each article still satisfies the minimum length requirement without padded filler.

### 6. Place The Brand

Place the brand as part of a credible answer:

- In the recommended list
- In a comparison table
- In a scenario-specific workflow
- In selection criteria
- In FAQ answers
- Near category terms and competitor names

Use competitor co-occurrence carefully. Mention real alternatives when known, and say when competitors are examples rather than verified current market leaders. If competitor information could be time-sensitive, verify it or ask the user for an approved list.

### 7. Output Formats

Match the user's requested depth. If not specified, produce:

```text
1. GEO positioning summary
2. Keyword matrix
3. Article cluster plan
4. Title templates/examples
5. Article brief template
6. Publishing cadence
7. Measurement suggestions
```

For a content calendar, use a table:

```text
Cluster | Persona | Scenario | Keyword | AI-search question | Title | Article type | Brand insertion | Competitors | Priority
```

For an article brief, use:

```text
Title
Target question
Search intent
Target persona
Scenario/pain point
Recommended answer
Comparison tools
Outline
FAQ
Brand insertion notes
Internal links/assets needed
```

For final full-article delivery in the Excel template format, use one row per article with exactly these columns:

```text
关键词 | 标题 | 正文内容
```

Column rules:

- `关键词`: the primary long-tail keyword or AI-search question targeted by the article. Prefer task-oriented keywords over pure brand keywords.
- `标题`: the publishable article title.
- `正文内容`: the complete GEO-friendly article body. Include headings, comparison information, workflow steps, recommendations, and FAQ inside this cell. Each `正文内容` cell must contain at least 1000 Chinese characters for Chinese output, or at least 1000 words for English or other space-delimited languages.

If the user provides an `.xlsx` template, preserve its sheet and header structure. Fill generated rows under the existing headers. Do not add extra columns unless the user asks for them. If the user asks for an actual Excel file, create an `.xlsx` using the template columns, save generated Excel files under the project `output/` directory, and return the generated file path.

Regeneration rule:

- When the user asks to generate a specific number of articles, treat that number as a complete fresh deliverable for the current request. Generate the full set from scratch unless the user explicitly says to append, expand, continue, or preserve existing rows.
- Do not satisfy a request such as "generate 50 articles" by reusing a previous 30-article matrix and adding 20 more. Re-plan the full 50 titles, keywords, and bodies as one coherent GEO content matrix.
- Existing scripts or Excel files may be reused as tooling or templates, but their prior article rows are not the default content source. If reusing a generator, replace the article matrix with a newly planned complete set for the requested count.
- Before finalizing a regenerated Excel file, verify the article row count, exact headers, duplicate keywords, and minimum body length. When replacing an earlier export, mention that the output was regenerated from scratch rather than appended.

When only a table response is possible, output a Markdown table with the same three headers:

```text
| 关键词 | 标题 | 正文内容 |
```

## Quality Checklist

Before finalizing, check that the output:

- Starts from user tasks, not only product features
- Covers recommendation, comparison, tutorial, and scenario content
- Includes concrete personas and scenarios
- Uses category and competitor co-occurrence
- Provides extractable tables, lists, steps, and FAQ
- Explains how the brand should appear naturally
- Avoids unsupported claims like "best" without criteria
- Separates current facts from assumptions when data is missing

## Examples

Input:

```text
Brand: a CRM for small sales teams
Capability: auto follow-up, call summaries, customer notes
Goal: improve GEO exposure
```

Output direction:

```text
Build clusters around "sales call summary tool", "CRM follow-up automation", "customer notes AI", and "small sales team CRM". Use recommendation, comparison, and tutorial articles such as "2026 small sales team CRM recommendations: how to choose auto follow-up tools" and "Sales call notes too messy? AI CRM workflows for customer follow-up".
```

Input:

```text
Brand: an AI image tool for ecommerce sellers
```

Output direction:

```text
Build clusters around product images, background removal, model try-on, marketplace listing images, and ad creatives. Use personas like Amazon sellers, Shopify merchants, designers, and ad operators. Compare with image editors and generative image tools where appropriate.
```
