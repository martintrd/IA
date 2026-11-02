# AI Roadmap

A path of 19 modules and 182 tasks to understand and use AI from A to Z: daily use, math, machine learning, deep learning, LLMs, RAG, agents, production, security and law.

## How to use it

1. Check the `- [ ]` box of each task you finish.
2. Under **My notes**, write what you did, the code or prompt you used, and what you took away from it.
3. Each new term goes into the [[Glossary]], which you fill in with your own words.
4. For each project, duplicate the [[Project Template]] into the Projects folder, and create each reading note in the Readings folder.

## Three possible paths

You don't have to follow the modules in order. Choose based on your current goal:

- **Advanced user (1 to 2 months)**: [[A01 AI General Knowledge|A01]], [[A02 Using AI Assistants Every Day|A02]], [[A03 Advanced Prompt Engineering|A03]], [[A17 Ethics, Law and Society|A17]].
- **Application builder (3 to 6 months)**: add [[A05 Python for Data|A05]], [[A10 Building with APIs|A10]], [[A11 RAG and Semantic Search|A11]], [[A12 Agents and Automation|A12]], [[A13 Local and Open Source AI|A13]], [[A15 Production and MLOps|A15]], [[A16 AI and Cybersecurity|A16]].
- **Deep understanding (6 to 12 months)**: add [[A04 Essential Math|A04]], [[A06 Classical Machine Learning|A06]], [[A07 Deep Learning|A07]], [[A08 Language and Transformer Architecture|A08]], [[A09 Large Language Models|A09]], [[A14 Multimodal and Generative AI|A14]].

Module A18 (tech watch and career) runs continuously from the start.

## Modules

- [[A00 Set Up Your Environment]] (7 tasks) · The basic tools you need to follow the whole path.
- [[A01 AI General Knowledge]] (9 tasks) · Know what you're talking about, and talk about it accurately.
- [[A02 Using AI Assistants Every Day]] (9 tasks) · Become an effective user before becoming a builder.
- [[A03 Advanced Prompt Engineering]] (8 tasks) · Get reliable, reproducible results.
- [[A04 Essential Math]] (9 tasks) · The minimum you need to really understand what's going on. Can be done alongside modules A05 to A07.
- [[A05 Python for Data]] (8 tasks) · The working tool of all of AI.
- [[A06 Classical Machine Learning]] (12 tasks) · The foundations, still widely used in companies.
- [[A07 Deep Learning]] (12 tasks) · Neural networks, from theory to code.
- [[A08 Language and Transformer Architecture]] (9 tasks) · Understand the mechanics that power every LLM.
- [[A09 Large Language Models]] (11 tasks) · How an LLM is built, aligned and evaluated.
- [[A10 Building with APIs]] (10 tasks) · Move from user to developer.
- [[A11 RAG and Semantic Search]] (10 tasks) · Make a model answer from your own documents.
- [[A12 Agents and Automation]] (11 tasks) · Models that act, not just models that answer.
- [[A13 Local and Open Source AI]] (9 tasks) · Run models on your own machine.
- [[A14 Multimodal and Generative AI]] (8 tasks) · Images, audio, video and vision.
- [[A15 Production and MLOps]] (9 tasks) · What separates a demo from a real product.
- [[A16 AI and Cybersecurity]] (12 tasks) · The module that directly boosts your SOC analyst profile.
- [[A17 Ethics, Law and Society]] (9 tasks) · Understand the stakes, not just the technology.
- [[A18 Tech Watch, Projects and Career]] (10 tasks) · Stay up to date and prove it.

## Progress

These tables are displayed with the **Dataview** community plugin.

### By module

```dataview
TABLE length(filter(file.tasks, (t) => t.completed)) AS "Done", length(file.tasks) AS "Total", round(100 * length(filter(file.tasks, (t) => t.completed)) / length(file.tasks)) + " %" AS "Progress"
FROM "Modules"
SORT file.name ASC
```

### Next tasks

```dataview
TASK
FROM "Modules"
WHERE !completed
LIMIT 5
```

### My projects

```dataview
TABLE status AS "Status"
FROM "Projects"
WHERE file.name != "Read Me"
```
