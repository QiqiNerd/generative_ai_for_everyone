# Week 3 Lesson 2–3: Coding Activity Notes

### Markdown Cell
## Prompting an LLM in code

### Markdown Cell
Instructions: 
1. For each of the two code cells below, click on the cell then hit Shift+Enter on your keyboard to run the code (or if on a mobile device, press 'play' button). 
2. Optionally edit the prompt, and try again!

### Markdown Cell
**Code cell 1:** Set up programming environment to use code to send prompts to OpenAI's cloud-hosted service.

### Code Cell
```python
import openai
import os

openai.api_key = os.getenv("OPENAI_API_KEY")

def llm_response(prompt):
    response = openai.ChatCompletion.create(
        model='gpt-3.5-turbo',
        messages=[{'role':'user','content':prompt}],
        temperature=0
    )
    return response.choices[0].message['content']
```

### Markdown Cell
**Code cell 2:** Define a prompt that will classify the sentiment of a restaurant review.

### Code Cell
```python
prompt = '''
    Classify the following review 
    as having either a positive or
    negative sentiment:

    The banana pudding was really tasty!
'''

response = llm_response(prompt)
print(response)
```
