# LLM-Observability---LLM-as-a-Judge

LLM-as-a-Judge is an evaluation method to assess the quality of text outputs from any LLM-powered product, including chatbots, Q&A systems, or agents.

# Types of LLM judges : 

## 1. Pairwise comparison: give LLM two responses and ask to choose the better one. This lets you compare models, prompts, or configurations to see which performs best.

   ![image](https://github.com/user-attachments/assets/5ec2fba0-9ebe-4347-8c73-a09579d032c6)

## 2. Evaluation by criteria (reference-free): ask the LLM to assess a response or conversation based on tone, clarity, correctness, or other dimensions.

![image](https://github.com/user-attachments/assets/ee89bdc7-b980-4c93-b210-82c8fedd6dda)

## 3. Evaluation by criteria (reference-based): provide extra context, like a source document or reference, and ask the LLM to score the response.

   ![image](https://github.com/user-attachments/assets/41975633-f0b2-4587-a985-a3081fc50708)


# Implementation of LLM Judge : 

![image](https://github.com/user-attachments/assets/fd98b6dd-8d53-456e-a083-09cbdf4b3d4e)

## Step 1 : Install necessary libraries , import libraries and instantiate the Open AI key that will be leveraged

## Step 2 : Create the golden dataset 

## Step 3 : preview the golden dataset

![image](https://github.com/user-attachments/assets/438f3e35-5ffc-4485-9479-76e3ab5735f2)


![image](https://github.com/user-attachments/assets/a59dc317-4de4-424b-bbf0-80665e169541)

## Step 4 : Design the LLM Judge and generate report

Design a prompt in such way as to leverage Open AI's model (gpt-4o-mini) Compare the "target_response" with new_response semantically . It leverages gpt-4o-mini to classify the new_response as 
correct/incorrect with a reasoning . Please find below the marked screenshot of the output

![image](https://github.com/user-attachments/assets/9fb90082-ed85-4f61-9d75-8f8ac55e7c7c)

## Step 5 : Evaluate the LLM Judge 

![image](https://github.com/user-attachments/assets/e3123842-475a-46b5-a627-220c07fcf768)

![image](https://github.com/user-attachments/assets/9f01ca9c-e4d7-409e-80be-4716b269b991)

![image](https://github.com/user-attachments/assets/8478d2d1-c49c-472e-b65f-877623424615)

## Step 6 : Verbosity judge ( binary classification - concise / verbose ) definition and execution 

Design a prompt in such way as to leverage Open AI's model (gpt-4o-mini) to classify the new_responses into concise / verbose category ( concise / verbose definition is part of the prompt ) . Please find below the responses 

![image](https://github.com/user-attachments/assets/bb45a4e8-dbb7-4b4d-a2c2-0d9a152763af)

![image](https://github.com/user-attachments/assets/c67fd701-1879-405d-93fa-0791ce29d513)

Note : The report output can be extracted as .html , json or dictionary . Attached a sample report as .html file . Other prerequisites are to have an active Open AI API Key .

Happy Coding :) 
















