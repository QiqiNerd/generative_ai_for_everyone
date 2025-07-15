# Week 3 Lesson 1: Using Generative AI in Software Applications

## 1. Introduction

In previous lessons, we explored using **generative AI**（生成式人工智能）via web interfaces. This week, we shift focus to how it is used within **software applications**（软件应用）. We’ll also explore technology options beyond simple prompting, such as using AI on **proprietary documents**（专有文档） instead of only on public Internet data.

## 2. Examples of Generative AI Applications

Recapping from last week, generative AI can power software that:

- Answers questions based on **internal policy documents** (e.g., company parking rules)
- Reads and analyzes **restaurant reviews**（餐厅评论） for sentiment and reputation monitoring
- Powers **chatbots**（聊天机器人） to take food orders

While some of these systems existed pre-GenAI, the arrival of generative AI has made:

- Development **faster**
- Systems **more powerful and efficient**

## 3. Traditional AI Development: A Long Timeline

### 3.1 Supervised Learning Approach（监督学习方法）

Steps to build a sentiment analysis system traditionally:

1. **Collect labeled data**（收集带标签的数据）
   - Example: “Best soup dumplings I’ve ever eaten.” → Positive
2. **Train a model**（训练模型） with a machine learning team
3. **Deploy using cloud platforms**（部署到云平台） like AWS, GCP, or Azure

Total time:  
- Data collection: ~1 month  
- Model training: ~3 months  
- Deployment: ~3 months  
→ **6–12 months** in total

This process was slow, required experts, and demanded infrastructure support.

## 4. Prompt-Based Development: A New Paradigm（基于提示的开发：新范式）

Now, with **prompt-based AI**:

- The same task can be implemented in **minutes to days**
- No labeled dataset or model training required

### 4.1 Coding Example

Only minimal code is needed:

```python
prompt = "Classify the following review as having either a positive or negative sentiment: Best bubble tea I’ve ever had."
response = call_large_language_model(prompt)
print(response)
```

This replaces hundreds or thousands of lines of traditional ML code.

### 4.2 Time Comparison

| Approach               | Timeline        |
|------------------------|-----------------|
| Supervised Learning    | 6–12 months     |
| Prompt-Based AI        | Hours to Days   |

This democratization allows **millions of developers** to build apps that previously required elite ML teams.

## 5. Important Caveat: Works Best on Unstructured Data（非结构化数据）

Generative AI excels with:

- Text
- Images
- Audio

It is **less effective** for structured/tabular data (like spreadsheets), which are better handled by **traditional supervised learning**.

## 6. Empowering the Community

Lowering the **barrier to entry**（进入门槛）has led to:

- Explosive growth in AI applications
- Broader access for non-experts
- Faster innovation cycles

This trend marks a shift from “ML engineers required” to “anyone can build.”

## 7. What’s Next

In the optional next video, you’ll see a hands-on demo for reading and classifying restaurant reviews. You’re encouraged to try it out—even if you’ve never coded before—just to see how accessible building AI apps has become.

Then we’ll return to explore the **project lifecycle**（项目生命周期） of building generative AI software systems.

See you there.
