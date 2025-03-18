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

# Workshop Prompts

Nachstehend finden Sie die in diesem Workshop verwendeten Prompts.

<br>

---

# Links

https://tiktokenizer.vercel.app


---

<br>

# Beispiel System Prompt

```

Entwickeln Sie eine Reihe von Multiple-Choice-Fragen, um das Verständnis von „Prompt Engineering“ unter den Teilnehmern des GKV-Workshops zu bewerten. 
Denken Sie Schritt für Schritt, um die bestmöglichen Multiple-Choice-Fragen zu erstellen.

# Aufgabe
Stellen Sie sicher, dass die Fragen klar sind und sich auf die Hauptthemen der Präsentation über „Prompt Engineering“ konzentrieren.
Jede Frage sollte eine richtige Antwort und mehrere plausible Distraktoren enthalten.
Achten Sie auf eine Mischung aus verschiedenen Schwierigkeitsgraden der Fragen, um die verschiedenen Verständnisebenen richtig einschätzen zu können.

# Schritte

1. Identifizieren Sie die Hauptthemen und Ziele der Präsentation über „Promptes Engineering“.
2. Entwickeln Sie Fragen, die diese Schlüsselthemen ansprechen, und stellen Sie sicher, dass sie das Verständnis, die Anwendung und die Analyse bewerten, wo dies möglich ist.
3. Entwickeln Sie eine Reihe von Multiple-Choice-Optionen für jede Frage, einschliesslich einer richtigen Antwort und drei Ablenkungsmöglichkeiten.
4. Überprüfen Sie die Fragen auf Klarheit und Relevanz für das Präsentationsmaterial.

# Ausgabeformat

Auf jede Frage sollten vier Optionen folgen, wobei:
- Eine Option ist als die richtige Antwort gekennzeichnet.
- Jede Option ist mit einem Buchstaben gekennzeichnet (a, b, c, d).

Beispielformat:

Frage: [Text der Frage]
a) Option 1
b) Option 2
c) Option 3 (Richtige Antwort)
d) Option 4

# Beispiele

**Frage**: Was ist „Prompt Engineering“?

a) Der Prozess der Erstellung und Verfeinerung von Prompts, um KI-Modelle effizient zu instruieren (Richtige Antwort)
b) Der Bau physischer Komponenten für Computersysteme
c) Die Entwicklung von Software für die Datenanalyse
d) Entwurf von Prompts für die Mensch-Computer-Interaktion

...

# Anmerkungen

- Fügen Sie Fragen ein, die sich mit Definitionen, praktischen Anwendungen und potenziellen Fallstricken beim „Prompt Engineering“ befassen.
- Ziehen Sie szenariobasierte Fragen in Betracht, um das angewandte Verständnis zu testen.
- Vermeiden Sie übermässigen Fachjargon, es sei denn, er wurde ausdrücklich in der Präsentation behandelt.

```
<br>

---

<br>

# Bestandteile eines effektiven Prompts

| **Kategorie**                            | **Empfehlungen**                                                                                                                                                                      |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Klarheit und Verständlichkeit**       | - Verwenden Sie Trennzeichen für mehr Klarheit (z. B. `### Text ###`)<br>- Erwägen Sie die Bereitstellung von Beispielen für die korrekte Ausgabe (Few-Shot-Prompt)                                                           |
| **Spezifität und Detailgenauigkeit**    | - Geben Sie das gewünschte Ausgabeformat an<br>- Geben Sie die Länge der Ausgabe an. Denken Sie in natürlichen Mengen, wie „ein Dutzend“.                                                                                       |
| **Kontext und Relevanz**                | - Definieren Sie die Rolle (z. B. „Sie sind Übersetzer.“)<br>- Zielgruppe und Zweck (z. B. „Übersetzen Sie für ein italienisches Publikum, das nach frischen Produkten sucht.“)                                                |
| **Schritt-für-Schritt-Anleitung**       | - Fügen Sie Schritt-für-Schritt-Anweisungen ein (z. B. „Übersetzen Sie zuerst ins Italienische, dann machen Sie es eingängig.“)                                                                                                |
| **Konditionierung für Präzision**       | - Konditionieren Sie die Antworten des Modells auf den Kontext, um genauere Ergebnisse zu erhalten (z. B.: „Legen Sie Ihrer Übersetzung gegebenenfalls das folgende Wörterbuch zugrunde: `{Wörterbuch}`“)                     |


