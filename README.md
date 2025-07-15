# 🩺 Emergency Department Wait Time and Navigation Assistant Chatbot

This project is a local, AI-powered chatbot that helps users in the Halifax Regional Municipality explore healthcare options, including emergency department (ED) wait times, walk-in clinics, VirtualCareNS, pharmacy care, and more.

The chatbot is built using the **Ollama + AnythingLLM** stack and retrieves information from local, authoritative Nova Scotia Health documents. It is designed as an educational tool to reduce unnecessary emergency visits by guiding users to the most appropriate level of care.

---

## Features

- Simulates ED wait time estimates based on historical patterns
- Recommends alternatives such as 811, walk-in clinics, and VirtualCareNS
- Provides document-backed answers with citations
- Operates entirely locally with no internet connection required
- Uses a friendly, supportive tone (non-diagnostic)

---

## Repository Structure
```text
healthcarellm-chatbot-ed-waittime/
├─ knowledge_base/
│ ├─ knowledge_document_1.pdf # Where to go for care
│ ├─ knowledge_document_2.pdf # VirtualCareNS patient guide
│ ├─ knowledge_document_3.txt # Live wait time site URL
│ ├─ knowledge_document_4.txt # Nova Scotia Walk-in Clinics
│ └─ knowledge_document_5.txt # Typical wait time patterns
│ └─ knowledge_document_6.txt # VirtualCareNS
│ └─ knowledge_document_7.txt # 811 Telehealth Nova Scotia
│ └─ knowledge_document_8.txt # Mobile Primary Care Clinics - Nova Scotia Health
│ └─ knowledge_document_9.txt # Urgent Treatment Centres - Nova Scotia Health
├─ prompt/
│ └─ system_prompt.txt
├─ documentation/
│ ├─ scenario_pack.md
│ └─ use_case_description.md
├─ demo/
│ ├─ demo_video.mp4
│ └─ chat_transcript.txt
└─ README.md
```

---

## How to Run Locally

1. **Install Ollama**
   - [https://ollama.com/download](https://ollama.com/download)
   - Run: `ollama run mistral` or `ollama run llama3`

2. **Install AnythingLLM**
   - [https://anythingllm.com/desktop](https://anythingllm.com/desktop)
   - Configure your workspace and connect to Ollama at `http://127.0.0.1:11434`

3. **Upload Documents**
   - Go to the Knowledge tab inside your AnythingLLM workspace
   - Upload all files in the `/knowledge_base` folder

4. **Set the System Prompt**
   - Paste contents of `prompt/system_prompt.txt` into the workspace prompt settings

5. **Test the Chatbot**
   - Ask guided questions such as:
     - "How long is the wait time at Halifax Infirmary tonight?"
     - "If I have a minor cut, should I go to the ED or a walk-in clinic?"

---

## Sample Questions to Try

- "What can 811 help with?"
- "How do I refill a prescription without visiting a doctor?"
- "What’s VirtualCareNS and who can use it?"
- "When are EDs in Halifax usually busiest?"

---

## MEDICAL DISCLAIMER

This chatbot provides general information about ED wait times and healthcare alternatives in the Halifax Regional Municipality. The information is for educational purposes only.

This chatbot:
- Does NOT provide medical advice, diagnosis, or treatment  
- Is NOT a substitute for professional medical care  
- Does NOT establish a doctor-patient relationship  
- Should NOT be used in medical emergencies  

Always seek the advice of qualified healthcare professionals regarding any medical condition. In case of emergency, call 911 or go to your nearest emergency department immediately.

The wait time information provided is an estimate only and is subject to change based on patient volume and acuity. Patients with life-threatening conditions will always be seen first regardless of wait times.

**By using this chatbot, you acknowledge and agree to these terms.**

---

## Author

- Anjili Seereeram (Nova Scotia Health AI Project – MBAN Program)
- Date: July 2025

---
