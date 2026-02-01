# keplerquest_llm

This repository contains the **LLM-based conversational backend** developed for the KeplerQuest-AI framework.  
The system provides guided, inquiry-oriented dialogue to support learners’ conceptual understanding of **Kepler’s laws of planetary motion**, and is designed to operate in conjunction with an external visualization client (e.g., augmented reality).

The implementation corresponds to the backend described in the paper presented at the  
**2026 IEEE Global Engineering Education Conference (EDUCON)** and is released to ensure **reproducibility and reuse** of the conversational AI infrastructure.

---

## Overview

The backend implements web-based conversational agents that:
- Interact with users through a browser-based chat interface
- Support inquiry-driven reasoning through structured prompts
- Avoid explicit disclosure of Kepler’s laws, encouraging observation-based explanation
- Provide qualitative evaluative feedback on user responses

The system is intentionally **domain-constrained to planetary motion and Kepler’s laws**, but the architecture can be adapted to other STEM topics requiring guided conceptual exploration.

---

## Knowledge Source

The Streamlit application retrieves its domain-specific knowledge from a
**public GitHub repository**, which is used as the source for the retrieval
process that grounds the LLM responses.

This design supports reproducibility and allows the backend to be adapted to
other instructional domains by changing the referenced repository.

---

## Technology Stack

- **Frontend / Interface:**  
  - Streamlit

- **LLM Inference:**  
  - Ollama (Open LLaMA 3.3–70B)
  - Optional support for Groq as an accelerated inference backend

- **Prompting Strategy:**  
  - Narrative framing  
  - Socratic questioning  
  - Reflection-oriented feedback  
  - Qualitative scoring of explanations

---

## Repository Contents

- `SpaceChat-app.py`  
  Main Streamlit application that launches the chatbot interface and manages user interaction.

- `htmlTemplates.py`  
  HTML templates used to structure and style the chat interface within Streamlit.

- `requirements.txt`  
  Python dependencies required to run the backend locally.

---

## Scope and Adaptation

This repository provides **only the conversational AI infrastructure** developed for the KeplerQuest-AI framework.  
It does not include learning activities, assessment instruments, or visualization components.

Although originally designed to support the learning of **Kepler’s laws of planetary motion**, the backend architecture is generalizable and can be adapted to:
- Inquiry-based STEM education  
- Conceptual scaffolding through guided dialogue  
- AI-supported reflective learning environments  

---

## License

This project is released under the  
**Creative Commons Attribution–NonCommercial 4.0 International (CC BY-NC 4.0)** license.

---

## Citation

If you use or adapt this code, please cite the corresponding paper presented at the  
**2026 IEEE Global Engineering Education Conference (EDUCON)**.
