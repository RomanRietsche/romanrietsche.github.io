---
title: 'Workshop AI in Research'
type: event
location: 'Bern University of Applied Sciences'
summary: 'How to use generative AI in reasearch'
#abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
#date: '2024-11-13'
#date_end: '2030-06-01T15:00:00Z'

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

# How-to 

Below you will find the prompts used in this workshop.

---

# Table of Contents
1. [Prompts](#prompts)
2. [Steps to Create Effective ChatGPT Prompt](#steps-to-create-effective-chatgpt-prompt)
3. [Example Phrases for Prompts](#example-phrases-for-prompts)
4. [Complex Prompt to Understand a New Topic](#complex-prompt-to-understand-a-new-topic)
6. [Prompt Techniques – Using Formula](#prompt-techniques-using-formula)
7. [Complex Few-Shot Learning for Data Tagging](#complex-few-shot-learning-for-data-tagging)
8. [Chain-of-thoughts (CoT)](#chain-of-thoughts-cot)
9. [Question based Prompt: Writing & Revision](#question-based-prompt-writing-revision)
10. [Metric based Prompt Writing Revision](#metric-based-prompt-writing-revision)
10. [Test Data](#test-data)

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


<br>

## Steps to Create Effective ChatGPT Prompt

1. **Identify the purpose and focus of the conversation.**
2. **Use specific and relevant language** (e.g., "Act as...").
3. **Avoid open or overly general prompts.**
4. **Review and revise your prompt.**

### Example Proposal Writing

> “Imagine you are writing a scientific proposal for receiving funding for educational technology in the canton of Bern in Switzerland. Act as a research scientist at the intersection of HCI and educational technology. Please imagine the following proposal summary: '…' Please create a specific timeline with milestones for the project and arrange them for the quarters in 2024. Study 1 will happen in Q2 and Study 2 in Q4.”

<br>

---

<br>

## Example Phrases for Prompts:

- Critical self-reflect …
- Improve it by 100% …
- Shorten the text by 20% … 
- You get 100 dollar tips when you improve it…
- Convince the reader …

<br>

**Improve Text:**

1. Create, at first, five quantitative measures, and rate your text on them
2. Then, revise the text
3. Measure the new text again, and show sentence by sentence how the measures improve
4. Provide reasoning first

<br>

---

<br>

## Complex Prompt to Understand a New Topic

-> copy each step one after the other into chatGPT, Claude, Gemini, etc.

I want to understand “prompt engineering”

### Initial Question Generation:
**Step 1**: 
Generate 10 initial questions about the topic, aiming for a mix of open-ended and closed questions. This variety encourages a broad exploration while also gathering specific details.  

**Guideline**: 
Ensure questions cover the what, why, how, and implications related to the topic to ensure a comprehensive initial overview.  

*Ask for my permission to go to the next step!*

<br>

### Thematic Clustering and Optimization:
**Step 2**: 
Determine an "optimal amount" of themes for clustering the questions. Use thematic analysis principles, focusing on patterns and concepts that recur across the initial questions.  

**Step 3**: 
Cluster the initial questions into themes based on the identified patterns. Aim for distinct yet comprehensive thematic clusters.  

*Ask for my permission to go to the next step!*

<br>

### Reflective Expansion of Questions:
**Step 4**: 
Review each theme cluster to identify gaps or emerging insights. Add two more questions for each theme to ensure thorough coverage. For each added question, provide a rationale based on identified gaps or new insights.  

**Step 5**: 
Output the final clusters with the set of questions.  

*Ask for my permission to go to the next step!*

<br>

### Detailed Question Answering with a Structured Template:

**Step 6**: 

Answer each question in 200 words using a specific template. Tailor the template slightly for questions (e.g., theoretical vs. practical) to allow nuanced responses.  
The template should cover why the question is important, what information or actions are needed, and which methods will be used, including examples or analogies. Emphasize reasoning before providing the answer, using a structured step-by-step approach.  

**Step 7**: 

After answering a question, ask permission to proceed to the next, ensuring a methodical and reflective process.  

*Ask for my permission to go to the next step!*

<br>

### Iterative Reflection and Summary:

**Step 8**: Conduct a reflective review of all responses after completing the answers. Summarize critical insights, contradictions, and new questions that have emerged. This step fosters a deeper understanding and may highlight further areas of inquiry.

<br>

---

<br>

## Prompt Techniques Using Formula

**Acting as [ROLE] perform [TASK] in [FORMAT]: insert unique data**

| **Role**                        | **Task / Aim**                 | **Format**                  |
|---------------------------------|--------------------------------|-----------------------------|
| • Expert Science Writer         | • Formulate research questions | • PDF                        |
| • Ronald C. Kessler             | • Write an abstract            | • Bullet points              |
| • Professor XYZ                 | • Analysis                     | • Summary                    |
| • Editor from [target] journal  | • Condense lists               | • Table/Chart                |
| • PhD student in [specific field] | • Draft references           | • (MLA, APA, Chicago) citations |

<br>

---

<br>

## Complex Few-Shot Learning for Data Tagging

```
Classify the text after *** using the classification definition after +++ and examples for classification after ###.


+++
  { "factual": "Events, personal facts, actions, or known information without personal characteristics or opinions.",
    "cognitive": "Opinions, attitudes, thoughts, personal characteristics, agreement/disagreement statements, and self-disclosure questions.",
    "emotional": "Expressions of emotions towards events, people, or experiences, including self-esteem and emotional words like 'excited', 'hate', 'love', etc.",
    "irrelevant": "Contains general or unrelated statements not related to factual, cognitive or emotional." }

**Examples:**

*1. Example*

  {"text": "Partially in St. Gallen and in Zurich because I am from Zurich.", "answer": "factual"}

*2. Example*

  {"text": "I was in the sports gymnasium and therefore I had to manage school and sport at the same time", "answer": "factual"}

*3. Example*

  {"text": "I am just happy that they aren't in my courses.", "answer": "emotional"}

**To predict**

I really like prompt engineering

```

<br>

---

<br>

# Chain-of-thoughts (CoT)

Let’s work this out in a step by step way to be sure we have the right answer. 
Provide Reasoning first and then the answer.

<br>

---

<br>

## Question based Prompt Writing  Revision 


```
You are an editor for the information systems research journal, A+ journal in the information systems area. You will receive a paper with the introduction after ###.

**Copy Step 1:**

Go through the introduction, and in the first step, find mistakes, logical breaks, and weak argumentations.

<br>

**Copy Step 2:**

In the second step, go sentence by sentence and write out the questions a reviewer would have, reading the text, such as what is unclear or vague. Come up with one question per sentence/topic.
Think step by step to come up with the correct solution. Provide detailed reasoning for each step, followed by the correct solution.

<br>

**Copy Step 3:**

Now, let's go through the 30 questions step by step and provide 1-2 specific sentences answering the question. Provide first the reasoning of why your solution would answer the question and how it would answer it. Afterward, provide your solution and the sentence which should be replaced.
Let's do this question per question. If you are done with one question, ask my permission to proceed to the next question until we reach the 30th question.


```

<br>

---

<br>

# Metric based Prompt Writing Revision

```
You are a reviewer for the "Information Systems Research" Journal, an A+ journal in Information Systems. 
You received a paper with the introduction shown between ###.

*Task*
Your task is to improve the quality of the introduction. 
The introduction should convince the reviewers to accept the paper.
Go through the introduction paragraph by paragraph and apply the following steps.

1. Evaluate the paragraph of this research paper according to five core metrics. For each metric, provide a score from 1-5 and a brief explanation
	1. **Relevance and Novelty**: Does the introduction engage the reader by addressing a pressing or innovative issue in the field?
	2. **Theoretical/Practical Contribution**: Does it establish why the research is essential for advancing knowledge or practice within information systems?
	3. **Positioning and Literature Engagement**: Does it critically situate the study within recent, high-impact research and show a clear and essential research gap?
	4. **Ambition of Objectives**: Are the objectives clear but also ambitious and original, fitting the scope of a leading journal?
	5. **Impactful Research Questions/Hypotheses**: Are the questions or hypotheses poised to make a meaningful impact, possibly opening new research paths or addressing a significant issue?
2. Improve the paragraph so that the metrics are improved. Make the changes bold.
3. Evaluate the paragraph of this research paper according to the five core metrics again. For each metric, provide a score from 1-5 and a brief explanation
4. Compare the two metrics; if the metrics are below 5, improve the paragraph again.

Think step by step, sentence by sentence, to provide the best possible solution. Provide in-depth reasoning first.

Ask for my permission to go to the next paragraph.

###

In 2021, blockchain added an estimated US\$ 119 million to the education market and is expected to increase with a compound annual growth rate of almost 44% to over US\$ 3 billion by 2030 (Business Research Insight, 2024). This development goes hand in hand with the increasing demand for digitizing and smartifying learning and working environments for flexibility and efficiency purposes. Regarding the development of digitization in the educational sector, according to HolonIQ (2023), the quaternary sector, including adult and on-the-job education, with 76%, is more than twice as oriented towards entering new markets and integrating new technologies than the tertiary sector, including higher education institutions, such as universities, with only 35%.

However, investigation concerning the use of blockchain in the former sector and emphasizing the benefits for teachers and institutions remains open. According to the Gartner 2019 CIO Survey (2019), implementing blockchain technology in the educational sector could promote the simplification of record keeping verifying various digitized types of certificates and their accreditation through blockchain technology. In addition to increasing efficiency, blockchain adoption helps secure intellectual property and prevent document fraud. Furthermore, it can also lead to entirely new business models, such as educational institutions "rely(ing) on blockchain and smart contracts as the basis of the relationship between learners and educators," as Moore states (2019).

Our systematic literature review revealed several proposals for implementing blockchain in higher education to increase efficiency and security, benefiting teachers and students.

Firstly, in the context of research and course development, Yano et al. (2022) propose building a blockchain network between researchers to openly publish and mutually peer-review their findings in an automated manner. Van Rossum (2017) further mentions that the latter could also facilitate and shorten the publishing process of research papers by involving publishers in the network or replacing them by just implementing smart contracts to set the standards for publishing.

###

```

Did all metrics improve to 5? critically reflect

# Test Data

```
Title: “More Than Just Pizza, It's An Experience!”
Rating: ★★★★★ 
Last night, we ventured out as a family to try this much-talked-about pizza place. The decor was an eclectic mix of modern chic and classic Italian. But the real star? The food. We opted for the chef's special tasting menu, and every dish was a revelation. The Pepperoni had the right amount of spice and the white pizza with truffle oil was sublime. The kids loved the interactive DIY pizza station. The staff was friendly, making sure we felt welcomed and attended to at all times. They truly understand that dining out is more than just about food; it's about creating lasting memories.

Title: “The Gold Standard of Home Delivery”
Rating: ★★★★★ In the age where takeout and deliveries can be hit or miss, this place sets the gold standard. Not only did the pizza arrive piping hot and well within the promised time, but the packaging was also eco-friendly. The taste? Absolutely divine! I ordered the Veggie Delight, and each vegetable tasted like it was handpicked with love. The crust was perfectly crispy, and the cheese ratio was spot on. The app was user-friendly with real-time tracking, and the delivery person was courteous and professional. Truly a seamless experience from start to finish.

Title: "Unpleasant Discovery Ruined My Meal" 
Rating: ★☆☆☆☆ 
I was halfway through enjoying my Margherita when I noticed something off. Upon closer inspection, I was horrified to find a hair embedded into the cheese. This just shows their utter disregard for hygiene standards. I had heard mixed reviews before but decided to give them a try. Never again!

Title: "Billing Nightmares with This Place!" 
Rating: ★☆☆☆☆ 
I always check my bank statements and, to my dismay, found that I was double charged for a single pizza order last week. When I reached out to customer service, they brushed off my concerns, leaving me feeling duped. It’s a real shame; their pizza is decent, but I can’t support a place with such shady billing practices.

Title: "Bait and Switch Promotions? No Thanks" 
Rating: ★★☆☆☆ Came across their 'buy one get one free' deal and thought it was a great opportunity to try their range. Imagine my surprise when I was informed at checkout that the deal doesn't apply to the pizzas I chose. It's disheartening when businesses use such misleading tactics to lure customers in.

Title: "App Experience is Abysmal" 
Rating: ★☆☆☆☆ Thought I'd save some time and order through their app. Big mistake! The app kept freezing and, on the third try, processed my payment without confirming my order. I spent a good hour on the phone trying to rectify this. It's 2023; app glitches like these are just unacceptable.

Title: "Dine-in? More Like Dive-in!" 
Rating: ★★☆☆☆ Wanted a change of scene, so decided to dine in. The tables were sticky, the service slow, and there was this loud group that the staff did nothing about. The whole atmosphere was far from the cozy pizza place I had imagined.

```
