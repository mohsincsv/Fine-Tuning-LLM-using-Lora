# Model Fine-Tuning on 7b Model with LoRa Integration

Note: Due to GPU limitations and memory issues, thorough testing and evaluation of the model's performance were not feasible.

I've studied and got help from the following two articles:

1) [Practical Tips for Finetuning LLMs Using LoRA (Low-Rank Adaptation)](https://magazine.sebastianraschka.com/p/practical-tips-for-finetuning-llms)
2) [Fine-Tuning Tutorial: Falcon-7b LLM To A General Purpose Chatbot](https://www.labellerr.com/blog/hands-on-with-fine-tuning-llm/)

## Objective: 
This project focuses on fine-tuning a large-scale pre-trained model with at least 7 billion parameters, incorporating LoRa (Long Range) technology for efficient and effective adaptation. This README details the process and outcomes of fine-tuning the Falcon-7b Large Language Model (LLM) using the QLoRA technique, focused on creating a mental health chatbot. 

## Tasks Overview

### 1. Select a 7b Model [10 points]
- Model Selection: Chose the Falcon-7b LLM for its extensive training on a large corpus and high parameter count, suitable for complex tasks like a mental health chatbot.
- Justification: Falcon-7b's capacity and flexibility make it ideal for domain-specific adaptation, essential for sensitive and nuanced topics like mental health.\

### 2. Define Fine-Tuning Objectives [15 points]
- Objectives: Aimed to build a mental health chatbot that offers reliable information and emotional support, leveraging the Falcon-7b's advanced language understanding capabilities.
- Data Specification: Used a curated dataset comprising high-quality conversations related to mental health, sourced from various reputable healthcare websites and blogs.

### 3. Data Preparation for Fine-Tuning [15 points]
- Data Processing: Prepared a dataset of 172 conversational pairs, ensuring anonymization and preprocessing to remove unwanted characters and maintain relevance.
- Considerations: Emphasized the importance of high-quality, contextually rich data for effective training in the mental health domain.

### 4. Fine-Tuning Process [20 points]
- Procedure Outline: Utilized QLoRA for efficient fine-tuning, focusing on specific modules within Falcon-7b, and configured training parameters tailored to the task.
- Mitigating Overfitting: Addressed potential overfitting and memory issues by employing quantization techniques and careful management of training parameters.

### 5. LoRa Integration [20 points]
- Integration Strategy: Integrated Low-Rank Adapters (LoRA) to fine-tune the model effectively without extensively altering the pre-trained weights, preserving the original model's strengths.
- QLoRA Application: Applied QLoRA for reducing memory footprint and enabling fine-tuning on consumer-grade hardware without compromising model performance.


### 6. Coding Implementation [20 points]
- Implemented the fine-tuning process in Python, using libraries like trl, transformers, accelerate, and bitsandbytes for effective model training and adaptation.

### 7. Testing and Evaluation [15 points]
- I could evaluate the fine-tuned model's performance by comparing its responses to those of original model, focusing on coherence and context.