<br>

# Schritte zur Erstellung eines effektiven Prompts

1. Bestimmen Sie den Zweck und den Schwerpunkt des Gesprächs.
2. Verwenden Sie eine spezifische und relevante Sprache ("Handeln Sie als...")
3. Vermeiden Sie offene oder übermässig allgemeine Prompts.
4. Überprüfen und überarbeiten Sie Ihren Prompt.


## Beispiel E-mail:

Stellen Sie sich vor, Sie schreiben eine geschäftliche E-Mail, um Finanzierung für ein Innovationsprojekt im Bereich der Gebäudeversicherung im Kanton Zürich, Schweiz, zu beantragen.
Handeln Sie als Unternehmen mit dem Fokus auf die Verbesserung von Risikobewertungen und Schadensprävention durch den Einsatz von Technologie oder Schulungsressourcen für Versicherungsfachleute.

Verfassen Sie eine detaillierte E-Mail-Zusammenfassung des Projektvorschlags, in der ein fortschrittliches Analyseinstrument oder ein Schulungsprogramm vorgestellt und dessen Einführung sowie Evaluierung beschrieben wird. 

Ziel ist es, die Genauigkeit bei der Risikoeinschätzung oder das Schadenmanagement nachhaltig zu optimieren.

<br>

---

<br>



# Anleitung zur kritischen Selbstreflexion und Textverbesserung

## Zielsetzung
- Verbessern Sie den gegebenen Text um 100%. 
- Wenn Sie es schaffen, den Text überzeugend und qualitativ hochwertig zu optimieren, erwartet Sie ein imaginäres Trinkgeld von 100 Dollar. 
- Der Leser soll von der neuen Version des Textes überzeugt werden.

---

# Beispiel: Verbesserung des Textes "XYZ"

