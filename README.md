📘 Daily Reflection Decision Tree Assignment


🔹 Overview

This assignment focuses on building a deterministic decision tree system that helps users reflect on their daily productivity using a structured framework:

Question → Hypothesis → Experiment

The system takes user inputs about their day and provides logical, rule-based suggestions for improvement.

🔹 Part A: Decision Tree (Deterministic System)
✅ Objective

To analyze a user’s day based on task completion, satisfaction, and challenges, and provide actionable suggestions.

🌳 Decision Tree Structure
Start
 ↓
Did you complete your main task today?
 ├── Yes
 │    ↓
 │    Were you satisfied with your performance?
 │        ├── Yes
 │        │    → Output: "Great job! Maintain consistency."
 │        │
 │        └── No
 │             → Output: "You completed the task, but try improving quality or focus tomorrow."
 │
 └── No
      ↓
      What was the main reason?
          ├── Distraction
          │     → Output: "You were distracted. Try Pomodoro technique or reduce screen time."
          │
          ├── Lack of Planning
          │     → Output: "Plan your day in advance using a to-do list or priority matrix."
          │
          ├── Low Energy
          │     → Output: "Focus on sleep, hydration, and breaks to improve energy."
          │
          └── Other
                → Output: "Identify the issue and create a small improvement plan for tomorrow."
🔹 Question → Hypothesis → Experiment Framework
1. Question
Did I complete my main task today?
Was I satisfied with my performance?
If not, what was the reason?
2. Hypothesis
If distracted → productivity decreased due to interruptions
If no planning → unclear priorities caused delay
If low energy → physical/mental fatigue affected output
3. Experiment
Use Pomodoro technique (25 min focus sessions)
Create a daily to-do list before starting work
Improve sleep schedule and take regular breaks
🔹 Sample Test Cases
✅ Case 1

Input:

Task Completed: Yes
Satisfaction: Yes

Output:

"Great job! Maintain consistency."

✅ Case 2

Input:

Task Completed: No
Reason: Distraction

Output:

"You were distracted. Try Pomodoro technique or reduce screen time."

✅ Case 3

Input:

Task Completed: No
Reason: Lack of Planning

Output:

"Plan your day in advance using a to-do list or priority matrix."

🔹 Pseudocode Implementation
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
🔹 Guardrails to Prevent AI Hallucination

To ensure the system remains deterministic and reliable:

Restricted Inputs Only
Task Completed → Yes / No
Satisfaction → Yes / No
Reason → Distraction / Planning / Energy / Other
Rule-Based Logic
No dynamic or AI-generated responses
Outputs are predefined and mapped to inputs
No Assumptions
System does not infer beyond given input
Only explicit user choices are considered
Consistent Output
Same input always produces same output
🔹 Part B (Optional - Not Implemented)

The AI Agent component is optional and has not been implemented.
However, the current system can be extended into an AI chatbot that asks questions interactively and provides suggestions.

🔹 Conclusion

This decision tree provides a simple yet effective way to analyze daily productivity using structured reasoning. It ensures clarity, consistency, and actionable insights without relying on complex AI models.
