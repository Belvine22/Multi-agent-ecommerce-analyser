# 🤖 Multi-Agent E-commerce Analyzer

> Système multi-agents IA pour l'automatisation de l'analyse 
> de produits e-commerce — développé chez DeBytes Ltd (2026)
> Code source confidentiel — vitrine technique publique

---

## 🎯 Résultats clés

| Métrique | Valeur |
|----------|--------|
| 🤖 Nombre d'agents | **7 agents IA** |
| ⚡ Temps d'analyse | **< 5 minutes** par produit |
| 🔗 Orchestrateur | **Google ADK** |
| 🧠 LLMs intégrés | **Gemini + Groq** |
| 🔄 Pipeline | Analyse · ROI · Scoring · Rapport |

---

## 🏗️ Architecture multi-agents

```
          PRODUIT E-COMMERCE (input)
          URL · Titre · Prix · Données
                      │
                      ▼
        ┌─────────────────────────┐
        │     ORCHESTRATEUR       │
        │      Google ADK         │
        │   (coordination des     │
        │      7 agents)          │
        └─────────────┬───────────┘
                      │
     ┌────────────────┼────────────────┐
     │                │                │
     ▼                ▼                ▼
┌─────────┐     ┌─────────┐      ┌─────────┐
│ Agent 1 │     │ Agent 2 │      │ Agent 3 │
│Scraper  │     │Analyzer │      │Pricing  │
│Collecte │     │Analyse  │      │Analyse  │
│ données │     │produit  │      │  prix   │
└────┬────┘     └────┬────┘      └────┬────┘
     │               │                │
     ▼               ▼                ▼
┌─────────┐     ┌─────────┐      ┌─────────┐
│ Agent 4 │     │ Agent 5 │      │ Agent 6 │
│Competitor     │  ROI    │      │ Quality │
│Analysis │     │Calculator     │Checker  │
│         │     │         │      │         │
└────┬────┘     └────┬────┘      └────┬────┘
     │               │                │
     └───────────────┼────────────────┘
                     │
                     ▼
              ┌─────────────┐
              │   Agent 7   │
              │   Report    │
              │  Generator  │
              └──────┬──────┘
                     │
                     ▼
        ┌────────────────────────┐
        │     RÉSULTAT FINAL     │
        │  • Score produit       │
        │  • Analyse ROI/marges  │
        │  • Recommandation      │
        │  • Rapport complet     │
        └────────────────────────┘
```

---

## 🔄 Pipeline de décision

```
INPUT PRODUIT
     │
     ▼
┌─────────────────────┐
│  COLLECTE DONNÉES   │  Scraping · APIs data
│  Agent 1            │  Prix · Descriptions
└──────────┬──────────┘  Avis · Concurrents
           │
           ▼
┌─────────────────────┐
│  ANALYSE LLM        │  LangChain + Gemini
│  Agents 2·3·4       │  Orchestration des
└──────────┬──────────┘  appels · Mémoire
           │
           ▼
┌─────────────────────┐
│  CALCUL ROI/MARGES  │  Analyse rentabilité
│  Agent 5            │  Seuils de décision
└──────────┬──────────┘  Scoring automatique
           │
           ▼
┌─────────────────────┐
│  QUALITY CHECK      │  Validation résultats
│  Agent 6            │  Retry si insuffisant
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  RAPPORT FINAL      │  Streamlit dashboard
│  Agent 7            │  Visualisations Plotly
└─────────────────────┘  Export PDF/CSV
```

---

## 🛠️ Stack technique

**LLM & Orchestration**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=google&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat&logo=groq&logoColor=white)

**Interface & Visualisation**

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)

**Infrastructure**

![GitLab](https://img.shields.io/badge/GitLab_CI/CD-FC6D26?style=flat&logo=gitlab&logoColor=white)
![Plesk](https://img.shields.io/badge/Plesk-52BBE6?style=flat&logo=plesk&logoColor=white)

---

## 💡 Fonctionnalités clés

- **Orchestration intelligente** — Google ADK coordonne les 7 agents avec gestion des dépendances et retry automatique
- **Mémoire des agents** — LangChain maintient le contexte entre les appels LLM
- **RAG intégré** — enrichissement des agents avec données produits en temps réel
- **Analyse ROI automatique** — calcul des marges, seuils de rentabilité et recommandations
- **Dashboard interactif** — interface Streamlit avec visualisations Plotly en temps réel
- **Pipeline robuste** — gestion des erreurs, retry logic et validation qualité

---

## ⚠️ Note sur la confidentialité

Ce projet a été développé dans le cadre d'un **stage chez DeBytes Ltd (2026)**.
Le code source est la propriété de l'entreprise et reste **confidentiel**.

Ce repository est une **vitrine technique publique** décrivant l'architecture
et les choix technologiques du projet.

---

## 👩‍💻 Auteure

**Belvine YEMDJO** — [@Belvine22](https://github.com/Belvine22)

Ingénieure Systèmes Numériques & IA — UTT 2026
