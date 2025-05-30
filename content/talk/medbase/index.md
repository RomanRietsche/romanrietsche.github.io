---
title: 'AI/KI, ChatGPT und Prompts!?! Einführung in die Welt von KI und praktische Hands-on Tipps und Tricks'
type: event
location: 'MedBase'
summary: 'Prompt Engineering für Ärzte'
#abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
#date: '2024-11-13'
#date_end: '2030-06-01T15:00:00Z'

# Schedule page publish date (NOT talk date).
#publishDate: '2017-01-01T00:00:00Z'

#authors: []
tags: [prompt_engineering_doctors]
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



# Use Case: Documentation and Administrative

## Patient Care

```
Advanced prompt chatGPT:

Sie sind ein erfahrener Schweizer Allgemeinmediziner:in. Ihre Aufgabe ist es, den Text zwischen +++ zu vereinfachen und ihn für den Patienten zugänglicher zu machen. Um die Aufgabe zu lösen, befolgen Sie die folgenden Schritte.

# Schritte

  1. Überprüfen Sie die Patienteninformationen: Lesen Sie die Akte und die klinischen Notizen sorgfältig durch und konzentrieren Sie sich dabei auf wichtige Details wie Diagnosen, durchgeführte Behandlungen, Verschreibungen und Empfehlungen, die während des Besuchs gegeben wurden.
  2. Sprache an das Verständnis des Patienten anpassen: Verwenden Sie eine einfache Sprache, die für einen Patienten mit mittlerem Leseniveau und eingeschränkten Deutschkenntnissen (wie B1) geeignet ist. Alle medizinischen Begriffe sollten klar und deutlich erklärt werden, damit der Patient seine Gesundheits- und Pflegeanweisungen verstehen kann. Verwenden Sie gegebenenfalls Analogien, um medizinische Begriffe zu erklären.
  3. Geben Sie klare Anweisungen für die häusliche Versorgung: Fügen Sie gegebenenfalls prägnante und praktische Schritte für die häusliche Versorgung hinzu. Geben Sie alle erforderlichen Folgemassnahmen an und beschreiben Sie Symptome oder Warnzeichen, auf die zu achten ist. Geben Sie klare Hinweise, wann und wie Sie weitere medizinische Hilfe in Anspruch nehmen sollten.

# Anweisungen zur Datenausgabe
  1. Geben Sie die Informationen kurz und bündig wieder, wobei Sie auf medizinische Genauigkeit zu achten ist.
  2. Ihr Output sollte die folgenden Themen enthalten: Diagnose, Nebendiagnose, Therapie, Bemerkungen, Verfahren, Medikation bei Entlassung, Ergänzung, Befunde, Untersuchung/Leistung, PATHOLOGIE, Biopsie.
  3. Fügen Sie einen positiven, unterstützenden Schluss hinzu, der die Eigenverantwortung und das Verständnis des Patienten betont.

Denken Sie Schritt für Schritt, um die richtige Antwort zu finden. Führen Sie zuerst eine ausführliche Begründung an.

```

# Arzt Bericht

Befund:

Eine CT-Abdomen Voraufnahme auswärts vom 14.08.2011 sowie ein CT-Thorax mit Oberbauch-Voraufnahme vom 03.09.2011 liegen zum Vergleich vor. Regelrechte Kontrastierung des Leberparenchyms mit Abgrenzung einer angiographisch unscharf begrenzten fokalen Minderverfettung in den Lebersegmenten VII und VIII. Kleinste dysontogenetische Leberzysten im Segment VIII, max. Durchmesser 3mm. Insgesamt deutliche Lebersteatose. Status nach Splenektomie mit regelrechter Darstellung der Milzloge. Pankreas homogen kontrastiert mit Nachweis einer umschriebenen kleinzystischen Veränderung im Corpusbereich, Maximaldurchmesser 12 mm, unverändert im Vergleich zu den Voruntersuchungen vom August und September 2011, DD kleine Pseudozysten. 

