# RAT (Retrieval Augmented Thoughts)
## 🧠 What is RAT?
Retrieval Augmented Thoughts (RAT) is a method designed to enhance the reasoning capabilities of large language models (LLMs) by integrating external information retrieval into the reasoning process. Unlike traditional approaches that rely solely on the model's internal knowledge, RAT iteratively revises each step of a chain of thought (CoT) using relevant external information. This process aims to improve the factual accuracy and coherence of the model's reasoning, particularly in complex, long-horizon tasks.
## 🔄 Process Overview
1) Initial Zero-Shot CoT Generation: <br>
Given a task prompt, the LLM generates an initial chain of thought without any prior examples, simply by prompting it to "think step-by-step." <br>

2) Iterative Revision: <br>
For each step in the generated CoT, the model retrieves relevant external information—considering the task prompt, the current step, and previous steps—and revises the current thought step accordingly. <br>

3) Progressive Refinement: <br>
This process is repeated for each step in the CoT, progressively refining the reasoning path to enhance accuracy and coherence. <br>
## 🔧 Algorithmic Framework
The RAT framework operates as follows: <br>
Input: A task prompt. <br>
* Step 1: The LLM generates an initial zero-shot CoT. <br>
* Step 2: For each thought step: <br>
  * Retrieve relevant information based on the task prompt and the current and previous thought steps. <br>
  * Revise the current thought step using the retrieved information. <br>
* Output: A refined chain of thought with improved factual accuracy and logical coherence.
## ✅ Benefits of RAT
* Enhanced Reasoning: By incorporating external information, RAT allows LLMs to tackle complex tasks that require multi-step, context-aware reasoning.
* Reduced Hallucinations: The iterative revision process helps mitigate the generation of incorrect or fabricated information.
* Improved Task Performance: Empirical evaluations demonstrate that RAT significantly boosts performance across various tasks
![Process of RAT](https://raw.githubusercontent.com/MeysamAgah/RAT/refs/heads/master/pics/RAT.jpg)
