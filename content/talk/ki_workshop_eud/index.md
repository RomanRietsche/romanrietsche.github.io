---
title: 'KI-Workshop Ernährung und Diätetik (EuD)'
type: event
location: 'Bern University of Applied Sciences'
summary: 'Prompt Engineering for EuD'
date: '2026-03-16'
tags: [ki_workshop_eud]
draft: false
---

# Workshop Prompts

Below you will find the prompts used in this workshop.

<br>

---

# Links

https://tiktokenizer.vercel.app

<br>

---

<br>

# How to Craft Effective Prompts: Key Principles

| **Category**                | **Guidelines**                                                                                 |
|-----------------------------|-----------------------------------------------------------------------------------------------|
| **Clarity and Understanding** | - Use delimiters for clarity (e.g., `### text ###`)<br>- Consider providing examples for correct output (few-shot prompting)                        |
| **Specificity and Detailing** | - Specify desired output format<br>- Specify output length. Think in natural quantities, like "a dozen"                          |
| **Context and Relevance**   | - Define Role (e.g., "You are a registered dietitian.")<br>- Audience and Purpose (e.g., "Write for patients with newly diagnosed type 2 diabetes.") |
| **Separating in Smaller Packages** | - Include Step-by-Step Instructions (e.g., "First, assess the nutritional profile. Next, suggest meal alternatives.") |
| **Conditioning for Questions** | - Ask me questions for clarification |
| **Task-list** | - For state tracking use a task-list |

<br>

---

<br>

# RODES Framework

Use this framework for the 7-minute exercise.

```
Role (R)
Define the role the AI is playing.
Example: "You are a registered dietitian specializing in clinical nutrition."

Objective (O)
Articulate the goal of the conversation.
Example: "Help me create a 7-day meal plan for a patient with iron-deficiency anemia."

Details (D)
Specific details about the objective.
Example: "The patient is vegetarian, lactose-intolerant, and needs at least 18mg iron per day. Include bioavailability-enhancing food combinations."

Examples (E)
Provide examples of ideal results.
Show the AI a few examples of what a good result looks like.

Sense Check (S)
Confirm understanding.
Example: "Before creating the meal plan, do you have any questions about the patient's dietary restrictions?"
```

<br>

---

<br>

# Markdown Language

```
Heading:        # H1  /  ## H2  /  ### H3
Bold:           **bold text**
Italic:         *italicized text*
Blockquote:     > blockquote
Ordered List:   1. First item  2. Second item  3. Third item
Unordered List: - First item  - Second item  - Third item
Code:           `code`
Horizontal Rule: ---
```

<br>

---

<br>

# Example System Prompt

```

You are an expert in nutrition science and dietetics education. Develop a series of multiple-choice questions to assess understanding of "prompt techniques" among nutrition and dietetics professionals attending a workshop.

# Task
Ensure that the questions are clear and focus on how prompt engineering can be applied in nutrition counseling, meal planning, patient communication, and food science contexts.
Each question should contain one correct answer and several plausible distractors.
Look for a mix of difficulty levels to properly assess the different levels of understanding.

# Steps
1. Identify the main topics and objectives of the presentation on "Prompt Engineering" as it applies to nutrition and dietetics work.
2. Develop questions that address these key topics and ensure that they assess understanding, application and analysis where possible.
3. Develop a range of multiple-choice options for each question, including one correct answer and three distractor options.
4. Review the questions for clarity and relevance to the presentation material.

# Output format
Each question should be followed by four options, where:
- One option is labeled as the correct answer.
- Each option is marked with a letter (a, b, c, d).

Question: [Text of the question]
  a) Option 1
  b) Option 2
  c) Option 3 (correct answer)
  d) Option 4

# Examples

**Question**: A dietitian wants to use AI to simplify a complex lab report for a patient. Which prompting strategy is most effective?

a) "Simplify this report"
b) "You are a registered dietitian. Rewrite the following lab report in plain language for a patient with limited health literacy. Explain what each value means for their nutrition." (Correct answer)
c) "Translate this to simple words"
d) "Make this easier"

...

# Notes
- Include questions that address definitions, practical applications in nutrition/dietetics, and potential pitfalls in "prompt engineering."
- Consider scenario-based questions involving meal planning, patient education, and dietary analysis.
- Avoid excessive jargon unless it has been explicitly covered in the presentation.

```

<br>

---

<br>

# Few-Shot Prompt: Nutrition & Dietetics LinkedIn-Post

```
Example 1
Topic: Sustainable Nutrition
"What we eat shapes not only our health but our planet. 🌱 Shifting towards plant-forward diets can reduce food-related emissions by up to 50%. As nutrition professionals, we have the responsibility to guide evidence-based choices that nourish people and protect ecosystems. What is one sustainable swap you recommend to your clients?"

Example 2
Topic: Personalized Nutrition
"One size does not fit all when it comes to nutrition. 🧬 Advances in nutrigenomics and microbiome research are transforming how we design dietary interventions. Personalized nutrition plans that account for genetics, lifestyle, and individual metabolism are the future of dietetics. How are you integrating personalized approaches into your practice?"

Example 3
Topic: Food Literacy
"Understanding food labels should not require a science degree. 📋 Yet many consumers struggle to interpret nutritional information. As dietitians, we bridge this gap by translating complex data into actionable advice. What is the most common misconception about food labels you encounter?"

Now write a LinkedIn post for the topic: <<INSERT YOUR TOPIC>>
```

