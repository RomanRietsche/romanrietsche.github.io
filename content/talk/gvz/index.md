---
title: 'KI, ChatGPT und Prompts!?! Einführung in die Welt von KI und praktische Hands-on Tipps und Tricks'
type: event
location: 'GVZ'
summary: 'Grundlagen der Prompt Techniken'
#abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
#date: '2024-11-13'
#date_end: '2030-06-01T15:00:00Z'

# Schedule page publish date (NOT talk date).
#publishDate: '2017-01-01T00:00:00Z'

#authors: []
tags: [prompt_engineering_gvz]
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

<br>


# Prompts

```

# Beispiel System Prompt

Entwickeln Sie eine Reihe von Multiple-Choice-Fragen, um das Verständnis von „Prompt Engineering“ unter den Teilnehmern des GKV-Workshops zu bewerten.

# Aufgabe
Stellen Sie sicher, dass die Fragen klar sind und sich auf die Hauptthemen der Präsentation über „Prompt Engineering“ konzentrieren.
Jede Frage sollte eine richtige Antwort und mehrere plausible Distraktoren enthalten.
Achten Sie auf eine Mischung aus verschiedenen Schwierigkeitsgraden der Fragen, um die verschiedenen Verständnisebenen richtig einschätzen zu können.

# Schritte

Identifizieren Sie die Hauptthemen und Ziele der Präsentation über „Promptes Engineering“.
Entwickeln Sie Fragen, die diese Schlüsselthemen ansprechen, und stellen Sie sicher, dass sie das Verständnis, die Anwendung und die Analyse bewerten, wo dies möglich ist.
Entwickeln Sie eine Reihe von Multiple-Choice-Optionen für jede Frage, einschliesslich einer richtigen Antwort und drei oder vier Ablenkungsmöglichkeiten.
Überprüfen Sie die Fragen auf Klarheit und Relevanz für das Präsentationsmaterial.

# Ausgabeformat

Auf jede Frage sollten vier Optionen folgen, wobei:
Eine Option ist als die richtige Antwort gekennzeichnet.
Jede Option ist mit einem Buchstaben gekennzeichnet (A, B, C, D, E).

Beispielformat:
Frage: [Text der Frage]
A) Option 1
B) Option 2
C) Option 3 (Richtige Antwort)
D) Option 4

# Beispiele

**Frage**: Was ist „Prompt Engineering“?
Der Prozess der Erstellung und Verfeinerung von Prompts, um KI-Modelle effizient zu instruieren 
Der Bau physischer Komponenten für Computersysteme
Die Entwicklung von Software für die Datenanalyse
Entwurf von Prompts für die Mensch-Computer-Interaktion
(Richtige Antwort: A)

...

# Anmerkungen

Fügen Sie Fragen ein, die sich mit Definitionen, praktischen Anwendungen und potenziellen Fallstricken beim „Prompt Engineering“ befassen.
Ziehen Sie szenariobasierte Fragen in Betracht, um das angewandte Verständnis zu testen.
Vermeiden Sie übermäßigen Fachjargon, es sei denn, er wurde ausdrücklich in der Präsentation behandelt.

```




## How to Craft Effective Prompts: Key Principles

# Bestandteile eines effektiven Prompts

| **Kategorie**                            | **Empfehlungen**                                                                                                                                                                      |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Klarheit und Verständlichkeit**       | - Verwenden Sie Trennzeichen für mehr Klarheit (z. B. `### Text ###`)<br>- Erwägen Sie die Bereitstellung von Beispielen für die korrekte Ausgabe (Few-Shot-Prompt)                                                           |
| **Spezifität und Detailgenauigkeit**    | - Geben Sie das gewünschte Ausgabeformat an<br>- Geben Sie die Länge der Ausgabe an. Denken Sie in natürlichen Mengen, wie „ein Dutzend“.                                                                                       |
| **Kontext und Relevanz**                | - Definieren Sie die Rolle (z. B. „Sie sind Übersetzer.“)<br>- Zielgruppe und Zweck (z. B. „Übersetzen Sie für ein italienisches Publikum, das nach frischen Produkten sucht.“)                                                |
| **Schritt-für-Schritt-Anleitung**       | - Fügen Sie Schritt-für-Schritt-Anweisungen ein (z. B. „Übersetzen Sie zuerst ins Italienische, dann machen Sie es eingängig.“)                                                                                                |
| **Konditionierung für Präzision**       | - Konditionieren Sie die Antworten des Modells auf den Kontext, um genauere Ergebnisse zu erhalten (z. B.: „Legen Sie Ihrer Übersetzung gegebenenfalls das folgende Wörterbuch zugrunde: `{Wörterbuch}`“)                     |


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



