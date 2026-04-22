# 📘 Daily Reflection Decision Tree Assignment  

**Candidate Name:** Barkha Yadav  
**Role:** Data Analytics Intern  
**Company:** DeepThought CultureTech  

---

## 🔹 Overview

This project is a deterministic decision tree system designed to help users reflect on their daily productivity using a structured framework:

**Question → Hypothesis → Experiment**

---

## 🔹 Part A: Decision Tree (Deterministic System)

### ✅ Objective
To analyze a user’s day based on task completion, satisfaction, and challenges, and provide actionable suggestions.

---

## 🌳 Decision Tree Structure

Start
↓
Did you complete your main task today?
├── Yes
│ ↓
│ Were you satisfied with your performance?
│ ├── Yes
│ │ → Output: "Great job! Maintain consistency."
│ │
│ └── No
│ → Output: "You completed the task, but try improving quality tomorrow."
│
└── No
↓
What was the main reason?
├── Distraction
│ → Output: "You were distracted. Try Pomodoro technique or reduce screen time."
│
├── Lack of Planning
│ → Output: "Plan your day in advance using a to-do list or priority matrix."
│
├── Low Energy
│ → Output: "Focus on sleep, hydration, and breaks to improve energy."
│
└── Other
→ Output: "Identify the issue and create a small improvement plan for tomorrow."



---

## 🔹 Question → Hypothesis → Experiment

### 1. Question
- Did I complete my main task today?
- Was I satisfied with my performance?
- If not, what was the reason?

### 2. Hypothesis
- Distraction → interruptions reduced productivity  
- Lack of planning → unclear priorities caused delay  
- Low energy → fatigue affected performance  

### 3. Experiment
- Use Pomodoro technique (25-minute focus sessions)  
- Create a daily to-do list  
- Improve sleep and take breaks  

---

## 🔹 Sample Test Cases

### ✅ Case 1
**Input:**
- Task Completed: Yes  
- Satisfaction: Yes  

**Output:**  
"Great job! Maintain consistency."

---

### ✅ Case 2
**Input:**
- Task Completed: No  
- Reason: Distraction  

**Output:**  
"You were distracted. Try Pomodoro technique or reduce screen time."

---

### ✅ Case 3
**Input:**
- Task Completed: No  
- Reason: Lack of Planning  

**Output:**  
"Plan your day in advance using a to-do list or priority matrix."

---

## 🔹 Pseudocode

```python
if task_completed == "yes":
    if satisfied == "yes":
        output = "Great job! Maintain consistency."
    else:
        output = "Improve quality or focus tomorrow."
else:
    if reason == "distraction":
        output = "Use Pomodoro technique."
    elif reason == "planning":
        output = "Create a to-do list."
    elif reason == "energy":
        output = "Improve sleep and take breaks."
    else:
        output = "Identify issue and improve."


🔹 Guardrails
Only predefined inputs allowed (Yes/No, Distraction/Planning/Energy/Other)
Fully rule-based logic (no AI randomness)
No assumptions beyond user input
Same input always gives same output


🔹 Part B (Optional)
Not implemented. Can be extended into an AI chatbot in future.

🔹 Conclusion

This system provides a simple, structured way to reflect on daily productivity and generate actionable improvements using deterministic logic.






