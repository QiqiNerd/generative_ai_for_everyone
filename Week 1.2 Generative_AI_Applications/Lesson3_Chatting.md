# Week 2 Lesson 3: Chatting

## 1. Introduction

In addition to **writing** and **reading** tasks, LLMs are also widely used in **chatting applications**（对话应用）. While general-purpose chatbots like ChatGPT, Bard, and Bing Chat are well known, many businesses are developing **specialized chatbots**（专用聊天机器人） for specific use cases.

## 2. Specialized Chatbots

Specialized chatbots are designed for focused tasks such as:

- **Travel planning**  
  Example: “How can I vacation in Paris inexpensively?”

- **Advice bots**  
  Domains: Career coaching, cooking, fitness, etc.

- **Customer service bots**  
  Tasks: Taking orders, answering FAQs, processing returns

Some bots can also **interface with business systems** to take action, such as:

- Submitting orders
- Sending password reset links
- Verifying user identity

## 3. Chatbot Design Spectrum

Focusing on **text-based chat** (not voice), businesses generally adopt one of several chatbot designs across an **automation spectrum**:

### 3.1 Human-Only Interaction

All messages are written by customer service agents.

Example:  
Agent types, “Welcome to Better Burgers. Let me place your order.”

### 3.2 Bot-Only Interaction

Chatbots handle entire conversations without human intervention.

### 3.3 Human-in-the-Loop (人类在环)

- Bot drafts message
- Human agent **reviews or edits** before sending
- Helps prevent inappropriate or incorrect responses

This approach is especially useful when:

- The **risk of error** is high
- Human oversight is essential

### 3.4 Message Triage

- Bot handles **simple requests**
- More complex or unclear requests are **escalated to humans**

Example:  
A bot detects refund requests and provides instructions without human involvement.

Outcome:  
- Offloads ~10% of traffic from agents
- Frees agents to focus on **more complex cases**

### 3.5 Human + Bot Multitasking

Bots assist agents by generating drafts or handling easy cases, allowing agents to manage **multiple customer chats simultaneously** (4, 8, or even 16 conversations at once).

## 4. Safe Deployment Practices

Deploying bots safely often follows a phased approach:

### Phase 1: Internal Testing

- Bot is only available to internal team
- Safe environment to observe behavior and errors
- Easier to troubleshoot without public exposure

### Phase 2: Human-in-the-Loop

- Bot generates messages
- Humans review before sending to customers

### Phase 3: Full Automation

- Bot communicates directly with customers
- Only used after confidence in safety and performance

Businesses choose different deployment paths based on:

- **Volume of interactions**
- **Risk of incorrect responses**
- **Operational feasibility**

## 5. Summary

LLMs enable powerful chatting capabilities that can:

- Improve customer service
- Reduce response time
- Scale support operations

Design choices depend on context, balancing **efficiency**, **accuracy**, and **safety**.

## 6. Transition

So far, we’ve explored how LLMs can be used for:

- Writing
- Reading
- Chatting

These categories are not exhaustive but represent practical and high-impact use cases. However, LLMs have limitations.

In the next lesson, we will look at what **LLMs can and cannot do**, to better understand where they might fall short.

Let’s move on.
