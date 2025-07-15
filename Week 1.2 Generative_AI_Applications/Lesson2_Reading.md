# Week 2 Lesson 2: Reading

## 1. Introduction

In contrast to writing tasks, where short prompts yield longer outputs, **reading tasks**（阅读任务）usually start with a longer input and produce shorter or similarly-sized outputs. These tasks leverage the LLM’s ability to **understand and process**（理解和处理）text effectively.

## 2. Proofreading

LLMs can detect:

- Spelling errors
- Grammar issues
- Awkward phrasing

### Example:
Prompt:  
“Proofread the following text intended for a children’s stuffed toy website…”

Result:  
- Corrected “snuggle” spelling  
- Improved sentence structure and grammar

This functionality is useful even after multiple rounds of manual proofreading.

## 3. Summarization

LLMs can efficiently summarize long-form content.

### Example:

Andrew received a long article titled *The Turing Trap* by Erik Brynjolfsson. He used an LLM to generate a summary instead of reading the entire article immediately.

Key idea of the article:  
- AI should **augment**（增强）rather than **automate**（自动化）human labor.

This use case is ideal for time-constrained professionals who need to process long texts quickly.

## 4. Summarizing Customer Service Calls

### Scenario:

- A call center manager receives transcripts from recorded customer service calls.
- Each call generates long text.
- LLM is used to **summarize each conversation**.

Example summary:  
“MP401-27KX was reported as broken…”

Managers can quickly spot issues or trends using these summaries.

📝 Note: This use case works best as a **software-based application**（软件型应用） rather than through a web interface.

## 5. Email Classification and Routing

This task involves using an LLM to:

- Determine if an email is a **complaint**（投诉）
- Decide which **department** it should be routed to

### Prompt Issue:

Prompt: “Read the email and route to appropriate department.”

Problem:  
LLM chooses a non-existent department, e.g., “complaints,” which doesn’t exist in the organization.

### Improved Prompt:

“Read the email and choose the department only from the following list: Apparel, Billing, Shipping…”

→ LLM routes correctly to “Apparel”

**Lesson**: Providing structured context is critical for accurate task completion.

## 6. Reputation Monitoring via Sentiment Analysis

You can use LLMs to evaluate **customer reviews** and classify them as **positive or negative**（正面或负面）.

### Example:

Prompt: “Read the following review and classify its sentiment.”

Review: “The food was amazing and the staff were friendly.”  
→ Classified as **positive**

Software can count sentiments over time and generate a **dashboard** showing:

- Trends in customer satisfaction
- Spikes in negative feedback

Managers can then respond proactively to emerging issues.

## 7. Summary

Reading tasks are highly practical and include:

- Proofreading
- Summarization
- Email classification
- Routing
- Sentiment analysis

Use them when:

- You have a **long input**
- You want a **shorter, informative output**

This can automate decision-making and improve productivity in areas like customer service, content analysis, and operations.

## 8. What’s Next

In the next lesson, we’ll explore **chatting tasks**, where LLMs interact with users through back-and-forth dialogue.

Let’s continue.
