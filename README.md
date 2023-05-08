# [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/) by DeepLearning.AI.

**Course link:** [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)

## Introduction
- A lot of the powerful applications of LLMs can be achieved through API calls.
- There are two types of LLMs:
    - **Base LLMs** (e.g GPT-4)
        - These predict the next word based on the training data.
        - They are essentially highy advanced autocompletes.
        - They are trained on extremely large amounts of data (think all documented human knowledge).
    - **Instruction tuned LLMs** (e.g ChatGPT)
        - These try to follow instructions rather than just predict the next word.
        - To train this, you would start with a base LLM and train it further using *good* instruction-answer pairs.
        - You could also further fine tune it using reinforcement learning with human feedback (RLHF).
        - They can be trained to be helpful, honest, and harmless. This makes them more practical for real world applications.
- In this course we learn how to effectively interact with instruction tuned LLMs.
- It is useful to think of an LLM as a person, so be clear and specific when talking to it.

## Guidelines for Prompting
- **Write clear and specific instructions:**
    - Use delimiters (e.g ``, "", < >, `<tag> </tag>`, `:`) to clearly indicate distinct parts of the input.
    - Ask for a structured output (e.g `JSON`, `HTML`, custom structure).
    - Ask the model to check whether initial conditions are satisfied.
    - Give it a few sample promt-response pairs, this is known as few-shot prompting.
- **Give the model time to think:**
    - Break down and specify the speficic steps required to complete the task.
    - Instruct the model to double check itself before rushing to a conclusion ( this is a good way to prevent hallucinations).
- **Limitations:** The main limitation of LLMs is that they are prone to hallucinations (making up information that isn't real).
