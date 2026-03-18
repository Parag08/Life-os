# 🤖 Life OS Agents

## Activation (Slash Commands)

Type these in Antigravity to switch agents:

| Command | Agent | Scope |
|---------|-------|-------|
| `/academics` | 📚 Academics Agent | INSEAD coursework, assignments, exams |
| `/everhaus` | 💼 Everhaus Agent | Part-time job, tasks, deliverables |
| `/gym` | 💪 Gym Agent | Training logs, progressive overload |
| `/case-interview` | 🧩 Case Interview Agent | Mock cases, feedback analysis, next-steps |

## Structure

```
.agents/
├── workflows/                  ← Antigravity slash-command entry points
│   ├── academics.md            ← /academics
│   ├── everhaus.md             ← /everhaus
│   ├── gym.md                  ← /gym
│   └── case-interview.md       ← /case-interview
└── skills/                     ← Agent context, instructions, and protocols
    ├── academics/SKILL.md
    ├── everhaus/SKILL.md
    ├── gym/SKILL.md
    └── case-interviews/SKILL.md
```
