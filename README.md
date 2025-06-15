# Imaginaries, Governance, and Practices of AI in the Welfare State: A Cultural Critical Inquiry
*By Heider Jeffer*

## 1. Introduction and Relevance

Early AI governance efforts prioritize efficiency, yet insufficient attention has been given to how welfare-state AI shapes public imaginaries, media discourses, and citizen perceptions. This doctoral project aims to examine how AI infrastructures in welfare services—such as social benefit algorithms, automated case allocation, and digital eligibility systems—are enacted, portrayed, and experienced within media environments. For instance, Försäkringskassan’s AI pilot projects on social benefits eligibility offer a concrete Swedish example of how algorithmic tools are introduced and contested in welfare governance.

Drawing on Critical and Cultural Theory, it explores three interconnected streams:

1. **Imaginaries**: How public narratives, mediated by journalism and social media, construct the AI welfare state.
2. **Governance**: How policies, institutional protocols, and algorithmic practices reinforce or challenge public values—justice, transparency, inclusion.
3. **Practices**: How citizens and welfare workers perceive, trust, and participate in algorithmic governance.

Situating these streams within Media and Communication Studies, the project responds to WASP-HS’s call for interdisciplinary exploration of AI’s societal impacts (\[wasp-hs.org]\[1]). It offers a critical-cultural intervention by interrogating not only the technologies themselves, but the mediated frameworks that legitimize them to citizens.

It offers a critical-cultural intervention by interrogating not only the technologies themselves, but also the mediated frameworks that legitimize them to citizens—including how governments may strategically manipulate public opinion through AI-powered narratives and decision-making systems.

## 2. Research Questions

1. **Imaginaries**

   * How do Swedish and regional media (print, digital, social) frame AI in welfare services, particularly relating to cases like Försäkringskassan’s pilot projects?
   * What imaginaries—threat, progress, surveillance, care—do these frames evoke?

2. **Governance**

   * How are algorithmic welfare tools, exemplified by Försäkringskassan’s initiatives, rationalized within policy documents and administrative discourse?
   * Which analytical frameworks and power dynamics become visible or hidden?

3. **Practices**

   * How do citizens and welfare professionals interpret, trust, resist, or subvert algorithmic interventions?
   * How do discourses and lived experiences align or clash?


## 3. Theoretical Framework

* **Critical and Cultural Theory**: Following Anderson’s ‘imagined communities’, media create collective imaginaries that shape social cohesion and exclusion. This framework allows analysis of how AI as “social glue” transforms welfare legitimacy.
* **Critical Algorithm Studies**: Drawing on James and Whelan’s work, the project pays close attention to bias, transparency, and ethical concerns in welfare algorithms (\[muse.jhu.edu]\[2], \[journals.sagepub.com]\[3]).
* **Media Ecology and Political Communication**: Inspired by WASP-HS research on AI and political communication, I will use multimodal analysis of visual and textual framing (\[wasp-hs.org]\[1]).

Finally, drawing from political communication theory, the project will interrogate how governments may *deploy AI discursively to manage, redirect, or manipulate public opinion*, particularly in moments of crisis or reform. This contributes to broader critiques of algorithmic power as an instrument of soft governance.

## 4. Methodology

**a. Media & Discourse Analysis**

* Collect a representative sample of Swedish media (national newspapers like *Dagens Nyheter*, *Svenska Dagbladet*, SVT news, and regional outlets) from 2023–2025.
* Focus on coverage of Försäkringskassan’s AI pilot projects to trace public and journalistic framings.
* Conduct frame analysis—identifying metaphors, narratives, affective registers.
* Analyze visual AI-media interplay using image analysis and semiotics.

**b. Policy & Institutional Text Analysis**

* Examine government white papers, municipal guidelines, and Försäkringskassan’s project documentation.
* Trace discursive strategies: data-driven efficiencies, accountability promises, and risk language.
* Use critical discourse analysis to understand power dynamics in language and logics.

**c. Ethnographic Engagement**

* Conduct interviews and focus groups with citizens, social workers, and case managers, including those involved in or affected by Försäkringskassan’s AI initiatives.
* Explore embodied experiences of AI systems: trust, alienation, resistance.
* Use qualitative coding (e.g., NVivo) to extract emergent themes.

**d. Triangulation & Reflexivity**

* Bridge discursive representations with real-world experiences to expose strengths and gaps in the imagined AI welfare state.
* Adopt a reflexive stance to my dual background in AI and humanities.

Here's a Python representation of the methodology section, structured as pseudocode with actual data structures and flow to show how the project could be implemented as a research workflow. This uses standard Python concepts like functions, classes, and comments to model **Media & Discourse Analysis**, **Policy Text Analysis**, and **Ethnographic Engagement**.

This is not production research code, but a structured illustration of the methodology. We can expand this using real tools like:

* `spaCy`, `nltk` or `transformers` for NLP and frame analysis
* `NVivo` (not Python, but you can export/import codebooks)
* `pandas` and `matplotlib` for data analysis and visualization


