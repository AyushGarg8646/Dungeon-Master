# Dungeon-Master
For the demo click the link
https://drive.google.com/drive/folders/1_I3ixucIYpfBZQ2dR9ngO-tBfVqnmYI6?usp=sharing
# 🧙‍♂ *AI Dungeon Master: Persistent Storytelling with Intelligent Memory*

> "Every choice matters, every consequence persists, and the world evolves with you."

---

## 🎯 *Project Overview*

Text-based storytelling in tabletop role-playing games (TTRPGs) thrives on one key figure — the *Dungeon Master (DM)* — who maintains world continuity, reacts dynamically to player choices, and keeps every session coherent and alive.

This project reimagines that experience with *AI Dungeon Master, an intelligent storytelling system powered by **Large Language Models (LLMs)* and a *dual-memory architecture* that allows it to remember, adapt, and evolve over time.

Unlike traditional AI chat systems that forget context after a few turns, our design ensures:
- Persistent long-term memory across 30+ turns 🧠  
- Coherent, cinematic storytelling 🎬  
- Immersive gameplay continuity 🧩  

---

## 🏗 *Vision & Design Goals*

- 🧩 *Consistency & Coherence:* Maintain story continuity across long interactions.  
- 🧠 *Dynamic Memory System:* Combine short-term reasoning with long-term recall.  
- 🎨 *Immersive Storytelling:* Blend creativity with logical world rules.  
- ⚙ *Modular & Scalable Architecture:* Easy to extend, debug, and upgrade.  
- 💬 *Natural Player Experience:* Accepts typos, slang, or imperfect English seamlessly.  

---

## ⚙ *System Architecture*

The AI Dungeon Master system integrates *memory-driven narrative intelligence* through the following modular pipeline:


                ┌─────────────────────────────────────────┐
                │          🧙‍♂ AI DUNGEON MASTER          │
                │  Cinematic storytelling & world logic   │
                └─────────────────────────────────────────┘
                                ▲
                                │
     ┌──────────────┬───────────┼───────────────┬──────────────┐
     │              │           │               │              │
     ▼              ▼           ▼               ▼              ▼
🎭 Story Context   📚 Rulebook  💾 Memory DB   💡 Info DB   🔁 Input Verifier
(Long-Term RAG)   (Lore &      (Persistent    (Monsters,   (Grammar, intent,
30+ Turns)         Mechanics)   Chroma Store)  Spells, etc)  typo correction)


---

---

## 💻 *Technical Stack*

| Component | Technology |
|------------|-------------|
| *LLM Engine* | [Groq API](https://groq.com) with *LLaMA-3.3-70B-Versatile* |
| *Embeddings* | SentenceTransformers (all-MiniLM-L6-v2) |
| *Vector Store* | [ChromaDB](https://www.trychroma.com/) |
| *Graph Orchestration* | [LangGraph](https://github.com/langchain-ai/langgraph) |
| *Environment Management* | Python dotenv, modular scripts |
| *Memory Persistence* | Chroma-based RAG + summarization |
| *Frontend Interaction* | Text-based console adventure |

---

## 🧩 *Key Features*

✅ *Dynamic Memory System* — Combines short- and long-term context for coherent storytelling.  
✅ *Context-Aware Input Correction* — Understands imperfect or typo-filled player commands.  
✅ *Rulebook-Integrated Logic* — Automatically references D&D spells, monsters, and rules.  
✅ *Auto-Summarization* — Extracts and stores only relevant story details for future recall.  
✅ *Agentic RAG Architecture* — Modular graph flow with intelligent state transitions.  
✅ *Engaging Player Experience* — Natural dialogue, evolving world, and cinematic narration.  

---

## 🚀 *Setup Guide*

### 1️⃣ *Clone the Repository*
bash
git clone https://github.com/<your-username>/ai-dungeon-master.git
cd ai-dungeon-master


### 2️⃣ *Install Dependencies*
bash
pip install -r requirements.txt


### 3️⃣ *Set Up Environment Variables*
Create a .env file and add your *Groq API Key*:
bash
GROQ_API_KEY="your_groq_api_key_here"


### 4️⃣ *Prepare Vector Databases*
Make sure the following directories exist:

./Test4/                ← Long-term story memory
./dm_rulebook_db/       ← D&D rulebook embeddings
./dm_info_db/           ← Structured entity info


### 5️⃣ *Run the Game*
bash
python main.py


---

## 🧩 *Gameplay Flow*

1. *Player Input* → Understood & verified (even with typos).  
2. *Memory Retrieval* → Relevant context fetched via RAG.  
3. *Rule & Info Augmentation* → Adds lore, rules, and entities.  
4. *AI Narration* → DM generates immersive, cinematic response.  
5. *Summarization* → Only relevant data stored into long-term memory.  

---

## 🧭 *Future Enhancements*

- 🧩 Dynamic Quest Log with auto-updating objectives.  
- 🗺 Visual map integration via Streamlit UI.  
- 🧍 NPCs with evolving memories and emotional states.  
- 💾 Cloud-based persistent saves across sessions.  

---

## 👥 *Team & Credits*
*TeamName:* Barbarians
*Developer:* Dhairya Goyal & Ayush Garg 
*Mentorship:* INTER IIT Bootcamp  
*Project Theme:* Dynamic Memory for Persistent Storytelling  
*Model:* LLaMA-3.3-70B via Groq API  

---

## 🧡 *In One Line*

> “An AI Dungeon Master that remembers your past, reacts to your choices, and builds a living world that grows with every turn.” 🌍✨
