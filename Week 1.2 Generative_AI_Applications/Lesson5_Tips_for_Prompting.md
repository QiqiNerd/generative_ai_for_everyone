# Week 2 Lesson 5: Tips for Prompting

## 1. Introduction

Prompting is how we communicate with LLMs（大型语言模型） to guide their behavior. In this lesson, we explore:

- Practical tips for writing prompts
- How to improve prompt results through iteration
- Two important caution points

Whether you’re using a web UI or building a software application, these tips apply.

## 2. Tip 1: Be Detailed and Specific（提供详细具体的信息）

Use the **Fresh College Graduate analogy**（刚毕业大学生类比）— assume the LLM needs enough background info to perform the task.

### Example:

Weak prompt:  
> Help me write an email asking to be assigned to the Legal Documents project.

Better prompt:  
> I’ve applied to the Legal Documents project. We review legal content. I’ve used LLMs to generate legal copy before. Write a paragraph explaining why I’m a good fit.

**Why it works**:
- Provides **context**（上下文）
- Clarifies **desired output**（期望结果）

## 3. Tip 2: Guide the Model to Think Step-by-Step（引导模型逐步思考）

LLMs can follow **multi-step reasoning** if you guide them.

### Example:

Prompt:
> Brainstorm 5 rhyming names for a cat toy with relevant emojis.

Better prompt:
1. List 5 joyful words related to cats.  
2. For each word, create a rhyming name.  
3. Add a fun, relevant emoji to each.

This structure helps the model generate:
- purr → purr-twirl 🐱  
- whisker → whisker-whisper 🐾  
- feline → feline-beeline 🧶

## 4. Tip 3: Experiment and Iterate（尝试与迭代）

Prompting is **not about finding a perfect prompt** on your first try.

### Example:

1. Initial:  
   > Help me rewrite this.  
2. Still unclear:  
   > Correct any grammatical and spelling errors.  
3. Final:  
   > Correct grammatical/spelling errors and rewrite in a professional resume tone.

The key is to:

- Try a simple prompt
- Observe the response
- Adjust based on what’s missing

Prompting is **iterative**（迭代性的）— not perfection from the start.

## 5. Prompting Workflow

A simple framework:

1. **Initial Prompt** – Get started quickly
2. **Observe Output** – Is it close to what you want?
3. **Diagnose Gap** – What’s missing?
4. **Refine Prompt** – Add clarity or constraints
5. **Repeat** – Iterate until satisfied

📝 **Tip**: Don’t overthink the first prompt. You won’t “break the internet” by writing a flawed one.

## 6. Two Cautions

### 6.1 Confidential Information（敏感信息）

Before pasting **confidential data** into a public LLM interface, understand:

- Does the provider store prompts?
- Is your data being used for model training?

**Always review privacy policies**（隐私政策）.

### 6.2 Trust But Verify（审慎使用）

As shown in the earlier **lawyer example**（律师误用案例）:

- Don’t blindly trust LLM outputs
- Fact-check when using results for high-stakes contexts (e.g., legal, health)

## 7. Summary

Effective prompting means:

- Giving enough **context**
- Structuring prompts clearly
- Iterating toward better results
- Being cautious with sensitive data and high-stakes outputs

## 8. Next Steps

Try these tips using your preferred LLM tools. This concludes the main lessons of Week 2.

In the optional video, we’ll explore **image generation** and **diffusion models**（扩散模型）.

Next week, we’ll dive into building **LLM-powered projects**.

See you then!