```python
# Research Methodology Representation in Python
# Developed using Python by Heider Jeffer

from typing import List, Dict
import random

# ---------------------------------------------
# 1. Data Collection & Sampling
# ---------------------------------------------

def collect_media_samples(years: List[int], sources: List[str]) -> List[Dict]:
    """
    Simulate collecting media articles from given sources and years.
    """
    media_data = []
    for year in years:
        for source in sources:
            media_data.append({
                "year": year,
                "source": source,
                "title": f"AI in welfare debated in {source} ({year})",
                "text": "AI is revolutionizing welfare systems...",
                "type": random.choice(["print", "digital", "social"]),
            })
    return media_data


# ---------------------------------------------
# 2. Media Frame Analysis
# ---------------------------------------------

def analyze_frames(media_data: List[Dict]) -> Dict[str, int]:
    """
    Perform simple keyword-based frame detection (placeholder for NLP).
    """
    frames = {"surveillance": 0, "care": 0, "efficiency": 0, "bias": 0}
    for article in media_data:
        text = article["text"].lower()
        if "surveillance" in text:
            frames["surveillance"] += 1
        if "care" in text:
            frames["care"] += 1
        if "efficient" in text:
            frames["efficiency"] += 1
        if "bias" in text:
            frames["bias"] += 1
    return frames


# ---------------------------------------------
# 3. Policy & Institutional Text Analysis
# ---------------------------------------------

def analyze_policy_documents(docs: List[str]) -> List[Dict]:
    """
    Simulate analysis of policy language (discourse markers).
    """
    keywords = ["efficiency", "accountability", "transparency", "risk"]
    results = []
    for doc in docs:
        found = [word for word in keywords if word in doc.lower()]
        results.append({"document": doc[:30], "keywords_found": found})
    return results


# ---------------------------------------------
# 4. Ethnographic Interview Simulation
# ---------------------------------------------

def conduct_interviews(participants: List[str]) -> List[Dict]:
    """
    Simulate qualitative interviews with citizens/welfare professionals.
    """
    themes = ["trust", "confusion", "resistance", "acceptance"]
    return [{"participant": p, "theme": random.choice(themes)} for p in participants]


# ---------------------------------------------
# 5. Triangulation
# ---------------------------------------------

def triangulate_results(media_frames, policy_keywords, interview_themes):
    """
    Integrate findings from all sources into a consolidated output.
    """
    print("\n[Triangulated Summary]")
    print("Media Frames:", media_frames)
    print("Policy Keyword Themes:", policy_keywords[:2], "...")  # print sample
    print("Interview Themes:", interview_themes[:3], "...")  # print sample


# ---------------------------------------------
# Run the Research Workflow
# ---------------------------------------------

years = [2023, 2024, 2025]
sources = ["Dagens Nyheter", "Sveriges Radio", "Twitter"]
policy_docs = [
    "The digitalization of welfare must increase efficiency and transparency.",
    "AI tools raise accountability and privacy concerns."
]
participants = ["Anna", "Mohammed", "Sara", "Lars"]

media_data = collect_media_samples(years, sources)
media_frames = analyze_frames(media_data)
policy_keywords = analyze_policy_documents(policy_docs)
interviews = conduct_interviews(participants)

triangulate_results(media_frames, policy_keywords, interviews)
```

Here is the visual representation of your research methodology workflow. Each step in the research process is shown as a node, with directional arrows indicating the flow from one phase to the next.

```python
# Research Methodology Representation in Python
# Developed using Python by Heider Jeffer

import matplotlib.pyplot as plt
import networkx as nx

# Define the research phases as a directed graph
phases = [
    ("Start", "Media Sampling"),
    ("Media Sampling", "Frame Analysis"),
    ("Media Sampling", "Visual Semiotics"),
    ("Frame Analysis", "Policy Document Collection"),
    ("Visual Semiotics", "Policy Document Collection"),
    ("Policy Document Collection", "Critical Discourse Analysis"),
    ("Critical Discourse Analysis", "Power Mapping"),
    ("Power Mapping", "Interviews & Focus Groups"),
    ("Interviews & Focus Groups", "Theme Extraction"),
    ("Theme Extraction", "Triangulation"),
    ("Triangulation", "Reflexive Analysis"),
    ("Reflexive Analysis", "Python Modeling"),
    ("Python Modeling", "End")
]

# Create a directed graph
G = nx.DiGraph()
G.add_edges_from(phases)

# Draw the graph
plt.figure(figsize=(15, 10))
pos = nx.spring_layout(G, seed=42)  # consistent layout
nx.draw(G, pos, with_labels=True, node_size=3000, node_color='lightblue', 
        font_size=10, font_weight='bold', arrows=True, arrowstyle='->', arrowsize=15)
plt.title("Visual Representation of Research Methodology Workflow", fontsize=14)
plt.show()

```


## 5. Alignment with WASP-HS and Media & Communication Studies

