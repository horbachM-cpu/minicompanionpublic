> Note: This repository is a public presentation of the project and does not include the full source code.

<div align="center">

# 🐾 Mini Companion

### *A Cute Desktop Mascot & Character UI Prototype*

A playful Tamagotchi-inspired mascot UI that combines light pet-care mechanics, local state, and lightweight AI conversations.

[✨ Features](#-features) • [🎮 Companions](#-meet-your-companions) • [📸 Screenshots](#-screenshots) • [💬 Contact](#-get-in-touch)

</div>

---

## 🌟 What is Mini Companion?

Mini Companion brings the joy of virtual pets into the AI era! Choose from 5 unique companions, each with their own personality, and experience meaningful conversations powered by advanced language models. Watch your companion grow, care for their needs, and unlock beautiful backgrounds as you build your relationship.

---

## ✨ Features

### 💭 **Intelligent Conversations**
- Each companion has a unique personality and speaking style
- Natural, context-aware responses that adapt to your companion's mood
- Optional "Think Mode" for more thoughtful, reasoned responses
- Customizable personality traits through custom instructions

### 🎮 **Tamagotchi-Inspired Gameplay**
- **Three Core Stats**: Hunger, Energy, and Happiness that change over time
- **Care Actions**: Feed, Play, Rest, and Pet your companion
- **Level System**: Gain XP through conversations and care
- **Daily Quests**: Complete tasks to earn Legacy Points
- **Background Shop**: Unlock and collect themed backgrounds for each companion

### 🎨 **Beautiful Design**
- Gorgeous kawaii dark-mode aesthetic
- Smooth animations and transitions
- Per-companion chat histories
- Multiple unlockable backgrounds for each companion
- Export/import your chat data

### 🤖 **Multiple AI Models**
- **Free Models**: DeepSeek Chimera (with reasoning), Llama 3.3 70B
- **Premium Models**: Grok 4.1 Fast, DeepSeek V3.2
- Optional reasoning mode for deeper, more thoughtful responses
- Flexible credit system for premium features

---

## 🐱 Meet Your Companions

<table>
<tr>
<td width="20%" align="center">
<h3>🐱 Mochi</h3>
<b>Kitten</b>
<br>
Sweet, playful, and full of curiosity
</td>
<td width="20%" align="center">
<h3>🐶 Biscuit</h3>
<b>Puppy</b>
<br>
Loyal, energetic, and always excited
</td>
<td width="20%" align="center">
<h3>🐥 Peep</h3>
<b>Chick</b>
<br>
Cute, curious, and adorably innocent
</td>
<td width="20%" align="center">
<h3>🦊 Kira</h3>
<b>Fox</b>
<br>
Mystical, wise, and enchanting
</td>
<td width="20%" align="center">
<h3>💕 Aria</h3>
<b>Human</b>
<br>
Friendly, expressive, and a little theatrical
</td>
</tr>
</table>

Each companion has **3 unique backgrounds** to unlock and collect!

---

## 📸 Screenshots

<div align="center">

### Default View
<img src="screenshots/Screenshot.png" width="45%" alt="Mini Companion Default Interface">

### Custom Background
<img src="screenshots/Screenshot2.png" width="45%" alt="Mini Companion with Custom Background">

*Experience beautiful kawaii aesthetics with unlockable themed backgrounds*

</div>

---

## 🎯 How It Works

1. **Choose Your Companion** - Select from 5 unique personalities
2. **Start Chatting** - Have natural conversations powered by AI
3. **Care for Them** - Feed, play, rest, and pet to keep them happy
4. **Level Up** - Gain XP and unlock new features
5. **Complete Quests** - Earn Legacy Points through daily challenges
6. **Customize** - Unlock and switch between beautiful backgrounds

---

## 🏗️ Architecture

Mini Companion uses a clean, serverless architecture that keeps everything responsive and scalable:

```mermaid
graph TD
    User[👤 User] <-->|Interacts| UI[📱 Frontend UI]

    subgraph Browser["🖥️ Client (Browser)"]
        UI <-->|Updates| State[🔄 State System]
        State -->|Persists| LS[(💾 LocalStorage)]
        State -- "Gamification Logic" --> UI
    end

    subgraph Cloud["☁️ Serverless Backend"]
        State -->|Fetch Request| Lambda[⚡ AWS Lambda]
        Lambda -->|Secure Proxy| OpenRouter[🤖 OpenRouter API]
    end

    OpenRouter -->|LLM Response| Lambda
    Lambda -->|JSON| State
```

**Key Benefits:**
- 🚀 Fast and responsive client-side interactions
- 💾 All data stays in your browser (privacy-first)
- ☁️ Serverless backend scales automatically
- 🔒 Secure API key management

---

## 📱 Tech Stack

**Frontend:**
- Vanilla JavaScript (ES6+)
- CSS3 with custom animations
- Modular architecture

**Backend:**
- AWS Lambda (serverless)
- OpenRouter API integration
- Secure API proxy

**Data:**
- LocalStorage for persistence
- JSON-based chat history
- Per-companion save states

---

## 💎 Highlights

- 🎨 **15 Backgrounds** - 3 unique themed backgrounds per companion
- 💬 **Unlimited Chats** - Free AI models for endless conversations
- 📊 **Gamification** - Stats, levels, quests, and rewards
- 🎭 **5 Personalities** - Each companion feels unique and authentic
- 💾 **Data Control** - Export/import all your conversations
- 🌙 **Dark Mode** - Easy on the eyes, beautiful aesthetics

---



## 📝 License

MIT License - Feel free to learn from and build upon this project!

---

## 💬 Get In Touch

Interested in the code, want to collaborate, or just want to chat about the project?

📧 **m.horbach92@gmail.com**

I'm happy to share access to the full repository and discuss the technical implementation!

---

<div align="center">

### Made with 💕 for cute companions everywhere!

*Remember: Your virtual companion is always there for you* 🐾

</div>
