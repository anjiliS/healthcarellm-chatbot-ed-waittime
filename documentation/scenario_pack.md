# Emergency Department Wait Time and Navigation Assistant Chatbot

## Scenario Background

In Halifax, Nova Scotia, emergency departments (ED) can experience significant wait times, especially during peak hours or flu season. Patients with non-urgent issues may not realize alternative care options are available, contributing to overcrowding. 

Nova Scotia Health and local hospitals sometimes publish average wait times and guidance on when to seek emergency versus urgent or primary care.

This scenario asks students to use the **Ollama + AnythingLLM** stack, combined with **locally available, authoritative health education materials**, to design a chatbot for **ED Wait Time and Navigation Assistance**.

---

## Scenario Goals

Your chatbot should:

- Help users understand typical ED wait times and how they fluctuate
- Guide users on alternative options (walk-in clinics, telehealth) for non-emergencies
- Clearly communicate that the chatbot does **not provide professional medical diagnoses**

---

## Recommended Knowledge Base Materials

You must collect and organize structured local health education materials as your retrieval-augmented generation (RAG) knowledge base. Suggested sources include:

- Nova Scotia Health – Emergency Department Wait Time Pages or Historical Averages
- Local Hospital Websites – Alternative Care Options
- Nova Scotia 811 Telehealth Service Information
- Walk-In Clinic Hours and Contact Details
- Any relevant government public health updates

All knowledge base documents must be uploaded as PDF, Markdown, or plain text, using consistent file names such as:

knowledge_document_1.pdf
knowledge_document_2.md
knowledge_document_3.txt


---

## Required Questions for Testing

Your final chatbot must be able to answer these user questions using your uploaded knowledge base materials:

1. **"How long is the average wait time at the downtown hospital emergency tonight?"**
2. **"If I have a minor cut, can I go to a walk-in clinic instead?"**

---

## Suggested GitHub Repository Structure

cold-flu-chatbot/
├─ knowledge_base/
│ ├─ knowledge_document_1.pdf
│ ├─ knowledge_document_2.md
│ └─ knowledge_document_3.txt
├─ prompt/
│ └─ system_prompt.txt
├─ documentation/
│ ├─ scenario_pack.md
│ └─ use_case_description.md
├─ demo/
│ ├─ demo_video.mp4
│ └─ chat_transcript.txt
└─ README.md


---

## Deliverables

**Knowledge Base**
- All documents used in AnythingLLM
- Clearly named and structured as shown above

**System Prompt**
- A file that defines the chatbot’s role, tone, scope, and ethical boundaries

**Use Case Description**
- A short Markdown file describing user pain points and how the chatbot addresses them

**Demo Materials**
- A screen recording or video showing chatbot responses to the core scenario questions
- A saved chat transcript

**README.md**
- Project overview
- Local deployment and testing instructions
- Author(s) and date
- **Must include a prominent disclaimer: "This chatbot does not provide medical advice."**

---

## Important Notes

- All materials must be uploaded to a public or private GitHub repository for review
- The chatbot is for **educational research only**
- It **must not be used** to diagnose or treat actual medical conditions


