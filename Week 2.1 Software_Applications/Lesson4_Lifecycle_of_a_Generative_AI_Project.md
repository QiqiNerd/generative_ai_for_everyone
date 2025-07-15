
# Week 2 Lesson 4: Lifecycle of a Generative AI Project

## 1. Overview

The lifecycle of building a **Generative AI** (生成式人工智能) software application can be broken down into several stages. This process is iterative (迭代式) and empirical (经验驱动), emphasizing rapid prototyping, continuous evaluation, and refinement.

## 2. Main Stages of the Lifecycle

### 2.1 Scoping the Project (项目范围定义)

The first step involves defining the goal of your software project.
- Example: Building a **restaurant reputation monitoring system** (餐厅声誉监测系统).

### 2.2 Initial Prototyping (初步原型制作)

Thanks to the ease of using **prompt-based development** (基于提示的开发), you can create a prototype in a day or two.
- The first version might be poor in performance, but fast prototyping enables faster feedback.

### 2.3 Internal Evaluation (内部评估)

Your internal team tests the system using a variety of inputs:
- Example error: The system classifies "My pasta was cold" as a **positive sentiment** (正面情感), though it's likely negative.
- Discovering such issues helps refine prompts or improve overall system logic.

### 2.4 Iterative Improvement (迭代改进)

Improving generative AI applications involves:
- Revising prompts (提示词调整)
- Rewriting logic
- Adding more examples for prompt context

### 2.5 External Deployment and Monitoring (外部部署与监控)

After internal evaluation, you can release the system externally and observe user inputs.
- Example edge case: “My miso ramen tasted like tonkotsu ramen.”
  - If misunderstood by the system, it may reflect a bias or a domain-specific knowledge gap.

## 3. Example Applications

### 3.1 Restaurant Sentiment Monitoring

#### Traditional Approach (传统方法)
- Supervised Learning (监督学习): Collect labeled reviews → Train a model → Deploy to cloud.
- Timeframe: 6–12 months.

#### Generative AI Approach (生成式人工智能方法)
- Write a prompt → Call LLM (大语言模型) → Deploy.
- Timeframe: Hours to days.

### 3.2 Food Ordering Chatbot (食物点餐聊天机器人)

- Scope: Build a bot to take food orders.
- Internal test: May handle "Do you have pickles?" well, but fail with "Do you have mushrooms?"
- External users may also ask unusual questions like "How many calories in a burger?"
  - Solution: Use **RAG (Retrieval-Augmented Generation, 检索增强生成)** to improve accuracy.

## 4. Generative AI is Highly Empirical (生成式AI是高度实验性的)

- Like prompting, building software applications involves testing and modifying based on feedback.
- Mistakes are expected and essential for improvement.

## 5. Improvement Tools Preview

In addition to prompt engineering, other tools include:
- **RAG (检索增强生成)**: Gives LLMs access to external data.
- **Fine-tuning (微调)**: Customizes LLMs for your task.
- **Pre-training (预训练)**: Training a model from scratch (advanced and resource-intensive).

These will be covered later in the course.

## 6. Cost Concerns

- Many worry about the **cost of using LLMs** hosted on cloud platforms.
- However, using generative AI can often be **cheaper than expected**, especially compared to traditional ML approaches.

Stay tuned for the next lesson where we discuss the cost of running LLMs.