# Anleitung zur Kritischen Selbstreflexion und Textverbesserung

## Zielsetzung
Verbessern Sie den gegebenen Text um 100%. Wenn Sie es schaffen, den Text überzeugend und qualitativ hochwertig zu optimieren, erwartet Sie ein imaginäres Trinkgeld von 100 Dollar. Der Leser soll von der neuen Version des Textes überzeugt werden.

---

## Beispiel: Verbesserung des Textes "XYZ"

```

### **1. Festlegung von Fünf Quantitativen Messwerten**
Definieren Sie zunächst fünf klare, quantitative Kriterien, um die Qualität des Textes objektiv zu bewerten. Diese könnten sein:

- **Klarheit** (Wie verständlich ist der Text? Skala von 1 bis 10)
- **Struktur** (Wie logisch und übersichtlich ist der Aufbau? Skala von 1 bis 10)
- **Überzeugungskraft** (Wie stark ist die Argumentation? Skala von 1 bis 10)
- **Leseransprache** (Wie gut wird der Leser emotional angesprochen? Skala von 1 bis 10)
- **Sprachliche Qualität** (Wie präzise und ansprechend ist die Wortwahl? Skala von 1 bis 10)

---

### **2. Bewertung des Ursprünglichen Textes**
Bewerten Sie den Ausgangstext nach den fünf festgelegten Kriterien.

| Messwert          | Bewertung (1-10) | Begründung                                      |
|-------------------|-----------------|-------------------------------------------------|
| Klarheit          | 6               | Einige Aussagen sind unklar formuliert.         |
| Struktur          | 5               | Der Text wirkt ungeordnet und sprunghaft.       |
| Überzeugungskraft | 4               | Die Argumentation ist wenig schlüssig.          |
| Leseransprache    | 5               | Wenig emotionale Ansprache, wirkt distanziert.  |
| Sprachliche Qualität | 6           | Sprachlich solide, aber mit Verbesserungspotenzial. |

---

### **3. Textverbesserung**
Überarbeiten Sie den Text gezielt, um alle fünf Messwerte zu verbessern. Achten Sie auf:

- Präzisere Formulierungen für mehr Klarheit.
- Einen logischen und gut strukturierten Aufbau.
- Stärkere Argumente und Belege zur Erhöhung der Überzeugungskraft.
- Eine aktivere und emotionalere Ansprache des Lesers.
- Eine abwechslungsreiche, aber klare Sprache.

---

### **4. Bewertung des Überarbeiteten Textes**
Messen Sie erneut die Qualität des verbesserten Textes.

| Messwert          | Bewertung (1-10) | Begründung                                      |
|-------------------|-----------------|-------------------------------------------------|
| Klarheit          | 9               | Der Text ist jetzt präzise und gut verständlich.|
| Struktur          | 9               | Der Aufbau folgt einer klaren, logischen Linie. |
| Überzeugungskraft | 8               | Die Argumentation ist deutlich schlüssiger.     |
| Leseransprache    | 8               | Der Leser wird direkter und emotionaler angesprochen. |
| Sprachliche Qualität | 9           | Die Wortwahl ist präzise und abwechslungsreich. |

---

### **5. Satz-für-Satz-Analyse**
Vergleichen Sie Satz für Satz den alten mit dem neuen Text und zeigen Sie konkret, wie sich die Messwerte verbessert haben.

**Beispiel:**
- **Alt:** "Der Text könnte besser strukturiert sein."
- **Neu:** "Um die Aussagekraft des Textes zu erhöhen, wurde eine klarere Struktur mit logischen Übergängen eingeführt."

**Verbesserung:** Erhöhte Klarheit und Struktur durch spezifischere Formulierung.

---

## Fazit
Durch die strukturierte Vorgehensweise und die gezielte Analyse nach definierten Messwerten wird der Text nicht nur messbar, sondern auch nachvollziehbar verbessert. Diese Methode gewährleistet eine nachhaltige Optimierung der Textqualität.

```

