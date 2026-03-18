# 🤖 Life OS Agents

| Agent | Area | Skill File |
|-------|------|-----------|
| 📚 **Academics Agent** | INSEAD coursework, assignments, exam prep | [SKILL.md](./skills/academics/SKILL.md) |
| 💼 **Everhaus Agent** | Part-time job, task management, deliverables | [SKILL.md](./skills/everhaus/SKILL.md) |
| 💪 **Gym Agent** | Training logs, progressive overload, planning | [SKILL.md](./skills/gym/SKILL.md) |
| 🧩 **Case Interview Agent** | Mock cases, feedback analysis, next-steps | [SKILL.md](./skills/case-interviews/SKILL.md) |
| 🚀 **Git Operations** | Version control & repository synchronization | [SKILL.md](./skills/git-ops/SKILL.md) |

## Activation (Slash Commands)

Type these in Antigravity to switch agents:

| Command | Agent | Scope |
|---------|-------|-------|
| `/academics` | 📚 Academics Agent | INSEAD coursework, assignments, exams |
| `/everhaus` | 💼 Everhaus Agent | Part-time job, tasks, deliverables |
| `/gym` | 💪 Gym Agent | Training logs, progressive overload |
| `/case-interview` | 🧩 Case Interview Agent | Mock cases, feedback analysis, next-steps |
| `/git-ops [message]` | 🚀 Git Operations | Commit and push to remote |

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
