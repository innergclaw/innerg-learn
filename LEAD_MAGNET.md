# OpenClaw Setup in 30 Minutes
## Free Quick-Start Guide

---

## What You'll Learn

By the end of this guide, you'll have:
- ✅ OpenClaw installed and running
- ✅ Your first AI agent configured
- ✅ A working memory system
- ✅ One custom skill installed

**Time required:** 30 minutes
**Skill level:** Beginner (no coding required)

---

## Step 1: Install OpenClaw (5 min)

### macOS
```bash
npm install -g openclaw
openclaw gateway start
```

### Windows
```bash
npm install -g openclaw
openclaw gateway start
```

### Linux
```bash
npm install -g openclaw
openclaw gateway start
```

**Verify installation:**
```bash
openclaw status
```

You should see: `Gateway: RUNNING`

---

## Step 2: Configure Your Agent (10 min)

Open your workspace folder:
```bash
cd ~/.openclaw/workspace
```

Create your identity files:

### IDENTITY.md
```markdown
# Who You Are
- Name: [Your Agent Name]
- Type: Personal Assistant
- Purpose: Help with [specific tasks]
```

### USER.md
```markdown
# About Your Human
- Name: [Your Name]
- Timezone: [Your Timezone]
- Preferences: [How you like to work]
```

### MEMORY.md
```markdown
# Long-Term Memory
Store important information here.
```

---

## Step 3: Set Up Memory (5 min)

Create the memory folder:
```bash
mkdir -p memory/episodic
```

Create today's log:
```bash
touch memory/episodic/$(date +%Y-%m-%d).md
```

Your agent now has:
- **Long-term memory** (MEMORY.md)
- **Daily logs** (memory/episodic/)
- **Context awareness** (reads these files each session)

---

## Step 4: Install Your First Skill (5 min)

Browse available skills:
```bash
openclaw skills list
```

Install a useful one:
```bash
openclaw skills install weather
```

Test it:
```
You: What's the weather in Philadelphia?
Agent: *uses weather skill to get real data*
```

---

## Step 5: Test Everything (5 min)

Start a chat with your agent:
```bash
openclaw chat
```

Try these test prompts:
1. "What do you know about me?"
2. "What's the weather today?"
3. "Remember that I prefer concise responses"

If all three work, you're set! 🎉

---

## What's Next?

Now that you have a working agent, you can:

1. **Add more skills** — weather, calendar, web search
2. **Set up automations** — cron jobs, heartbeat monitoring
3. **Connect APIs** — email, social media, databases
4. **Build custom skills** — for your specific workflow

---

## Want to Go Deeper?

**InnerG Learn** offers 1-on-1 training:

- **Single Session ($150)** — Get unstuck on ONE thing
- **Full Program ($300)** — Build complete AI automation system

📧 innergclaw@gmail.com  
🔗 innergclaw.github.io/innerg-learn

---

## Common Issues

**"npm command not found"**
→ Install Node.js first: nodejs.org

**"Gateway won't start"**
→ Check if port 3000 is in use: `lsof -i :3000`

**"Agent doesn't remember anything"**
→ Make sure MEMORY.md and memory/ folder exist

**"Skills won't install"**
→ Check your internet connection and try again

---

*This guide is free. Share it. Use it. Build cool stuff.*

**— InnerG Intel**
