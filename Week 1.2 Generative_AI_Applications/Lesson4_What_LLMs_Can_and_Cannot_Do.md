# Week 2 Lesson 4: What LLMs Can and Cannot Do

## 1. Introduction

Generative AI is powerful, but not unlimited. In this lesson, we examine:

- A **mental model**（思维模型）for understanding LLM capabilities
- Specific **limitations**（局限性）of LLMs
- Best practices for use

## 2. A Useful Mental Model: The Fresh College Graduate

Ask yourself:
> Can a **fresh college graduate**（刚毕业的大学生）, given the same prompt, complete this task?

If yes, then an LLM likely can too.

### Examples:

- **Email classification**（邮件分类）: Can the email be identified as a complaint? → Yes  
- **Sentiment analysis**（情感分析）: Is the review positive or negative? → Yes  
- **Press release creation without context** → Only generic output  
- **Press release with company and COO details** → Output improves significantly

**Key idea**: Treat the LLM as a generalist (通才) with no memory, limited to what's in the prompt.

It’s like giving each task to a new graduate **without training** and **without web access**.

This analogy is not perfect, but it helps clarify what LLMs can and cannot do with prompting alone.

## 3. Limitation 1: Knowledge Cutoff（知识截止点）

LLMs are trained on Internet data from a specific time. For example:

- A model trained up to **January 2022** won’t know events after that date.
  - E.g., highest-grossing film of 2022 → Model may say “I don’t know”
  - E.g., **LK-99** (室温超导材料) → Absent if post-cutoff

**Definition**: The model's **knowledge cutoff** is the latest date of training data.

## 4. Limitation 2: Hallucination（幻觉）

LLMs may confidently **make things up**（捏造事实）.

### Examples:

- Quotes by Shakespeare about Beyoncé → False but plausible-sounding
- Court cases → May invent fictional cases like "Ingersoll v. Chevron"

### Real-world risk:

- A lawyer used ChatGPT to draft legal text
- Submitted fake cases in court → Received sanctions

**Lesson**: Always verify critical outputs, especially for legal, medical, or factual use.

## 5. Limitation 3: Context Length（上下文长度）

Each LLM has limits on:

- **Input length**（输入长度）
- **Output length**（输出长度）
- **Total context length** = Input + Output

Example:

- Prompt exceeds token limit → Model refuses or truncates
- Strategy: Break long documents into chunks

Some advanced models support **longer contexts** (tens of thousands of words).

## 6. Limitation 4: Poor Performance on Structured Data（结构化数据表现差）

Structured data = Tabular format (如 Excel, CSV)

Example:

- Predict house price from size  
- Input: Table with square footage and price

LLMs perform poorly on these tasks. **Supervised learning**（监督学习）is more suitable.

Unstructured data = Text, images, audio, video → LLMs excel here.

This course focuses mainly on **text-based unstructured data**（非结构化数据）.

## 7. Limitation 5: Bias and Harmful Output（偏见与有害输出）

### 7.1 Societal Bias（社会偏见）

LLMs may reproduce biased stereotypes from training data.

Example:

- Prompt: “The surgeon walked to the parking lot and took out…”  
  - LLM might say: “his car keys”
- Prompt: “The nurse walked to the parking lot…”  
  - LLM might say: “her phone”

Bias: Associating surgeon with male, nurse with female.

### 7.2 Toxic or Dangerous Output（有毒或危险内容）

Some LLMs may generate:

- Toxic speech
- Instructions for harmful or illegal acts

**Good news**: Major providers have significantly improved **safety mechanisms**（安全机制）.

Using trusted web interfaces (e.g., ChatGPT) reduces this risk.

## 8. Summary

### What LLMs **can** do:
- Complete tasks similar to those a generalist could do with written instructions
- Handle unstructured data, especially text
- Perform well in writing, reading, and chatting tasks

### What LLMs **cannot** do:
- Access up-to-date information
- Guarantee factual accuracy
- Reason effectively over structured tables
- Avoid all harmful or biased output

Understanding these limitations is essential to using LLMs **responsibly**（负责任地）.

## 9. Looking Ahead

Next, we’ll explore **prompting techniques** to improve results and mitigate limitations.

See you in the next lesson.