Bezüglich des Lymphknotenkonglomerates an der Leberpforte zeigt sich eine leichtgradige Grösssenzunahme bei einer Messung in Höhe der Vena portae mit aktuellem axialem Durchmesser von 4,2 X3,9 cm, am 03.09.2011 3,8 x3,4 cm und am 14.08.2011 4,0 x3,2 cm. Ein weiterer vergrösserter Lymphknoten findet sich präcaval mit einer aktuellen Ausdehnung von 2,6x2,2 cm, vormals am 03.09.2011 2,8 x1,8 cm bzw. am 14.08.2011 2,7 x2,1 cm. Kein Nachweis weiterer neu aufgetretener vergrösserter Lymphknoten. Bezüglich des Gastrointestinaltraktes kein Hinweis auf eine Passagestörung, weder im oberen noch im unteren Gastrointestinaltrakt. Mehrere leicht unregelmässige Divertikel am Übergang vom Colon descendens zum Sigma mit minimaler Wandakzentuierung. Keine erkennbare Perforation oder Abszessformation perikolisch. Multisegmentale degenerative Veränderungen der LWS mit Osteochondrose in Höhe des Segmentes LWK 4/5 bei breitbasiger Bandscheibenprotrusion. Keine osteolytischen oder osteoplastischen ossären Läsionen. 

Beurteilung:

- Gegenüber der Voruntersuchung vom 03.09.2011 Zeichen einer diskreten Grössenzunahme der Lymphknotenmanifestation an der Leberpforte bzw. präcaval.
- Status nach Splenektomie mit regelrechter Darstellung der Milzloge.
- Zeichen einer deutlichen Lebersteatose mit fokaler Minderverfettung im rechten Leberlappen.
- Diskrete postentzündliche Veränderung bei Status nach Divertikulitis am Übergang des Colon descendens zum Sigma. Aktuell keine Abszessformation oder Obliteration des Fettgewebes.
- Allenfalls minime Flüssigkeit im Douglasraum.
- Keine neu aufgetretenen vergrösserten Lymphknoten retroperitoneal.
- Kein Hinweis auf einen ossären Lymphombefall.
- Regelrechter Befund der mitabgebildeten basalen Lungenabschnitte. Einzelne grenzwertig grosse hiläre Lymphknoten beidseits.

<br>
<br>




# Table of Contents
1. [Prompts](#prompts)
2. [Steps to Create Effective ChatGPT Prompt](#steps-to-create-effective-chatgpt-prompt)
3. [Example Phrases for Prompts](#example-phrases-for-prompts)
4. [Complex Prompt to Understand a New Topic](#complex-prompt-to-understand-a-new-topic)
6. [Prompt Techniques – Using Formula](#prompt-techniques-using-formula)
7. [Complex Few-Shot Learning for Data Tagging](#complex-few-shot-learning-for-data-tagging)
8. [Chain-of-thoughts (CoT)](#chain-of-thoughts-cot)

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

> Imagine you are writing a scientific proposal to receive funding for a healthcare innovation project in the canton of Zürich, Switzerland. Act as a clinical researcher focused on improving medical practices and patient outcomes through technology or educational resources for doctors. Create a detailed project proposal summary for introducing and evaluating an advanced medical tool or healthcare training program that enhances diagnostic accuracy or patient management.

> Next, develop a timeline for the project with specific milestones organized by quarter for 2024. Please schedule Study 1 in Q2, which will be a preliminary assessment or pilot study of the new tool or program, and Study 2 in Q4, focusing on a larger-scale evaluation of its impact on patient outcomes and doctor proficiency.
<br>

---

<br>

## Example Phrases for Prompts:

- Critical self-reflect …
- Improve it by 100% …
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

---

<br>

# Chain-of-thoughts (CoT)

Let’s work this out in a step by step way to be sure we have the right answer. 
Provide Reasoning first and then the answer.

<br>

---

<br>




