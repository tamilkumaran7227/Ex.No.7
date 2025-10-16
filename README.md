# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

### Date: 16.10.2025
### Register no: 212222030007

# Aim: 
To develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.

# Explanation: 
Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."
### Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.

# Title:

Designing a Personal Productivity Assistant Using Natural Language Interaction

# Objective:

To design and simulate a Personal Productivity Assistant (PPA) that manages daily tasks, schedules reminders, suggests wellness tips, answers general queries, and adapts to user preferences using an LLM such as ChatGPT.

# Core requirements:

| Feature                          | Description                                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Task Management**              | Accept tasks via natural language (e.g., “Remind me to call mom at 6 PM”), support deadlines, priorities, and provide daily summaries. |
| **Smart Scheduler**              | Schedule meetings/events, detect conflicts, and suggest alternative time slots.                                                        |
| **Wellness Tips Generator**      | Suggest hydration, posture, and breathing exercises based on context and prior responses.                                              |
| **General Query Answering**      | Respond to simple factual or contextual questions naturally.                                                                           |
| **Personalization & Adaptation** | Store preferences (tone, work hours) and learn from user interactions (e.g., frequent snoozes).                                        |
| **Natural Language Interface**   | Understand everyday language and respond conversationally.                                                                             |
| **Memory Simulation**            | Retain user settings and adapt responses accordingly over time.                                                                        |

# System Design Overview:

## Architecture

Input Module – Accepts natural-language commands.

Intent Parser – Classifies input into intents: Task, Schedule, Wellness, Preference, Query.

Action Handler – Executes intent logic and updates memory.

Memory Store – Maintains user preferences, snooze stats, and task list.

Response Generator (LLM) – Produces natural conversational replies.

Feedback Loop – Updates user model when preferences change.

# Prompt Templates Used with LLM:

| Task               | Prompt Template                                                                                                         |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| **System Prompt**  | “You are a helpful Personal Productivity Assistant. Be concise and friendly.”                                           |
| **Add Task**       | `User: "{user_text}"`<br>`Assistant: Extract task title, due date/time, priority, and create a JSON task object.`       |
| **Schedule Event** | `User: "{user_text}"`<br>`Assistant: Parse event title, proposed time, detect conflicts, and suggest alternatives.`     |
| **Wellness Tip**   | `User context: {context}`<br>`Assistant: Suggest a short wellness tip and one action button (e.g., Start/Snooze).`      |
| **General Query**  | `User question: "{user_text}"`<br>`Assistant: Provide a short helpful answer and, if relevant, a follow-up suggestion.` |

# Simulation Procedure:

## Input Handling:
The system receives user inputs such as:

“Remind me to call mom at 6 PM”

“I’m feeling stressed”

“Set work hours 10:00–18:00”

## Intent Classification:
Based on keywords and structure, the system decides if it’s a task, event, wellness query, etc.

## Response Generation:
The assistant forms natural responses using templates and stored preferences.

## Preference Adaptation:

Updates tone (“Use concise tone”)

Adjusts working hours

Records snooze or tip acceptance rates

## Output Simulation:
The final transcript and memory data are generated and stored.

# Output:

## Task Manager
```
User: Remind me to call mom at 6 PM  
Assistant: ✅ Got it — I added "Call mom" to your tasks. Due today at 6:00 PM. Would you like a reminder before it's due? (Yes/No)
```

## Smart Scheduler
```
User: Schedule meeting with Priya tomorrow at 3 PM  
Assistant: Scheduled "Meeting with Priya" at 3 PM for 1 hour.
```

## Wellness Suggestion
```
User: I'm feeling stressed  
Assistant: Try a 2-minute guided breathing exercise. Shall I start a session now? (Start/Snooze)

```

## Preference Update
```
User: Set work hours 10:00–18:00  
Assistant: Work hours updated to 10:00–18:00.

```

## Adaptive Response
```
User: Use concise tone  
Assistant: Got it — I'll keep responses concise.

```

# Adaptation Mechanism:

Maintains a JSON-based memory with fields like:
```
{
  "preferences": {
    "preferred_tone": "concise",
    "work_hours": {"start": "10:00", "end": "18:00"},
    "snooze_counts": {"stretch": 3}
  }
}
```
If a wellness tip is repeatedly snoozed, the assistant delays its frequency.

Tone changes immediately affect all future responses.

# Output Summary:

| Component                   | Example Behavior                                           |
| --------------------------- | ---------------------------------------------------------- |
| **Daily Task Manager**      | Creates and lists tasks with due dates.                    |
| **Smart Scheduler**         | Adds events, detects overlaps, proposes alternate slots.   |
| **Wellness Tips Generator** | Suggests context-aware health reminders.                   |
| **Preference Adaptation**   | Learns tone, work hours, and wellness timing.              |
| **LLM Interaction**         | Natural, conversational replies based on prompt templates. |



# Result: 
The lab exercise resulted in the creation of a prototype concept for a personal assistant powered by large language models. Students were able to:
 Understand how to tailor LLM prompts to real-life applications.
 Foster creativity by designing features suited to their personal or academic lives.
 Learn prompt engineering techniques for optimal interaction with AI tools.
 Experience the versatility and utility of generative AI in solving everyday problems.