<br>

---

<br>

# Framework-First Mindset

```
# 1. Define Five Quantitative Measures
Define five clear, quantitative criteria to objectively evaluate the quality of the text. These could be:

- **Clarity** (How understandable is the text? Scale 1-10)
- **Structure** (How logical and clear is the structure? Scale 1-10)
- **Persuasiveness** (How strong is the argumentation? Scale 1-10)
- **Reader Engagement** (How well is the reader emotionally addressed? Scale 1-10)
- **Linguistic Quality** (How precise and appealing is the wording? Scale 1-10)

---

# 2. Evaluate the Original Text
Rate the original text according to the five defined criteria.

---

# 3. Improve the Text
Revise the text to improve all five measures. Focus on:

- More precise formulations for clarity.
- A logical and well-structured layout.
- Stronger arguments and evidence to increase persuasiveness.
- A more active and emotional engagement of the reader.
- A varied but clear language.

---

# 4. Evaluate the Revised Text
Measure the quality of the improved text again.

---

# 5. Sentence-by-Sentence Analysis
Compare sentence by sentence the old with the new text and show specifically how the measures improved.
```

<br>

---

<br>

# Complex Prompt to Understand a New Topic

-> Copy each step one after the other into ChatGPT, Claude, Gemini, etc.

```
# Task: I want to understand "<<INSERT TOPIC>>"

## Initial Question Generation

**Step 1**

Generate 10 initial questions about the topic, aiming for a mix of open-ended and closed questions. This variety encourages a broad exploration while also gathering specific details.

**Guideline**

Ensure questions cover the what, why, how, and implications related to the topic to ensure a comprehensive initial overview.
```

```
## Thematic Clustering and Optimization

**Step 2**

Determine an "optimal amount" of themes for clustering the questions. Use thematic analysis principles, focusing on patterns and concepts that recur across the initial questions.

**Step 3**

Cluster the initial questions into themes based on the identified patterns. Aim for distinct yet comprehensive thematic clusters.
```

```
## Reflective Expansion of Questions

**Step 4**

Review each theme cluster to identify gaps or emerging insights. Add two more questions for each theme to ensure thorough coverage. For each added question, provide a rationale based on identified gaps or new insights.

**Step 5**

Output the final clusters with the set of questions.
```

```
## Detailed Question Answering with a Structured Template

**Step 6**

Answer each question in 200 words using a specific template. Tailor the template slightly for questions (e.g., theoretical vs. practical) to allow nuanced responses. The template should cover why the question is important, what information or actions are needed, and which methods will be used, including examples or analogies. Emphasize reasoning before providing the answer, using active inference. Think step-by-step.

**Step 7**

After answering a question, ask permission to proceed to the next, ensuring a methodical and reflective process.
```

<br>

---

<br>

# Chain-of-Thoughts (CoT)

```
Let's work this out in a step by step way to be sure we have the right answer.
Provide reasoning first and then the answer.
```

<br>

---

<br>

# Prompt Techniques Formula

> **As [ROLE] perform [TASK] in [FORMAT]: insert unique data**

| **Role**                        | **Task / Aim**                 | **Format**                  |
|---------------------------------|--------------------------------|-----------------------------|
| Registered Dietitian         | Create a meal plan | Table with macros                        |
| Clinical Nutritionist             | Summarize a patient case            | Bullet points              |
| Food Science Researcher                 | Analyze nutrient interactions                     | Summary                    |
| Editor from Journal of Nutrition  | Condense literature review               | Table/Chart                |
| Public Health Nutritionist | Draft dietary guidelines           | Structured report                              |

<br>

---

<br>

# References

Agarwal, R., Singh, A., Zhang, L. M., Bohnet, B., Chan, S., Anand, A., Abbas, Z., Nova, A., Co-Reyes, J. D., Chu, E., Behbahani, F., Faust, A., and Larochelle, H. 2024. Many-Shot In-Context Learning, arXiv. (http://arxiv.org/abs/2404.11018).

Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., Neelakantan, A., Shyam, P., Sastry, G., Askell, A., Agarwal, S., Herbert-Voss, A., Krueger, G., Henighan, T., Child, R., Ramesh, A., Ziegler, D. M., Wu, J., Winter, C., Hesse, C., Chen, M., Sigler, E., Litwin, M., Gray, S., Chess, B., Clark, J., Berner, C., McCandlish, S., Radford, A., Sutskever, I., and Amodei, D. 2020. "Language Models Are Few-Shot Learners," , May 28. (http://arxiv.org/pdf/2005.14165v4).

Bsharat, S. M., Myrzakhan, A., and Shen, Z. 2023. Principled Instructions Are All You Need for Questioning LLaMA-1/2, GPT-3.5/4. (https://doi.org/10.48550/ARXIV.2312.16171).

Schulhoff, Sander, Ilie, M., Balepur, N., et al. 2024. The Prompt Report: A Systematic Survey of Prompting Techniques, arXiv. (http://arxiv.org/abs/2406.06608).

Wei, J., Wang, X., Schuurmans, D., Bosma, M., Ichter, B., Xia, F., Chi, E., Le, Q., and Zhou, D. 2022. "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models," arXiv. (https://doi.org/10.48550/arXiv.2201.11903).

Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. 2022. "ReAct: Synergizing Reasoning and Acting in Language Models," arXiv. (https://doi.org/10.48550/arXiv.2210.03629).
