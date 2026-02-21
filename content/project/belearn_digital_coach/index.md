---
title: "BeLEARN: Conversational AI-Driven Coach"
summary: "Built and deployed a course-specific conversational AI tutor for university statistics, comparing Socratic and instructional tutoring strategies in a field experiment and deriving design guidelines for controllable LLM-based coaching systems."
tags:
  - AI and LLM Systems
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

## The Challenge

Students in introductory university statistics courses vary strongly in prior knowledge and study habits. Traditional support channels such as office hours, exercise sessions, and online forums do not scale to the volume and timing of student questions. Many learners need help that targets reasoning steps rather than just providing final answers. Large language models can offer personalized tutoring at scale, but uncontrolled generation conflicts with course-specific terminology, notation, and didactic sequencing.

## Approach and Methods

The project built a course-specific conversational AI tutor for an introductory statistics course at the University of Bern. The system used a checkpoint-based hybrid architecture that combined hard-coded constraints for terminology, references, and forbidden paraphrases with generative LLM components. This approach enforced strict adherence to course-specific notation (for example, exact use of partial eta-squared notation and specific R package arguments) while keeping the dialogue adaptive to different student paths. The tutor was deployed in a counterbalanced two-week field experiment where students were randomly assigned to receive either the Socratic or instructional mode first and then switched.

## Key Findings

The main finding was that real-world deployments require strong controllability. Course stakeholders expected strict adherence to the official wording and notation, while students expected the robustness of consumer AI platforms. The checkpoint-based hybrid architecture proved effective for enforcing terminology while keeping the dialogue adaptive. Differences between tutoring modes were not conclusive in the first week, while the second week showed a small trend favoring the Socratic mode. The study also highlighted challenges around model latency, exercise complexity requiring exact notation, and the limitations of a chatbot-only interface for structured statistical exercises.

## Implications

For educators considering LLM-based tutoring, the results suggest that controllability is the primary engineering challenge, not generation quality. A hybrid architecture that constrains the LLM at key decision points while allowing free-form dialogue in between proved more practical than relying on prompt engineering alone. The findings also indicate that a chatbot interface may not be sufficient for exercises requiring structured mathematical notation, pointing to the need for richer interaction modalities.

## Team and Funding

The project was led by Prof. Dr. Roman Rietsche (BFH, Institute for Digital Technology Management), with collaborators Dr. Andrew Ellis (BFH Virtual Academy), Prof. Dr. Lyle Ungar (University of Pennsylvania), and Andreas Goldi (University of St. Gallen). Dr. Boris Mayer (University of Bern, Institute of Psychology) provided the course content and co-designed the exercise integration. The project was funded by BeLEARN (January to December 2025).