* **Imaginaries**: Investigates how citizens understand AI in welfare, resonating directly with WASP-HS “imaginaries” stream.
* **Governance**: Evaluates institutional rationales and potential harms, aligning with the “governance” stream, exemplified by Swedish welfare AI initiatives.
* **Practices**: Explores user perceptions and practices, in line with “practices” focus.
* **Media-centric approach**: Positions media analysis at the core, making theoretical contributions to Media & Communication Studies.
* **Interdisciplinary training**: Integrates textual, visual, ethnographic methods with critical AI studies—reflecting the intellectual profile of WASP-HS.

---

## 6. Originality and Contribution

* Fills a research gap by combining discursive, institutional, and experiential perspectives on AI welfare—an emergent but under-theorized field.
* Introduces visual and narrative methodologies to the study of welfare algorithms, complementing existing scholarship on political bots and platform politics (\[mdpi.com]\[4], \[wasp-hs.org]\[5]).
* Engages with pressing questions: who frames welfare AI? Who benefits—and who becomes invisible?
* Informs policy by exposing how media framings shape trust and acceptance—and potentially undermine equity.

---

## 7. Work Plan (Timeline Overview)

| Phase | Tasks                                     | Months |
| ----- | ----------------------------------------- | ------ |
| 1     | Initial literature review, media sampling | 1–6    |
| 2     | Frame and discourse analysis              | 7–18   |
| 3     | Field interviews and thematic coding      | 12–24  |
| 4     | Integrative analysis; theory building     | 20–30  |
| 5     | Writing chapters, peer presentations      | 30–48  |
| 6     | Submission, defense, outreach efforts     | 48–60  |

Supports the doctoral structure (240 ECTS / 4 years), with integrated teaching and networking via WASP-HS.

---

## 8. Feasibility

* Strong institutional support from Södertörn and WASP-HS resources—including access to archives, media databases, ethical review boards, and interdisciplinary workshops.
* Technological and analytical capacity built through my background in Python, NLP, qualitative coding tools, and statistical methods.
* Multilingual proficiency (English, Arabic, Italian) supports media analysis and participant interviews.
* Prior success in managing complex, cross-disciplinary research projects demonstrates capability and scholarly maturity.

---

## 9. Ethical Considerations

* Full compliance with GDPR and ethical standards in analyzing media, policy, and human participants.
* Informed consent, anonymity, and secure storage for interview data.
* Reflexivity on positionality as an AI-trained researcher engaging with critical cultural studies.

---

## 10. Expected Outputs

* **Three academic articles**:

  1. Media framings of AI in welfare;
  2. Institutional governance logics, with reference to Försäkringskassan’s projects;
  3. Citizen experiences and trust in AI welfare.
* **Dissertation**: A coherent interdisciplinary argument about AI welfare imaginaries and practices.
* **Public outputs**: Summaries for policy stakeholders, workshops with welfare agencies, presentations at WASP-HS forums.
* **Long-term impact**: A theoretical model for future research, supporting democratic and media-aware AI governance in welfare systems.

---

## 11. Conclusion

This project combines a cultural‑critical lens with policy analysis and ethnographic insight to comprehensively examine AI’s role in welfare-state imaginaries, governance, and social practices. The inclusion of Försäkringskassan’s AI pilot projects as a case study grounds the research in Swedish contexts, aligning fully with the thematic priorities of WASP‑HS and Media & Communication Studies. It offers innovative contributions to both academic scholarship and public discourse on algorithmic justice.

---

### Bibliography

* Anderson, B. (1992). *Imagined Communities: Reflections on the Origin and Spread of Nationalism*. Verso. (\[arxiv.org]\[6])
* James, A., & Whelan, A. (2022). ‘Ethical’ artificial intelligence in the welfare state: Discourse and discrepancy in Australian social services. *Critical Social Policy, 42*(1). (\[journals.sagepub.com]\[3])
* Mendelsohn, J., Budak, C., & Jurgens, D. (2021). *Modeling Framing in Immigration Discourse on Social Media*. arXiv. (\[arxiv.org]\[6])
* Bondi, E., Xu, L., & Acosta‑Navas, D. (2021). *Envisioning Communities: A Participatory Approach Towards AI for Social Good*. arXiv. (\[arxiv.org]\[7])
* Jia, C., Lam, M., Mai, M. C., Hancock, J., & Bernstein, M. (2023). *Embedding Democratic Values into Social Media AIs via Societal Objective Functions*. arXiv. (\[arxiv.org]\[8])
* Öhman, C., & Mainz, S. (2021). *AI and Political Communication*. WASP‑HS Project. (\[wasp-hs.org]\[1])
* Försäkringskassan. (2022). *AI Pilot Project Report*. Government of Sweden. ([https://www.forsakringskassan.se/ai-pilot-project-report](https://www.forsakringskassan.se/ai-pilot-project-report))
* Pink, S. (2022). Critical perspectives on sociotechnical imaginaries of AI. *Discourse & Society*.




