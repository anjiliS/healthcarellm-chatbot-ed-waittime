# 📄 Use Case Description: ED Wait Time and Navigation Chatbot

## User Profile

The target users are **Nova Scotians seeking urgent or emergency care**, especially those who:
- Are unsure whether to visit the emergency department (ED)
- Do not have a primary care provider
- Are unfamiliar with alternative healthcare services like walk-in clinics, VirtualCareNS, or 811
- May be using mobile or web platforms for health information

---

## Problem Overview

Emergency departments in Halifax and surrounding regions frequently experience **overcrowding and long wait times**, especially during peak hours and flu season. Many patients with **non-urgent health issues** visit the ED due to a lack of awareness of **alternative care options**. This leads to system strain, increased wait times for serious cases, and poor patient experiences.

---

## Proposed Solution

The proposed solution is a **locally hosted chatbot**—powered by the Ollama + AnythingLLM stack—that:
- Uses **retrieval-augmented generation (RAG)** to pull responses from official Nova Scotia Health documents
- **Educates patients** on the difference between emergency, urgent, and primary care
- **Shares current or average ED wait times** (based on trusted sources)
- Recommends **appropriate alternatives** like 811, walk-in clinics, pharmacy services, and VirtualCareNS
- Avoids clinical advice and instead offers **navigation support and health education**

---

## Success Criteria

The chatbot is successful if it can:
1. **Accurately respond to the core scenario questions:**
   - “How long is the average wait time at the downtown hospital emergency tonight?”
   - “If I have a minor cut, can I go to a walk-in clinic instead?”
2. Provide clear, helpful guidance using only the uploaded local health documents
3. Offer **consistent, non-diagnostic responses** and always include appropriate disclaimers
4. Increase user awareness of alternative care services in Nova Scotia

---

## Technologies Used

- **Ollama**: For running a local large language model (Mistral)
- **AnythingLLM**: For document ingestion, retrieval, and chatbot interface
- **Nova Scotia Health PDFs and websites**: As the knowledge base
- (Optional) **Python scraper**: To pull live ED wait time data into the chatbot’s context

---

## Ethical and Safety Notes

- The chatbot does **not** provide medical advice or diagnoses.
- Users are always encouraged to call **911** for life-threatening emergencies.
- The system includes visible disclaimers to prevent misunderstanding.
