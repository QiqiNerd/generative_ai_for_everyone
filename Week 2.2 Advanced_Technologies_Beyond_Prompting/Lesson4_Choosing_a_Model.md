# Week 3 Lesson 4: Choosing an LLM

## 1. Introduction

When using a Large Language Model (LLM, 大型语言模型) to build software applications, developers often face a wide variety of options—some LLMs are large, others small; some are open-source (开源), while others are closed-source (闭源). This lesson provides a detailed guideline on how to choose the most suitable model for your application.

## 2. Model Size and Capabilities

### 2.1 Small Models (~1 Billion Parameters)

- **Capabilities**: Basic pattern matching (模式识别), limited world knowledge (世界知识).
- **Use Cases**: Suitable for simple tasks such as classifying restaurant reviews by sentiment.
- **Cost**: Lower deployment cost; often usable on laptops or even mobile phones.

### 2.2 Medium Models (~10 Billion Parameters)

- **Capabilities**: Improved world knowledge; better at following basic instructions.
- **Use Cases**: Tasks such as building a food-order chatbot become more feasible.

### 2.3 Large Models (100+ Billion Parameters)

- **Capabilities**: Extensive world knowledge across diverse fields like philosophy, science, and history; capable of complex reasoning (复杂推理).
- **Use Cases**: Ideal for brainstorming (头脑风暴), deep analytical tasks, or applications requiring high knowledge depth.

## 3. Practical Considerations: Try and Test

Even though model size gives a rough idea of capabilities, **development with LLMs is highly empirical (经验性的)**. You are encouraged to test several models and choose based on observed performance in your specific use case.

## 4. Open-source vs Closed-source Models

### 4.1 Closed-source Models

- **Access**: Generally accessed via cloud APIs (云API).
- **Advantages**:
  - Easy integration into software.
  - Often inexpensive due to economies of scale.
  - Hosted by large tech firms with strong infrastructure.
- **Disadvantages**:
  - Vendor lock-in (供应商锁定) risks.
  - Dependency on external platforms for uptime and future availability.

### 4.2 Open-source Models

- **Advantages**:
  - Full control over the model and infrastructure.
  - Can be deployed on-premises (本地部署), including laptops, PCs, or private servers.
  - Better for ensuring **data privacy (数据隐私)**, especially for sensitive domains such as healthcare.
- **Example**: In a healthcare project involving electronic health records (EHRs, 电子健康记录), an open-source model was required to avoid uploading private data to cloud servers.

## 5. Summary of Week 3

This week covered:

- The life cycle of building a generative AI (生成式人工智能) application.
- Enhancing LLM capability using **RAG (检索增强生成)** and **Fine-tuning (微调)**.
- How to choose the right model based on your application's needs and privacy constraints.

## 6. What's Next

There are two optional videos:

- One dives deeper into how LLMs can follow instructions safely.
- The other explores advanced technologies that allow LLMs to:
  - Automatically decide what actions to take.
  - Integrate external tools during operation.

In the next and final week, we’ll explore the societal and business impact of LLMs. Topics include:

- Identifying high-impact LLM use cases for your company.
- A framework to assess how generative AI affects different jobs.
- How individuals and businesses can navigate these changes.

Looking forward to seeing you in Week 4!