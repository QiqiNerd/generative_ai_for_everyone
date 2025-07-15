# Lesson 1: Tool Use and Agents

## 1. Introduction

In this lesson, we explore how **Large Language Models (LLMs)**（大型语言模型）can interact with external software systems by **using tools**（工具调用）and the emerging concept of **agents**（智能体）that can autonomously decide sequences of actions.

## 2. Tool Use

### 2.1 Example: Food Order Chatbot

LLMs, such as a food-ordering chatbot, may generate a response like:

> “OK, it’s on the way.”

However, behind the scenes, more happens. The LLM must **trigger a software tool** to place the order, for example:

```
Order burger for user 9876
Send to: 123 Example St
Charge card: **** **** **** 1234
Message to user: OK, it’s on the way
```

Only the last line is shown to the user, while the rest is parsed by backend software to place the order.

### 2.2 Safety Precaution

Because LLMs can make mistakes, developers should design **user confirmation interfaces**（用户确认界面）before executing costly or irreversible actions, such as charging a credit card.

### 2.3 Example: Calculator as Tool

LLMs are not very reliable at **precise math**. Given a prompt like:

> “How much will I have after 8 years if I deposit $100 with 5% interest?”

An LLM may output a wrong answer (e.g., $147.40 instead of \$147.74). Instead, we can let the LLM output a **command** for a calculator tool:

```
calculator: 100 * (1.05^8)
```

This command is interpreted by an external **calculator program**, and the result is plugged back into the LLM’s final user response.

### 2.4 Benefits of Tool Use

Giving LLMs access to tools improves:

- Accuracy (e.g., in math)
- Action-taking (e.g., order placement)
- Domain-specific logic (e.g., finance, health)

However, caution is necessary to avoid misfiring tools or causing harm.

## 3. Agents

### 3.1 Definition

**Agents**（智能体）go beyond one-shot tool use. They can **reason** about a **sequence of actions** to complete a complex task.

### 3.2 Example: Market Research Agent

Prompt:

> “Help me research BetterBurger’s top competitors.”

The LLM as a reasoning engine may:

1. Search for top competitors online
2. Visit competitor websites
3. Summarize homepage content

### 3.3 How It Works

- The LLM **decides** the steps
- Triggers tools like:
  - Web search
  - Website crawling
  - Summarization
- May **loop** over this process to complete multi-step tasks

### 3.4 Current Limitations

While promising, current **agent-based LLMs are still experimental**. Challenges include:

- Reliability
- Safety
- Tool orchestration
- Handling ambiguity

## 4. Summary

Tool use and agent capabilities represent the frontier of LLM applications:

- **Tool Use** enhances what an LLM can do (action or reasoning)
- **Agents** enable LLMs to plan and execute **multi-step tasks**

Both require careful design and are most powerful when **safety, user control, and clarity** are ensured.

## 5. Coming Next

In the next week, we will:

- Explore how Generative AI is impacting **businesses**
- Identify possible **AI use cases**
- Analyze effects on **society and jobs**

Stay tuned!
