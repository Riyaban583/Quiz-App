<div align="center">

# 🧠 Quiz App (React)

<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />

<p align="center">
  <img src="https://img.shields.io/github/stars/Riyaban583/Quiz-App?style=social" alt="Stars" />
  <img src="https://img.shields.io/github/forks/Riyaban583/Quiz-App?style=social" alt="Forks" />
  <img src="https://img.shields.io/github/watchers/Riyaban583/Quiz-App?style=social" alt="Watchers" />
</p>

### A simple and interactive **Quiz Application** built using **React**

*Users can attempt multiple-choice questions, get instant feedback on answers, and view their final score at the end.*

</div>

---

## 🌟 Features

<div align="center">

| Feature | Description |
|---------|-------------|
| 📋 **Multiple Choice** | Engaging multiple-choice questions |
| ✅ **Instant Feedback** | Real-time correct/wrong answer highlighting |
| 🔒 **Answer Locking** | Prevents multiple clicks per question |
| ➡️ **Easy Navigation** | Smooth next question transition |
| 🧮 **Score Tracking** | Live score updates throughout quiz |
| 🏁 **Result Display** | Comprehensive final score screen |
| 🎨 **Modern UI** | Clean and responsive design |

</div>

---

## 🛠️ Tech Stack

<div align="center">

```mermaid
graph LR
    A[React.js] --> B[Quiz App]
    C[JavaScript ES6] --> B
    D[CSS3] --> B
    E[Vite] --> B
    
    style A fill:#61DAFB,stroke:#333,stroke-width:2px
    style C fill:#F7DF1E,stroke:#333,stroke-width:2px
    style D fill:#1572B6,stroke:#333,stroke-width:2px
    style E fill:#646CFF,stroke:#333,stroke-width:2px
    style B fill:#FF6B6B,stroke:#333,stroke-width:3px
```

</div>

<div align="center">

| Technology | Purpose |
|------------|---------|
| ⚛️ **React.js** | UI Component Framework |
| 📜 **JavaScript (ES6)** | Core Programming Language |
| 🎨 **CSS** | Styling & Layout |
| ⚡ **Vite** | Build Tool & Dev Server |

</div>

---

## 📂 Project Structure

```
QuizApp/
│
├── 📁 src/
│   ├── 📁 components/
│   │   └── 📁 Quiz/
│   │       ├── 📄 Quiz.jsx        # Main quiz component
│   │       └── 🎨 Quiz.css        # Component styling
│   │
│   ├── 📁 assets/
│   │   └── 📄 data.js             # Quiz questions data
│   │
│   ├── 📄 App.jsx                 # Root component
│   └── 📄 main.jsx                # Entry point
│
├── 📁 public/                      # Static assets
├── 📄 index.html                   # HTML template
├── 📄 package.json                 # Dependencies
└── 📖 README.md                    # Documentation
```

## 📊 How It Works

<div align="center">

```mermaid
graph TD
    A[Start Quiz] --> B[Load Question from data.js]
    B --> C[Display 4 Options]
    C --> D{User Selects Answer}
    D --> E[Lock Answer]
    E --> F{Correct?}
    F -->|Yes| G[Highlight Green ✅]
    F -->|No| H[Highlight Red ❌]
    G --> I[Update Score]
    H --> I
    I --> J{More Questions?}
    J -->|Yes| B
    J -->|No| K[Show Final Score 🏆]
    
    style A fill:#4CAF50,stroke:#333,stroke-width:2px,color:#fff
    style K fill:#FF6B6B,stroke:#333,stroke-width:2px,color:#fff
    style G fill:#7CB342,stroke:#333,stroke-width:2px,color:#fff
    style H fill:#E53935,stroke:#333,stroke-width:2px,color:#fff
```

</div>

### 🎯 Key Mechanics

- ✨ Questions are loaded from `data.js`
- 🔢 Each question has 4 options
- 🟢 Correct answers are highlighted in **green**
- 🔴 Wrong selections are highlighted in **red**
- 📈 Final score is shown after the last question

---

### State Management

```javascript
const [index, setIndex] = useState(0);
const [question, setQuestion] = useState(data[index]);
const [lock, setLock] = useState(false);
const [score, setScore] = useState(0);
const [result, setResult] = useState(false);
```

---

## 📌 Future Enhancements

<div align="center">

| Priority | Feature | Status |
|----------|---------|--------|
| 🔥 | ⏱️ Timer for each question | 🔜 Planned |
| 🔥 | 🔁 Restart quiz option | 🔜 Planned |
| ⭐ | 📱 Better mobile responsiveness | 🔜 Planned |
| ⭐ | 🎉 Animations and sound effects | 💡 Idea |
| ⭐ | 📊 Question difficulty levels | 💡 Idea |
| ⭐ | 💾 Save progress locally | 💡 Idea |
| ⭐ | 🏅 Leaderboard system | 💡 Idea |

</div>
