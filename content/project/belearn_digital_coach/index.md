---
title: "BeLEARN: Conversational AI-Driven Coach"
summary: "Built and deployed a GPT-based Socratic tutor for a university statistics course, comparing tutoring strategies and deriving design guidelines for controllable LLM-based educational coaching systems. Funded by BeLEARN."
tags:
  - AI & LLM Systems
date: '2025-01-01'

external_link: ''

image:
  focal_point: Smart

links:
  - name: BeLEARN Project Page
    url: https://belearn.swiss/en/research-practice/projects/conversational-ai-driven-coach/
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''
---

# BeLEARN: Conversational AI-Driven Coach

## Scaling Personalized Tutoring with AI

Students in introductory university statistics courses vary strongly in prior knowledge and study habits. Traditional support channels, such as office hours, exercise sessions, and online forums, do not scale to the volume and timing of student questions. Many learners need help that targets reasoning steps rather than just providing final answers. Large language models can offer personalized tutoring at scale, but uncontrolled generation conflicts with course-specific terminology, notation, and didactic sequencing.

In this BeLEARN-funded project (January to December 2025), we built a course-specific conversational AI tutor for an introductory statistics course at the University of Bern. The system was designed to integrate tightly with the course's exercises, notation, and terminology while comparing two distinct tutoring strategies: Socratic tutoring, which guides students to discover answers through questions, and standard instructional explanations that provide direct teaching.

## Technical Architecture and Deployment

The tutor was implemented using a checkpoint-based hybrid architecture that combines hard-coded constraints for terminology, references, and forbidden paraphrases with generative LLM components. This approach allows the system to enforce strict adherence to course-specific notation while keeping the dialogue adaptive to different student paths. The system tracks student state across checkpoints, guiding learners through sub-tasks in a structured yet flexible manner. We deployed the tutor in a counterbalanced two-week field experiment where students were randomly assigned to receive either the Socratic or instructional mode first and then switched.

## Key Findings

The main technical finding was that real-world deployments require strong controllability. Course stakeholders expected strict adherence to the official wording and notation (for example, exact use of partial eta-squared notation and specific R package arguments), while students expected the robustness of consumer AI platforms. The checkpoint-based hybrid architecture proved effective for enforcing terminology while keeping the dialogue adaptive. In the field evaluation, differences between tutoring modes were not conclusive in the first week, while the second week showed a small trend favoring the Socratic mode. The study also highlighted challenges around model latency, exercise complexity requiring exact notation, and the limitations of a chatbot-only interface for structured statistical exercises.

## Team and Funding

The project was led by Prof. Dr. Roman Rietsche (BFH, Institute for Digital Technology Management), with collaborators Dr. Andrew Ellis (BFH Virtual Academy), Prof. Dr. Lyle Ungar (University of Pennsylvania), and Andreas Goldi (University of St. Gallen). Dr. Boris Mayer (University of Bern, Institute of Psychology) provided the course content and co-designed the exercise integration. The project was funded by BeLEARN (Bern Center for Digital Education).
