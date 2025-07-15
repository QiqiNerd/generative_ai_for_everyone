# Lesson 1. Concerns About AI

# 1.1 The Global Spread of Generative AI

Generative AI has rapidly become accessible worldwide, enabling people to generate high-quality essays, images, and audio with ease. However, alongside these powerful capabilities have come significant public anxieties. These concerns are not only technological but also deeply rooted in broader societal issues such as:

- Environmental degradation
- Distrust in institutions
- Social inequality
- Uncertainty about the future

AI, as a transformative and powerful tool, has absorbed much of this global anxiety and sparked new ethical, economic, and existential debates.

# 1.2 Amplifying Human Biases

One major concern is whether Large Language Models (LLMs, 大型语言模型) might amplify humanity’s worst qualities. Since LLMs are trained on internet text, they inevitably absorb both the best and worst of human behavior—including biases, prejudices, and misconceptions.

### Examples of Bias:
- Gender stereotypes: An LLM might assume that a "CEO" is a "man" because of patterns in historical data.
- Professional roles: Biases such as assuming nurses are female and surgeons are male have been observed.

This is not entirely surprising—training data reflects the past and present, which are not free from social injustice. However, ideally, LLMs should embody a **vision of the future**—one that is **fairer, less biased, and more inclusive**.

### Solution: Reducing Bias with RLHF

LLMs are becoming less biased through techniques like:

- **Fine-tuning (微调)**: Adjusting the model with curated datasets.
- **Reinforcement Learning from Human Feedback (RLHF, 来自人类反馈的强化学习)**: Aligning AI output with human values.

#### How RLHF Works:
1. **Prompting**: Present queries to the LLM (e.g., "The ___ was a CEO") and collect responses.
2. **Scoring by humans**: Label responses from desirable (e.g., “man” and “woman”) to undesirable (e.g., “airplane” or slurs).
3. **Reward model (奖励模型)**: A supervised learning model is trained to predict these scores.
4. **Self-improvement**: The LLM uses the reward model to generate better, more aligned responses.

**Outcome**: RLHF reduces LLM biases related to gender, race, religion, and helps LLMs become safer and more respectful.

# 1.3 Will AI Take Our Jobs?

Another widespread concern is the economic impact of AI:  
**Will AI replace human workers?**

### Case Study: Radiology

In 2016, AI pioneer **Geoff Hinton** famously predicted that AI would replace radiologists within five years. However, this has not happened. Not a single radiologist has lost their job due to AI. Why?

#### Two Key Reasons:
1. **Task Complexity**: Interpreting X-rays is harder than initially believed.
2. **Multi-role nature of jobs**: Radiologists perform ~30 tasks (according to O*NET), not just image analysis.

Examples of radiologist tasks:
- Operating imaging equipment
- Communicating with patients
- Handling complications
- Documentation

### Insight from Prof. Curtis Langlotz (Stanford):
> “AI won't replace radiologists. But radiologists who use AI will replace those who don't.”

This principle may apply across many professions. While some routine tasks may be automated, **AI will augment rather than replace** most jobs.

### Historical Parallel:
Every major wave of technology—from steam engines to computers—has displaced some jobs but created many more. Similarly, AI can drive **economic growth** and **create new roles**, especially in areas focusing on innovation rather than cost-cutting.

# 1.4 Will AI Destroy Humanity?

This is perhaps the most extreme concern:  
**Could AI lead to human extinction?**

### Examples of AI Failures:
- **Autonomous vehicles**: Crashes leading to fatalities.
- **Trading algorithms**: The 2010 stock market flash crash.
- **Criminal justice AI**: Biased sentencing outcomes.

While software errors can have serious consequences, **there is currently no concrete, specific scenario** demonstrating how AI could **cause human extinction**.

### Types of Existential Fears:
1. **Malicious Use**: AI used by bad actors (e.g., bioweapons).
2. **Unintentional Harm**: AI harming humanity by accident (e.g., environmental collapse due to neglectful decisions).

Most arguments boil down to speculative logic:  
> “It could happen because AI is new and powerful.”

But this logic applies to all new technologies and does not prove real risk.

### Analogy: Airplanes
In the early days, airplanes caused many deaths. Today, flying is among the safest modes of travel—thanks to better technology and strict regulations.

> We learned, improved, and built **safer systems**.

Similarly, we are learning how to **control AI**, and it is becoming safer over time.

# 1.5 AI as a Tool to Fight Existential Risks

Paradoxically, AI may be **vital** in addressing actual existential risks:

- **Climate change**: Modeling, prediction, and mitigation.
- **Pandemics**: Early detection and vaccine development.
- **Asteroids**: Surveillance and risk assessment.

Thus, AI might actually **increase humanity’s odds of long-term survival**, rather than reduce them.

# 1.6 Fear of AGI: The Root of Many Concerns

The deepest source of uncertainty may be the question:

> **When will we reach AGI (Artificial General Intelligence, 通用人工智能)?**

AGI refers to an AI that can perform **any intellectual task** that a human can.

Because no one knows when (or if) this will occur, predictions about the future impact of AI are full of ambiguity. This uncertainty drives both **hope and fear**.

Andrew Ng concludes that **AI's potential to help humanity is enormous**, and while concerns are valid, **continuous learning, regulation, and responsible development** will guide us toward a future where AI benefits all.
