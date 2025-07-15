# Lesson 1: Retrieval Augmented Generation (RAG)

## 1. Introduction to RAG

**Retrieval Augmented Generation (RAG)**（检索增强生成）is a technique that significantly extends the capabilities of **Large Language Models (LLMs)**（大语言模型）by enabling them to access additional information beyond what they have learned from publicly available datasets.

### 1.1 Problem with Plain LLMs

If you ask a general-purpose LLM something like:

> “Is there parking for employees?”

It might say:

> “I need more specific information about your workplace.”

This is because the LLM doesn’t know your company’s specific parking policy. RAG addresses this limitation.

## 2. How RAG Works

RAG consists of **three main steps**:

### 2.1 Step 1: Retrieve Relevant Documents

Given the user’s query, e.g., “Is there parking for employees?”, the system searches through a collection of internal documents (e.g., HR policies, facilities manuals) and identifies the **most relevant document**. 

In this case, it may pick a **facilities document** that mentions parking.

### 2.2 Step 2: Construct a Context-Rich Prompt

Next, RAG constructs a new **prompt**（提示词）that includes:

- An instruction:  
  `Use the following pieces of context to answer the question at the end.`

- Retrieved content from the selected document:  
  `All employees may park on levels 1 and 2...`

- The original question:  
  `Is there parking for employees?`

Note: Because LLMs have a limit on **input length**（输入长度）, the system should ideally extract only the most relevant part of the document.

### 2.3 Step 3: Generate the Answer

The final **enriched prompt**（增强提示）is sent to the LLM, which uses both the question and the added context to generate a more accurate and context-aware answer.

In some applications, a **source document link** may be included in the output for transparency and user verification.

## 3. Examples of RAG Applications

### 3.1 PDF Chat Tools

Tools like **PandaChat**, **AskYourPDF**, and **ChatPDF** let you upload a PDF and ask questions about it. They work by applying RAG to retrieve text from the document and answer your queries.

### 3.2 Website & Enterprise Content

- **Coursera Coach**: Answers questions based on Coursera content.
- **SnapChat’s chatbot**: Uses Snap’s internal knowledge base.
- **Hubspot**: Responds to marketing and product questions using RAG.

### 3.3 Next-Gen Search Engines

- **Microsoft Bing**: Chat-based search with RAG.
- **Google’s Search Generative Experience**
- **You.com**: Founded by Richard Socher, uses RAG and chat UI for search.

## 4. LLMs as Reasoning Engines

One powerful mindset shift is to treat LLMs **not as knowledge stores**, but rather as **reasoning engines**（推理引擎）.

Instead of relying on what an LLM has memorized:
- We give it the right context in the prompt.
- Then **ask it to reason** through the content to produce an answer.

This unlocks **a broader set of use cases**—even when using a basic web UI:
- You can manually paste relevant text into the input field.
- Then ask the LLM to generate answers based on that text.

This manual process is still an informal type of RAG!

## 5. Summary

RAG is a practical and widely adopted approach to enhance LLMs:
- Enables LLMs to give customized and up-to-date answers.
- Useful in business settings, websites, PDF assistants, and search engines.
- Encourages a shift from thinking of LLMs as databases to **reasoning engines**.

In the next lesson, we’ll explore **fine-tuning**（微调）—another advanced technique to tailor LLMs for specific applications.
