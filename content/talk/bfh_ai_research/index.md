---
title: "Workshop: AI in Research"
type: event
location: Bern University of Applied Sciences
#summary: “Enhancing Student Performance Through Technology-Mediated Formative Feedback in Large Scale University Lectures,” Department of Management, Technology, and Economics, ETH Zurich.
#abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-11-13'
#date_end: '2030-06-01T15:00:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
#publishDate: '2017-01-01T00:00:00Z'

#authors: []
tags: [bfh_ai_research]
draft: false  # Ensure it's published

# Is this a featured talk? (true/false)
#featured: false

#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
#  focal_point: Right

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
#url_code: ''
#url_pdf: ''
#url_slides: ''
#url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
#projects:
#  - example

#{{% callout note %}}
#Click on the **Slides** button above to view the built-in slides feature.
#{{% /callout %}}

#Slides can be added in a few ways:

#- **Create** slides using Wowchemy's [_Slides_](https://wowchemy.com/docs/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
#- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
#- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://wowchemy.com/docs/writing-markdown-latex/).

#Further event details, including [page elements](https://wowchemy.com/docs/writing-markdown-latex/) such as image galleries, can be added to the body of this page.


---

# Prompts

## How to Craft Effective Prompts: Key Principles

| **Category**                | **Guidelines**                                                                                 |
|-----------------------------|-----------------------------------------------------------------------------------------------|
| **Clarity and Understanding** | - Use delimiters for clarity (e.g., `### text ###`)                                        |
|                             | - Consider providing examples for correct output (few-shot prompting)                        |
| **Specificity and Detailing** | - Specify desired output format                                                              |
|                             | - Specify output length. Think in natural quantities, like "a dozen"                          |
|                             | - Be specific and precise                                                                     |
| **Context and Relevance**   | - Define Role (e.g., "You are a translator.")                                                |
|                             | - Audience and Purpose (e.g., "Translate for an Italian audience looking for fresh products.") |
| **Step-by-Step Guidance**   | - Include Step-by-Step Instructions (e.g., "First, translate to Italian. Next, make it catchy.") |
| **Conditioning for Accuracy** | - Condition the model's responses on the context to get more accurate results                |
|                             |   (e.g., "Base your translation on the following dictionary where appropriate: `{dictionary}`") |




## Steps to Create Effective ChatGPT Prompt

1. **Identify the purpose and focus of the conversation.**

2. **Use specific and relevant language** (e.g., "Act as...").

3. **Avoid open or overly general prompts.**

4. **Review and revise your prompt.**

### Example Proposal Writing

> “Imagine you are writing a scientific proposal for receiving funding for educational technology in the canton of Bern in Switzerland. Act as a research scientist at the intersection of HCI and educational technology. Please imagine the following proposal summary: '…' Please create a specific timeline with milestones for the project and arrange them for the quarters in 2024. Study 1 will happen in Q2 and Study 2 in Q4.”

---

## Example Phrases for Prompts:

Critical self-reflect …
Improve it by 100% …
You get 100 dollar tips when you improve it…
Convince the reader …

*Improve Text:*
Create, at first, five quantitative measures, and rate your text on them
Then, revise the text
Measure the new text again, and show sentence by sentence how the measures improve
Provide reasoning first

## Complex Prompt to Understand a New Topic

-> copy each step one after the other into chatGPT, Claude, Gemini, etc.

I want to understand “prompt engineering”

### Initial Question Generation:
**Step 1**: Generate 10 initial questions about the topic, aiming for a mix of open-ended and closed questions. This variety encourages a broad exploration while also gathering specific details.  
**Guideline**: Ensure questions cover the what, why, how, and implications related to the topic to ensure a comprehensive initial overview.  
*Ask for my permission to go to the next step!*

