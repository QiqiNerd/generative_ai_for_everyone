# Week 2 Lesson 6: Image Generation

## 1. Introduction

While text generation has seen the widest adoption, **image generation**（图像生成）is an equally exciting aspect of **generative AI**（生成式人工智能）. In this lesson, we explore:

- How image generation works
- What diffusion models are
- The role of **supervised learning**（监督学习） in this process

## 2. Multimodal Models（多模态模型）

Some generative AI models can generate both:

- Text
- Images

These are known as **multimodal models** because they handle **multiple modalities**（多种数据模态）.

## 3. Image Generation with Prompts

Given a **prompt**（提示词）, a generative model can create:

- A human face that never existed
- A futuristic city
- A robot design

How is this done? Mostly through a method called **diffusion modeling**（扩散模型）.

## 4. How Diffusion Models Work

Diffusion models are trained on **large-scale image datasets**（大规模图像数据集） found online.

### 4.1 Noise Process

1. Start with a clean image (e.g., an apple).
2. Add increasing levels of **noise**（噪声） over several steps.
3. Eventually reach an image of **pure noise**.

This process simulates how to destroy an image progressively.

### 4.2 Learning to Denoise with Supervised Learning

- Training pairs:  
  - Input A: Noisy image  
  - Output B: Slightly less noisy version

- The model learns to:
  - Turn noisy images into cleaner ones
  - Reverse the noise process gradually

This step is repeated across **millions of image pairs**.

## 5. Generating a New Image from Noise

At inference time:

1. Start with **pure noise**
2. Use the trained model to **denoise iteratively**
3. After ~100 steps, the final image emerges

Example:

- Initial noise → vague fruit shape → blurry watermelon → realistic watermelon

## 6. Adding Prompts for Control

To control what image gets generated, training is modified:

- Each image is paired with a **text caption**（文本描述）
  - E.g., “red apple”

### Modified Training:

- Input A: Noisy image + prompt “red apple”
- Output B: Less noisy image of a red apple

This teaches the model to **associate text with image features**.

## 7. Inference with Prompts

Example: Generate a **green banana**

1. Start with random noise
2. Input: Noise + prompt “green banana”
3. Model denoises image in steps:
   - Step 1: greenish blob
   - Step 2: blurry green banana
   - Step 3: clear green banana

Thus, prompts guide the model through each **denoising step** to form the final image.

## 8. Summary

- Image generation is powered by **diffusion models**
- Core mechanism: supervised learning on noisy/clean image pairs
- Prompts guide generation with **semantic control**
- Models learn to create art, scenes, and objects from scratch

This concludes our optional lesson on image generation.

## 9. Looking Ahead

Next week, we’ll explore **real-world applications** and how to **build projects** using generative AI.

See you then!
