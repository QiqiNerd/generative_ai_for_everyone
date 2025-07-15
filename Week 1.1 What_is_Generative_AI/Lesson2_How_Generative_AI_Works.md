# Week 1 Lesson 2: How Generative AI Works

## 1. Introduction

The text generation ability of tools like ChatGPT and Bard can seem magical. This lesson explains what powers these generative AI systems, enabling a better understanding of:

- What they can and cannot do
- When and how to use them effectively

## 2. Generative AI in the Broader AI Landscape

AI is best understood as a **set of tools**（工具集合）. Among them, two are currently most important for practical use:

- **Supervised Learning**（监督学习）
- **Generative AI**（生成式人工智能）

Other methods such as **Unsupervised Learning**（无监督学习）and **Reinforcement Learning**（强化学习）exist, but for this course, the focus is on the first two.

## 3. What is Supervised Learning?

Supervised learning trains a model to map inputs (A) to outputs (B). It uses labeled data and forms the foundation of modern generative AI.

### 3.1 Examples of Supervised Learning

- **Spam detection**:  
  - Input A: An email  
  - Output B: 0 (not spam) or 1 (spam)

- **Online advertising**:  
  - Input A: Ad + user information  
  - Output B: Probability of clicking the ad

- **Self-driving cars**:  
  - Input A: Camera + radar images  
  - Output B: Position labels for other vehicles

- **Medical diagnostics**:  
  - Input A: X-ray  
  - Output B: Diagnosis label

- **Manufacturing**:  
  - Input A: Product image  
  - Output B: Defect label

- **Speech recognition**:  
  - Input A: Audio clip  
  - Output B: Text transcript

- **Sentiment analysis**:  
  - Input A: Product review  
  - Output B: Positive/Negative label

Supervised learning had its "golden decade" from **2010–2020**, during which massive datasets were used, but performance plateaued when using **small AI models**（小型模型）.

## 4. The Power of Large AI Models

Researchers discovered that when using **very large models**（超大模型）with powerful computers and lots of memory, feeding more data **improved performance continuously**.

This insight led to major progress in AI and set the stage for **generative AI**.

Andrew Ng’s leadership at **Google Brain** focused on this principle:  
> “Build large models and feed them lots of data.”

This approach remains central to generative AI today.

## 5. How Text Generation Works

The core technology behind generative AI text tools like ChatGPT is the **Large Language Model (LLM)**（大型语言模型）.

### 5.1 Prompt Completion

Given a prompt such as:
> I love eating...

An LLM might complete it with:

- "bagels with cream cheese"
- "my mother’s meatloaf"
- "out with friends"

Each run can yield a different but coherent result.

### 5.2 Training Process

LLMs are trained using **supervised learning** to predict the **next word**（下一个词）based on previous words.

#### Example:
Given the sentence:
> My favorite food is a bagel with cream cheese.

This becomes multiple training examples:
- Input A: "My favorite food is a" → Output B: "bagel"
- Input A: "My favorite food is a bagel" → Output B: "with"
- Input A: "My favorite food is a bagel with" → Output B: "cream"
- ... and so on

Training an LLM requires:
- Hundreds of billions to over a **trillion words**（万亿级词语）
- **Massive computational resources**（庞大的计算资源）

### 5.3 Final Behavior

A trained LLM, given a prompt, is excellent at generating coherent follow-up text. In essence, it is:
> A system that **predicts the next word** based on a prompt.

This fundamental process powers most generative AI tools.

## 6. Looking Ahead

Next week, the course will cover:

- How LLMs are made to **follow instructions**（执行指令）
- How they are made **safe**（安全性训练）

For now, it's important to know that:
> LLMs are trained to **predict the next word**, and that’s how text generation works.

## 7. Real-World Use

Many people already use LLMs in their daily work to:

- Assist with writing
- Search for information
- Brainstorm or think through ideas

The next video will showcase common use cases of generative AI in action.
