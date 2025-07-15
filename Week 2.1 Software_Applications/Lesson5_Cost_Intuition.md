# Week 3 Lesson 5: Cost Intuition

## 1. Introduction

In this lesson, we build intuition for how much it costs to use large language models (LLMs, 大型语言模型) in software applications. Understanding cost is important for both individual users and companies deploying AI-powered features.

## 2. LLM Pricing Overview

### 2.1 Example Token Prices

Different providers charge based on the number of tokens (标记). These are example prices:

- **OpenAI GPT-3.5**: \$0.002 per 1,000 tokens
- **OpenAI GPT-4**: \$0.06 per 1,000 tokens
- **Google PaLM 2**, **Amazon Titan Lite**: also inexpensive (exact values vary)

Most LLMs charge based on:
- Prompt length (input tokens, 输入标记)
- Response length (output tokens, 输出标记)

However, output tokens tend to be more expensive, so the focus here is on output cost.

### 2.2 What is a Token?

A token is roughly a word or a sub-part of a word:

- Common words like “the” or “example” = 1 token
- “Andrew” = 1 token
- “Translate” → “tran” + “slate” = 2 tokens
- “Programming” → “program” + “ming” = 2 tokens
- Uncommon words like “tonkotsu” → might be 4 tokens

On average:
- 1 word ≈ 0.75 tokens
- 100 words ≈ ~133 tokens

## 3. Cost Estimate for a Use Case

### 3.1 Scenario

You want to estimate the cost of generating enough text to keep someone reading for **1 hour**.

- Average adult reading speed: **250 words/min**
- 1 hour = 60 min → 15,000 words
- Assume prompting also uses 15,000 words
- Total = 30,000 words

### 3.2 Token Conversion

- 30,000 words ≈ **40,000 tokens** (due to 0.75 words/token)

### 3.3 Cost Calculation

Assume OpenAI GPT-3.5 pricing:

- 40,000 tokens / 1,000 = 40 units
- 40 × \$0.002 = **\$0.08 (eight cents)**

This is the total cost to keep someone reading for an hour using an LLM.

## 4. Is It Expensive?

- In the **United States**, minimum wage ≈ \$10–\$15/hour
- LLM output cost ≈ **\$0.08/hour**
- This is a **small incremental cost** if it boosts productivity

However:
- For a **free app with a million users**, 1 million × \$0.08 = \$80,000 → this becomes significant without revenue
- But overall, **LLMs are cheaper than many people expect**

## 5. Conclusion

- Tokens are the basic unit of cost in LLMs
- Generating large volumes of content can be **surprisingly inexpensive**
- Having this cost intuition helps in budgeting for generative AI features

In the next lesson, we’ll explore advanced techniques to make LLMs even more powerful.