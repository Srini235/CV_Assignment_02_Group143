# CV_Assignment_02_Group143
Computer Vision subject Assignment Group 143 from BITS Pilani students
Problem statement 4: Fine-Tuning a Text-to-Image Model Using Crowd-Sourced Text–
Image Pairs
Problem Statement: You are given a small set of crowd-sourced images containing text, paired with 
corresponding text prompts. Your task is to fine-tune a pre trained text-to-image model so that it can 
generate images that visually resemble real operational text images when given a text prompt.
Objective:
Fine-tune a small text-to-image generation model to generate simple, readable text images using crowd-sourced text–image pairs collected from real-world operational contexts.
The goal is to understand:
● Domain shift from synthetic to real data
● Model adaptation using limited, noisy samples
● Practical constraints of fine-tuning generative models on Colab
Model Selection: Stable Diffusion (v1.5 or v1.4) with LoRA fine-tuning
● Fine-tune attention layers only
● Freeze base model
● Use diffusers + peft
Evaluation Criteria
1.Qualitative Evaluation
o Visual clarity of generated text
o Font and spacing realism
o Background consistency
2.Quantitative Evaluation (Mandatory)
o OCR-based readability test:
text → generated image → OCR → recovered text
o Metrics:
Exact string match
Character accuracy