<br>

---

<br>

## Komplexer Prompt zum Verstehen eines neuen Themas

-> Kopieren Sie die einzelnen Schritte nacheinander in chatGPT, Claude, Gemini, etc.

```


# Aufgabe: Ich möchte «Prompt-Technik» verstehen

## Initiale Fragengenerierung

**Schritt 1**

Entwickeln Sie 10 erste Fragen zum Thema, wobei Sie eine Mischung aus offenen und geschlossenen Fragen anstreben. Diese Vielfalt fördert eine breite Untersuchung, während gleichzeitig spezifische Details gesammelt werden.

**Richtlinie**

Achten Sie darauf, dass die Fragen das Was, Warum, Wie und die Auswirkungen des Themas abdecken, um einen umfassenden ersten Überblick zu erhalten.

---

## Thematisches Clustering und Optimierung

**Schritt 2**

Bestimmen Sie eine „optimale Anzahl“ von Themen für die Clusterung der Fragen. Wenden Sie die Prinzipien der thematischen Analyse an und konzentrieren Sie sich auf Muster und Konzepte, die in den ursprünglichen Fragen wiederkehren.

**Schritt 3**

Gruppieren Sie die ursprünglichen Fragen auf der Grundlage der ermittelten Muster zu Themen. Streben Sie eindeutige, aber dennoch umfassende thematische Cluster an.

---

## Reflektierte Erweiterung der Fragen

**Schritt 4**

Überprüfen Sie jeden Themenkomplex, um Lücken oder neue Erkenntnisse zu ermitteln. Fügen Sie für jedes Thema zwei weitere Fragen hinzu, um eine vollständige Abdeckung zu gewährleisten. Geben Sie für jede hinzugefügte Frage eine Begründung auf der Grundlage der festgestellten Lücken oder neuen Erkenntnisse.

**Schritt 5**

Geben Sie die endgültigen Cluster mit dem Fragenkomplex aus.

---

## Detaillierte Beantwortung von Fragen mit einer strukturierten Vorlage

**Schritt 6**

Beantworten Sie jede Frage in 200 Wörtern anhand einer bestimmten Vorlage. Passen Sie die Vorlage je nach Frage (z. B. theoretisch oder praktisch) leicht an, um differenzierte Antworten zu ermöglichen. Die Vorlage sollte erläutern, warum die Frage wichtig ist, welche Informationen oder Maßnahmen erforderlich sind und welche Methoden verwendet werden, einschließlich Beispiele oder Analogien. Betonen Sie die Argumentation, bevor Sie die Antwort geben, indem Sie aktive Schlussfolgerungen ziehen. Denken Sie Schritt für Schritt.

**Schritt 7**

Bitten Sie nach der Beantwortung einer Frage um Erlaubnis, mit der nächsten fortzufahren, um einen methodischen und reflektierten Prozess zu gewährleisten.

```


<br>

---

<br>

# Prompt-Techniken - Formel

> **Als [ROLE] führe [AUFGABE] in [FORMAT] aus: füge eindeutige Daten ein**

| **Rolle**                                      | **Aufgabe / Ziel**                               | **Format**                  |
|------------------------------------------------|--------------------------------------------------|-----------------------------|
| - Wissenschaftlicher Fachautor                 | - Frage formulieren                              | - PDF                       |
| - Ronald C. Kessler                            | - Verfassen einer Zusammenfassung                | - Aufzählungspunkte         |
| - Professor XYZ                                | - Analyse                                        | - Zusammenfassung           |
| - Redakteur von [Zielzeitschrift]              | - Listen kürzen                                  | - Tabelle/Grafik            |
| - Doktorand in [bestimmtes Fachgebiet]         | - Referenzen entwerfen                           |                              |

<br>

---

<br>

---

<br>

# Chain-of-thoughts (CoT)

Lassen Sie uns dies Schritt für Schritt ausarbeiten, um sicherzustellen, dass wir die richtige Antwort haben.
Geben Sie zunächst die Begründung an und dann die Antwort.

<br>

---

<br>




