# Week 2 Lesson 1: Writing

## 1. Introduction

In the previous lesson, we categorized LLM tasks into **writing**, **reading**, and **chatting**. Given that large language models are trained to **predict the next word**（预测下一个词）, they are especially effective at writing tasks.

Most writing tasks begin with a **short prompt**（简短提示）and result in a **longer, coherent text**.

## 2. Web-based Writing Applications

Many writing tasks can be performed directly through a web interface using general-purpose LLM tools like ChatGPT or Bard.

### 2.1 Brainstorming

LLMs can generate creative ideas based on simple prompts.

Examples:

- Prompt: “Brainstorm 5 creative names for peanut butter cookies”  
  → Output: Names like "Nutty Nirvana Nibbles"

- Prompt: “Brainstorm ideas for increasing cookie sales”  
  → Output: A list of marketing or distribution suggestions

LLMs can be valuable **brainstorming companions**（头脑风暴伙伴）for creative or business tasks.

### 2.2 Writing Marketing Copy

LLMs can help write documents such as:

- Press releases
- Announcements
- Promotional content

#### Example: Press Release

Prompt: “Write a press release announcing the new COO hire”  
→ Output: Generic text like “Company Name Welcomes New COO’s Full Name…”

To make the output more useful:

- Provide additional **context**（上下文） such as:
  - Name and background of the COO
  - Details about the company
  - Company mission or strategic goals

Revised Prompt:  
“Use the following information for the press release: [COO Bio], [Company Description], [Hiring Rationale]”  
→ Output: Much more **specific and relevant** content

**Tip**: It's normal not to get the ideal output on the first prompt. **Revise and retry**.

## 3. Translation Tasks

LLMs can also translate text and sometimes outperform **dedicated machine translation engines**（专用机器翻译引擎）— especially in **high-resource languages**（高资源语言） with abundant training data.

### 3.1 Limitations with Low-Resource Languages

For **low-resource languages**（低资源语言） like formal Hindi, performance can be inconsistent.

Example:

- Prompt: Translate a hotel welcome message into formal Hindi  
  → Initial Output: Awkward phrasing like “desk at the front” instead of “reception”

Revised Prompt: “Translate this into formal **spoken** Hindi”  
  → Output: Improved translation using correct term for "reception"

### 3.2 Creative Use: Pirate English

Many teams use **Pirate English** to test whether translation functions are working logically.

Prompt: “Translate this into Pirate English”  
→ Output: “Ahoy matey, we be hoping you'll relish your time aboard the Oceanview Inn.”

This allows teams to:
- Evaluate formatting and tone
- Test models in non-critical ways
- Have some fun with model outputs

## 4. Summary

Writing tasks are where LLMs excel. They are ideal for:

- Brainstorming
- Drafting content
- Translating between languages (with varying quality)

**Best Practices**:
- Always provide context in your prompt
- Expect to iterate for best results
- Be cautious with low-resource language outputs

In the next lesson, we’ll take a closer look at **reading tasks**, where LLMs interpret long texts to generate shorter summaries or classifications.
