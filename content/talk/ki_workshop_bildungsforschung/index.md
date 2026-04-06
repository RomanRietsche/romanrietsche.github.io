---
title: 'Generative KI in der Bildungsforschung'
type: event
location: 'University of Fribourg, Switzerland'
summary: 'Prompt Engineering for Educational Research'
date: '2026-04-09'
tags: [ki_workshop_bildungsforschung]
draft: false
---

# Workshop Prompts

Below you will find the prompts used in this workshop for the Fakultät für Erziehungs- und Bildungswissenschaften.

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
| **Context and Relevance**   | - Define Role (e.g., "You are an educational researcher specializing in self-regulated learning.")<br>- Audience and Purpose (e.g., "Write for first-year teacher education students preparing their bachelor thesis.") |
| **Separating in Smaller Packages** | - Include Step-by-Step Instructions (e.g., "First, summarize the theoretical framework. Next, derive testable hypotheses.") |
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
Example: "You are an educational researcher specializing in mixed-methods studies in higher education."

Objective (O)
Articulate the goal of the conversation.
Example: "Help me design a 4-week intervention study to improve self-regulated learning in first-year university students."

Details (D)
Specific details about the objective.
Example: "The cohort is 120 students from mixed STEM and humanities programs, the intervention runs in an online module, and the primary outcome is the MSLQ (Motivated Strategies for Learning Questionnaire) self-regulation subscale, measured pre and post."

Examples (E)
Provide examples of ideal results.
Show the AI a few examples of what a good intervention design or hypothesis statement looks like.

Sense Check (S)
Confirm understanding.
Example: "Before drafting the study design, do you have any questions about the learning context, the cohort, or the constraints of the online module?"
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

You are an expert in educational research and learning sciences. Develop a series of multiple-choice questions to assess understanding of "prompt techniques" among doctoral students and researchers attending a workshop at the Fakultät für Erziehungs- und Bildungswissenschaften.

# Task
Ensure that the questions are clear and focus on how prompt engineering can be applied in educational research, instructional design, qualitative coding, survey construction, and academic writing.
Each question should contain one correct answer and several plausible distractors.
Look for a mix of difficulty levels to properly assess the different levels of understanding.

# Steps
1. Identify the main topics and objectives of the presentation on "Prompt Engineering" as it applies to educational research and Bildungsforschung.
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

**Question**: A doctoral student wants to use an LLM to support open coding of 30 semi-structured interviews on teacher beliefs. Which prompting strategy is most effective?

a) "Code these interviews"
b) "You are a qualitative researcher trained in reflexive thematic analysis. For each interview excerpt below, propose 3-5 candidate inductive codes, give a one-sentence definition for each code, and flag any excerpt where the meaning is ambiguous so I can review it manually." (Correct answer)
c) "Tell me what these interviews are about"
d) "Summarize these interviews"

...

# Notes
- Include questions that address definitions, practical applications in educational research, and potential pitfalls in "prompt engineering" (e.g., hallucinations in literature reviews, sycophancy when refining hypotheses).
- Consider scenario-based questions involving survey design, qualitative coding, instructional design, and academic writing for educational journals.
- Avoid excessive jargon unless it has been explicitly covered in the presentation.

```

<br>

---

<br>

# Few-Shot Prompt: Educational Research LinkedIn-Post

```
Example 1
Topic: Evidence-Based Teaching
"Not every classroom innovation actually moves the needle on learning. 📊 Decades of meta-analyses show that some of the most hyped methods have effect sizes close to zero, while unglamorous practices like formative feedback and spaced retrieval consistently outperform. As educational researchers, our job is to translate this evidence into something teachers can use on a Monday morning. Which 'obvious' classroom practice were you most surprised to see fail in the data?"

Example 2
Topic: Generative AI in the Classroom
"Generative AI is now sitting in every student's pocket, whether universities authorize it or not. 🤖 The interesting research question is no longer 'should we allow it' but 'which task designs make AI use a learning accelerator instead of a shortcut around thinking'. Early findings suggest that prompts requiring critique, comparison and self-explanation preserve learning gains far better than prompts asking for finished products. What task redesigns have you seen that genuinely raise the cognitive bar?"

Example 3
Topic: Equity in Higher Education
"Access is not the same as belonging. 🎓 First-generation students often clear the admissions hurdle only to encounter a hidden curriculum no one teaches them: how to talk to professors, how to ask for help, how to read between the lines of an assignment brief. Closing this gap is not a matter of motivation, it is a matter of design. What is one structural change your institution made that actually moved equity outcomes?"

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

# Prompt Techniques Formula

> **As [ROLE] perform [TASK] in [FORMAT]: insert unique data**

| **Role**                                  | **Task / Aim**                                  | **Format**                  |
|-------------------------------------------|-------------------------------------------------|-----------------------------|
| Educational Researcher                    | Derive testable hypotheses from a theory        | Numbered list               |
| Learning Scientist                        | Design a formative assessment intervention      | Structured study protocol   |
| Survey Methodologist                      | Critique a questionnaire for construct validity | Annotated table             |
| Qualitative Researcher                    | Propose inductive codes for interview excerpts  | Codebook with definitions   |
| Editor of Educational Research Review     | Condense a literature review                    | Table / Chart               |
| Teacher Educator                          | Draft a workshop outline for in-service training| Lesson plan                 |

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
