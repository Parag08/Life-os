# 🤖 Life OS Agents

Each life area has a dedicated AI agent with its own context, skills, and operating protocol.

## Available Agents

| Agent | Area | Skill File |
|-------|------|-----------|
| 📚 **Academics Agent** | INSEAD coursework, assignments, exam prep | [SKILL.md](./academics/SKILL.md) |
| 💼 **Everhaus Agent** | Part-time job, task management, deliverables | [SKILL.md](./everhaus/SKILL.md) |
| 💪 **Gym Agent** | Training logs, progressive overload, planning | [SKILL.md](./gym/SKILL.md) |
| 🧩 **Case Interview Agent** | Mock cases, feedback analysis, next-steps | [SKILL.md](./case-interviews/SKILL.md) |

## How to Activate an Agent

When starting a conversation, tell Antigravity which agent you want:

> *"I want to work with the **Case Interview Agent**"*  
> *"Switch to the **Gym Agent**"*  
> *"Activate the **Academics Agent**"*

The agent will read its `SKILL.md` and operate within that domain only.

## Agent Isolation

Each agent is scoped to its area:
- They won't give advice outside their domain
- They maintain their own file areas in the repo
- They each have specific command vocabularies (see each SKILL.md)
