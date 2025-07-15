# Week 3 Lesson 2: Fine-tuning

## 1. Introduction to Fine-tuning

Fine-tuning（微调）is a technique that allows developers to adjust a pre-trained large language model (LLM, 大型语言模型) so that it can generate more customized outputs or handle specific types of information.

Unlike Retrieval Augmented Generation (RAG, 检索增强生成), which adds external information via prompts, fine-tuning actually changes the internal weights of the LLM based on new training data. This is particularly useful when:
- The context exceeds the LLM’s input limit.
- You want the model to adopt a specific style.
- You want a smaller model to perform better on a defined task.

## 2. How Fine-tuning Works

### 2.1 Pre-training vs Fine-tuning

Pre-training（预训练）is the initial phase where a model is trained on massive amounts of public text data—hundreds of billions or even trillions of words. It learns general language patterns, such as predicting the next word:  
e.g. *“My favorite food is a bagel with cream cheese.”*

Fine-tuning, on the other hand, involves additional training on a more specific and often smaller dataset to adjust the model’s behavior or outputs.

### 2.2 Shifting the Model’s Style

To change the tone of an LLM—for example, to make it more positive—you can fine-tune it on optimistic sentences like:
- *“What a wonderful chocolate cake!”*
- *“The novel was thrilling.”*

Even training on 10,000 to 1,000,000 such words can alter the output style of a pre-trained LLM significantly.

## 3. Applications of Fine-tuning

### 3.1 Tasks Hard to Define via Prompting

Some tasks are too subtle or complex to describe through a text prompt. Fine-tuning can help in:
- **Customer service summaries（客户服务摘要）**: Rather than a generic summary, a fine-tuned model could learn to produce highly specific summaries such as:
  *“MK401-27KX monitor reported broken by customer 5402.”*

- **Mimicking personal styles（模仿个人风格）**: If you want an LLM to speak like a specific person (e.g., Andrew Ng), prompting is insufficient. But fine-tuning with transcripts of that person’s actual speech can help generate outputs in their unique voice.

- **Cartoon or fictional characters**: Fine-tuning can give characters distinct, consistent speech patterns.

### 3.2 Domain Knowledge Adaptation

Fine-tuning allows an LLM to adapt to domain-specific language, such as:

- **Medical notes（医疗笔记）**:
  *“Pt c/o SOB on DOE. PE: mild wheezing. Rx: STAT chest X-ray.”*  
  Such text is difficult for general LLMs to process unless fine-tuned with similar examples.

- **Legal documents（法律文件）**:
  *“Licensor grants to licensee per Section 2(a)(iii)... within 15 days hereof.”*  
  Fine-tuning helps the LLM understand complex legal jargon.

- **Financial documents（财务文件）**:
  Specialized documents involving balance sheets, equity terms, etc., can also benefit from domain fine-tuning.

### 3.3 Using Smaller Models More Effectively

Large models (100B+ parameters) require expensive GPUs and are hard to run on laptops or phones. Smaller models (~1B parameters) are cheaper and more portable but less capable.

Fine-tuning a smaller model on task-specific data (like classifying restaurant reviews) allows it to perform nearly as well as large models for certain narrow tasks, reducing cost and latency（延迟）.

## 4. Summary of Fine-tuning Benefits

Fine-tuning is a powerful and often cost-effective tool. You might use it when:

- The task is difficult to specify via prompt.
- You need the model to adopt a specific tone or style.
- You want the model to understand a specialized domain.
- You want to get smaller models to perform nearly as well as large models on targeted tasks.

Fine-tuning typically costs tens to hundreds of dollars, depending on the size of your dataset.

In the next lesson, we’ll look at **pre-training（预训练）**, which is much more expensive and usually only attempted by large tech companies.