```

# **1. Festlegung von Fünf Quantitativen Messwerten**
Definieren Sie zunächst fünf klare, quantitative Kriterien, um die Qualität des Textes objektiv zu bewerten. Diese könnten sein:

- **Klarheit** (Wie verständlich ist der Text? Skala von 1 bis 10)
- **Struktur** (Wie logisch und übersichtlich ist der Aufbau? Skala von 1 bis 10)
- **Überzeugungskraft** (Wie stark ist die Argumentation? Skala von 1 bis 10)
- **Leseransprache** (Wie gut wird der Leser emotional angesprochen? Skala von 1 bis 10)
- **Sprachliche Qualität** (Wie präzise und ansprechend ist die Wortwahl? Skala von 1 bis 10)

---

# **2. Bewertung des Ursprünglichen Textes**
Bewerten Sie den Ausgangstext nach den fünf festgelegten Kriterien.

| Messwert          | Bewertung (1-10) | Begründung                                      |
|-------------------|-----------------|-------------------------------------------------|
| Klarheit          | 6               | Einige Aussagen sind unklar formuliert.         |
| Struktur          | 5               | Der Text wirkt ungeordnet und sprunghaft.       |
| Überzeugungskraft | 4               | Die Argumentation ist wenig schlüssig.          |
| Leseransprache    | 5               | Wenig emotionale Ansprache, wirkt distanziert.  |
| Sprachliche Qualität | 6           | Sprachlich solide, aber mit Verbesserungspotenzial. |

---

# **3. Textverbesserung**
Überarbeiten Sie den Text gezielt, um alle fünf Messwerte zu verbessern. Achten Sie auf:

- Präzisere Formulierungen für mehr Klarheit.
- Einen logischen und gut strukturierten Aufbau.
- Stärkere Argumente und Belege zur Erhöhung der Überzeugungskraft.
- Eine aktivere und emotionalere Ansprache des Lesers.
- Eine abwechslungsreiche, aber klare Sprache.

---

# **4. Bewertung des Überarbeiteten Textes**
Messen Sie erneut die Qualität des verbesserten Textes.

| Messwert          | Bewertung (1-10) | Begründung                                      |
|-------------------|-----------------|-------------------------------------------------|
| Klarheit          | 9               | Der Text ist jetzt präzise und gut verständlich.|
| Struktur          | 9               | Der Aufbau folgt einer klaren, logischen Linie. |
| Überzeugungskraft | 8               | Die Argumentation ist deutlich schlüssiger.     |
| Leseransprache    | 8               | Der Leser wird direkter und emotionaler angesprochen. |
| Sprachliche Qualität | 9           | Die Wortwahl ist präzise und abwechslungsreich. |

---

# **5. Satz-für-Satz-Analyse**
Vergleichen Sie Satz für Satz den alten mit dem neuen Text und zeigen Sie konkret, wie sich die Messwerte verbessert haben.

**Beispiel:**
- **Alt:** "Der Text könnte besser strukturiert sein."
- **Neu:** "Um die Aussagekraft des Textes zu erhöhen, wurde eine klarere Struktur mit logischen Übergängen eingeführt."

**Verbesserung:** Erhöhte Klarheit und Struktur durch spezifischere Formulierung.

---

# Fazit
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

| **Rolle**                                | **Aufgabe / Ziel**                               | **Format**                  |
|------------------------------------------|--------------------------------------------------|-----------------------------|
| - Wissenschaftlicher Fachautor           | - Frage formulieren                              | - PDF                       |
| - Ronald C. Kessler                      | - Verfassen einer Zusammenfassung                | - Aufzählungspunkte         |
| - Professor XYZ                          | - Analyse                                        | - Zusammenfassung           |
| - Redakteur von [Zielzeitschrift]        | - Listen kürzen                                  | - Tabelle/Grafik            |
| - Mitarbeiter in [bestimmtes Fachgebiet] | - Referenzen entwerfen                           |                              |

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

# Fortgeschrittene Prompt Techniken

Agarwal, R., Singh, A., Zhang, L. M., Bohnet, B., Chan, S., Anand, A., Abbas, Z., Nova, A., Co-Reyes, J. D., Chu, E., Behbahani, F., Faust, A., and Larochelle, H. 2024. Many-Shot In-Context Learning, arXiv. (http://arxiv.org/abs/2404.11018).
“AI Tutor.” 2023. , January 1. (https://github.com/JushBJJ/Mr.-Ranedeer-AI-Tutor).
Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., Neelakantan, A., Shyam, P., Sastry, G., Askell, A., Agarwal, S., Herbert-Voss, A., Krueger, G., Henighan, T., Child, R., Ramesh, A., Ziegler, D. M., Wu, J., Winter, C., Hesse, C., Chen, M., Sigler, E., Litwin, M., Gray, S., Chess, B., Clark, J., Berner, C., McCandlish, S., Radford, A., Sutskever, I., and Amodei, D. 2020. “Language Models Are Few-Shot Learners,” , May 28. (http://arxiv.org/pdf/2005.14165v4).
Bsharat, S. M., Myrzakhan, A., and Shen, Z. 2023. Principled Instructions Are All You Need for Questioning LLaMA-1/2, GPT-3.5/4, [object Object]. (https://doi.org/10.48550/ARXIV.2312.16171).
Chia, Y. K., Chen, G., Tuan, L. A., Poria, S., and Bing, L. 2023. “Contrastive Chain-of-Thought Prompting,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2311.09277).
Gao, S., Dwivedi-Yu, J., Yu, P., Tan, X. E., Pasunuru, R., Golovneva, O., Sinha, K., Celikyilmaz, A., Bosselut, A., and Wang, T. 2024. “Efficient Tool Use with Chain-of-Abstraction Reasoning,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2401.17464).
Gunasekar, S., Zhang, Y., Aneja, J., Mendes, C. C. T., Del Giorno, A., Gopi, S., Javaheripi, M., Kauffmann, P., Rosa, G., Saarikivi, O., Salim, A., Shah, S., Behl, H. S., Wang, X., Bubeck, S., Eldan, R., Kalai, A. T., Lee, Y. T., and Li, Y. 2023. “Textbooks Are All You Need,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2306.11644).
Liu, P., Yuan, W., Fu, J., Jiang, Z., Hayashi, H., and Neubig, G. 2021. “Pre-Train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2107.13586).
Park, J. S., O’Brien, J. C., Cai, C. J., Morris, M. R., Liang, P., and Bernstein, M. S. 2023. “Generative Agents: Interactive Simulacra of Human Behavior,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2304.03442).
Peng, B., Galley, M., He, P., Cheng, H., Xie, Y., Hu, Y., Huang, Q., Liden, L., Yu, Z., Chen, W., and Gao, J. 2023. “Check Your Facts and Try Again: Improving Large Language Models with External Knowledge and Automated Feedback,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2302.12813).
“Prompt Engineering Guide.” (n.d.). (https://www.promptingguide.ai/).
Schulhoff, Sander, Ilie, M., Balepur, N., Kahadze, K., Liu, A., Si, C., Li, Y., Gupta, A., Han, H., Schulhoff, Sevien, Dulepet, P. S., Vidyadhara, S., Ki, D., Agrawal, S., Pham, C., Kroiz, G., Li, F., Tao, H., Srivastava, A., Da Costa, H., Gupta, S., Rogers, M. L., Goncearenco, I., Sarli, G., Galynker, I., Peskoff, D., Carpuat, M., White, J., Anadkat, S., Hoyle, A., and Resnik, P. 2024. The Prompt Report: A Systematic Survey of Prompting Techniques, arXiv. (http://arxiv.org/abs/2406.06608).
Servantez, S., Barrow, J., Hammond, K., and Jain, R. 2024. “Chain of Logic: Rule-Based Reasoning with Large Language Models,” , January 1. (http://arxiv.org/pdf/2402.10400v2).
Shinn, N., Cassano, F., Labash, B., Gopinath, A., Narasimhan, K., and Yao, S. 2023. “Reflexion: Language Agents with Verbal Reinforcement Learning,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2303.11366).
Sun, J., Luo, Y., Gong, Y., Lin, C., Shen, Y., Guo, J., and Duan, N. 2023. “Enhancing Chain-of-Thoughts Prompting with Iterative Bootstrapping in Large Language Models,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2304.11657).
Wang, X., Wei, J., Schuurmans, D., Le, Q., Chi, E., Narang, S., Chowdhery, A., and Zhou, D. 2022. “Self-Consistency Improves Chain of Thought Reasoning in Language Models,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2203.11171).
Wang, Z., Mao, S., Wu, W., Ge, T., Wei, F., and Ji, H. 2023. “Unleashing Cognitive Synergy in Large Language Models: A Task-Solving  Agent through Multi-Persona Self-Collaboration,” , July 11. (http://arxiv.org/pdf/2307.05300v2).
Wei, J., Wang, X., Schuurmans, D., Bosma, M., Ichter, B., Xia, F., Chi, E., Le, Q., and Zhou, D. 2022. “Chain-of-Thought Prompting Elicits Reasoning in Large Language Models,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2201.11903).
Wu, T., Terry, M., and Cai, C. J. 2022. “AI Chains: Transparent and Controllable Human-AI Interaction by Chaining Large Language Model Prompts,” in CHI Conference on Human Factors in Computing Systems, S. Barbosa, C. Lampe, C. Appert, D. A. Shamma, S. Drucker, J. Williamson, and K. Yatani (eds.), New York, NY, USA: ACM, pp. 1–22. (https://doi.org/10.1145/3491102.3517582).
Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. 2022. “ReAct: Synergizing Reasoning and Acting in Language Models,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2210.03629).
Yao, Y., Li, Z., and Zhao, H. 2023. “Beyond Chain-of-Thought, Effective Graph-of-Thought Reasoning in Large Language Models,” arXiv, January 1. (https://doi.org/10.48550/arXiv.2305.16582).





