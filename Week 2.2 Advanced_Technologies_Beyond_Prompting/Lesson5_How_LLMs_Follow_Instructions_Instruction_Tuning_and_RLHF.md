# Week 3 Lesson 5: How LLMs follow instructions: Instruction tuning and RLHF

## 1. Introduction

Large Language Models (LLMs) were originally trained to **predict the next word (预测下一个词)** based on vast amounts of Internet text. However, when we prompt an LLM today, it often **follows our instructions (遵循我们的指令)** instead of simply continuing the text. This behavior is largely enabled by two important techniques:

- **Instruction Tuning (指令微调)**
- **Reinforcement Learning from Human Feedback, RLHF (基于人类反馈的强化学习)**

This lesson explains how these techniques help LLMs understand and execute instructions in a helpful, honest, and harmless way.

## 2. Instruction Tuning (指令微调)

### 2.1 Why Instruction Tuning?

If a model is only trained to predict the next word, it might complete a prompt like:

> "What is the capital of France?"

with another question, such as:

> "What is the capital of Germany?"

This is because LLMs have seen many sequences of questions on the Internet and might just continue the pattern.

### 2.2 What Instruction Tuning Does

To make the model **follow instructions**, we take a pre-trained LLM and **fine-tune (微调)** it on a dataset that contains:

- A **prompt or instruction (指令)**
- A **good response (优质回答)**

Example pairs might include:

- Prompt: "What is the capital of South Korea?"
- Response: "The capital of South Korea is Seoul."

- Prompt: "Help me brainstorm some fun museums to visit in Bogotá."
- Response: "Sure! Here are some fun museums in Bogotá:..."

- Prompt: "Tell me how to break into Fort Knox."
- Response: "Sorry, I can't help with that."

By feeding the LLM many of these examples, it learns to **respond appropriately and helpfully** to user instructions.

## 3. RLHF: Reinforcement Learning from Human Feedback (基于人类反馈的强化学习)

### 3.1 Motivation for RLHF

Even with instruction tuning, not all LLM outputs are perfect. To further improve quality and **align outputs with human preferences**, developers use RLHF. It helps LLMs produce responses that are:

- **Helpful (有帮助的)**
- **Honest (诚实的)**
- **Harmless (无害的)**

### 3.2 How RLHF Works

#### Step 1: Train an Answer Quality Model

1. Have humans **rate multiple LLM outputs** to the same prompt.
2. Label them based on how good the answer is (from bad to excellent).
3. Use these ratings as a dataset to **train a supervised model** that scores new responses.

Example:

- Prompt: "Advise me on how to apply for a job"
  - Response A: "Here are some helpful steps..." → Score: 5
  - Response B: "Just try your best." → Score: 3
  - Response C: "It's hopeless, why bother?" → Score: 0

Now we have a **reward model (奖励模型)**.

#### Step 2: Reinforcement Learning Using Reward Scores

1. The LLM generates many responses.
2. The reward model **scores each response automatically**.
3. Use **reinforcement learning algorithms (强化学习算法)** to adjust the LLM, so it generates responses with higher predicted scores.

This way, the LLM is encouraged to consistently produce **better, safer, more aligned answers**.

## 4. Summary

- **Instruction tuning** teaches LLMs to follow instructions instead of just predicting the next word.
- **RLHF** builds on that by training the model to generate responses that score well on **helpfulness, honesty, and safety**.
- These techniques are fundamental in making modern LLMs more useful and trustworthy in real-world applications.

