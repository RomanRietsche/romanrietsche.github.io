---
title: DigiBot
summary: Developed and evaluated an AI chatbot that personalizes standardized digital competence assessments based on individual user profiles, revealing that adaptive question generation improves relevance for advanced users while beginners prefer standardized formats.
tags:
  - AI and LLM Systems
date: '2024-01-01'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  focal_point: Smart

links:
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''
---

## The Challenge

Standardized digital skills assessments based on frameworks such as the European DigComp often feel disconnected from the daily work of the person being tested. A cybersecurity question written for a generic audience may not resonate with a marketing professional, reducing engagement and potentially misrepresenting actual competence levels. At the same time, manually creating role-specific assessment variants for every profession is impractical. The question was whether generative AI could adapt standardized assessment items to individual user contexts while preserving measurement consistency.

## Approach and Methods

DigiBot was implemented as a two-stage conversational chatbot. In the first stage, the bot engaged users in a brief profiling conversation, asking about their job role, daily tasks, and self-assessed digital skills. In the second stage, the system used ChatGPT to transform standardized DigComp assessment questions to match the user's professional context. For instance, a marketer received questions about identifying fake customer inquiries, while an IT administrator received questions focused on email security protocols. Users were then shown both original and personalized versions and asked to evaluate each on relevance, clarity, and preference.

## Key Findings

The evaluation revealed a clear trade-off between clarity and relevance. Original standardized questions scored higher on clarity and ease of understanding, while AI-personalized questions scored higher on contextual relevance and detail. User preferences split along competence levels: beginners preferred the simpler, standardized questions, while advanced users appreciated the deeper, profession-specific AI-generated versions. Personalized questions were most valued when they accurately reflected the user's actual professional background, suggesting that profiling quality is a critical upstream factor.

## Implications

The results suggest that a one-size-fits-all approach to AI personalization in assessment is insufficient. Effective personalization needs to adapt not only the question content but also the complexity level to the user's proficiency. For organizations deploying digital skills assessments at scale, a hybrid approach that offers standardized questions as a baseline with optional AI-personalized variants based on user profile and competence level appears most promising.

## Team and Funding

The project was conducted at the Bern University of Applied Sciences (BFH), Institute for Digital Technology Management, led by Prof. Dr. Roman Rietsche. The project was funded through BFH's Humane Digital Transformation strategic thematic field.