### Thematic Clustering and Optimization:
**Step 2**: Determine an "optimal amount" of themes for clustering the questions. Use thematic analysis principles, focusing on patterns and concepts that recur across the initial questions.  
**Step 3**: Cluster the initial questions into themes based on the identified patterns. Aim for distinct yet comprehensive thematic clusters.  
*Ask for my permission to go to the next step!*

### Reflective Expansion of Questions:
**Step 4**: Review each theme cluster to identify gaps or emerging insights. Add two more questions for each theme to ensure thorough coverage. For each added question, provide a rationale based on identified gaps or new insights.  
**Step 5**: Output the final clusters with the set of questions.  
*Ask for my permission to go to the next step!*

### Detailed Question Answering with a Structured Template:
**Step 6**: Answer each question in 200 words using a specific template. Tailor the template slightly for questions (e.g., theoretical vs. practical) to allow nuanced responses.  
The template should cover why the question is important, what information or actions are needed, and which methods will be used, including examples or analogies. Emphasize reasoning before providing the answer, using a structured step-by-step approach.  
**Step 7**: After answering a question, ask permission to proceed to the next, ensuring a methodical and reflective process.  
*Ask for my permission to go to the next step!*

### Iterative Reflection and Summary:
**Step 8**: Conduct a reflective review of all responses after completing the answers. Summarize critical insights, contradictions, and new questions that have emerged. This step fosters a deeper understanding and may highlight further areas of inquiry.

---

## Prompt Techniques – Using Formula

**Acting as [ROLE] perform [TASK] in [FORMAT]: insert unique data**

| **Role**                        | **Task / Aim**                 | **Format**                  |
|---------------------------------|--------------------------------|-----------------------------|
| • Expert Science Writer         | • Formulate research questions | • PDF                        |
| • Ronald C. Kessler             | • Write an abstract            | • Bullet points              |
| • Professor XYZ                 | • Analysis                     | • Summary                    |
| • Editor from [target] journal  | • Condense lists               | • Table/Chart                |
| • PhD student in [specific field] | • Draft references           | • (MLA, APA, Chicago) citations |

---

## Complex Few-Shot Learning for Data Tagging

- Classify the text after *** using the classification definition after +++ and examples for classification after ###.

- +++
  { "factual": "Events, personal facts, actions, or known information without personal characteristics or opinions.",
    "cognitive": "Opinions, attitudes, thoughts, personal characteristics, agreement/disagreement statements, and self-disclosure questions.",
    "emotional": "Expressions of emotions towards events, people, or experiences, including self-esteem and emotional words like 'excited', 'hate', 'love', etc.",
    "irrelevant": "Contains general or unrelated statements not related to factual, cognitive or emotional." }

- ### Examples: ###

- ### 1. Example ###
  {"text": "Partially in St. Gallen and in Zurich because I am from Zurich.", "answer": "factual"}

- ### 2. Example ###
  {"text": "I was in the sports gymnasium and therefore I had to manage school and sport at the same time", "answer": "factual"}

- ### 3. Example ###
  {"text": "I am just happy that they aren't in my courses.", "answer": "emotional"}

*** To predict ***

- I really like prompt engineering

---

# Chain-of-thoughts (CoT)

Let’s work this out in a step by step way to be sure we have the right answer.


## Prompt: Writing & Revision

You are an editor for the information systems research journal, A+ journal in the information systems area. You will receive a paper with the introduction after ###.

*Step 1*

Go through the introduction, and in the first step, find mistakes, logical breaks, and weak argumentations.

*Step 2*

In the second step, go sentence by sentence and write out the questions a reviewer would have, reading the text, such as what is unclear or vague. Come up with one question per sentence/topic.

Think step by step to come up with the correct solution. Provide detailed reasoning for each step, followed by the correct solution.

---

Now, let's go through the 30 questions step by step and provide 1-2 specific sentences answering the question. Provide first the reasoning of why your solution would answer the question and how it would answer it. Afterward, provide your solution and the sentence which should be replaced.

Let's do this question per question. If you are done with one question, ask my permission to proceed to the next question until we reach the 30th question.

---