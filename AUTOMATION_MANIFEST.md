# AUTOMATION MANIFEST — InnerG Claw

> Operational framework for high-output, low-token workflows
> Version 1.0 — April 16, 2026

---

## 🎯 THE NEW RULES

### 1. BATCHED REQUEST FORMAT

**OLD WAY (High Tokens):**
```
You: "Add image to tracker"
Me: "Done, which tracker?"
You: "Vivian's"
Me: "Done, what's the caption?"
You: "Logo concept"
Me: "Done, push live?"
You: "Yes"
= 6 messages, 45K tokens
```

**NEW WAY (Low Tokens):**
```
You: "Vivian tracker: add preview-1.jpg (black logo) and preview-2.jpg (metallic), 
      update stage to Review, add timeline 'Previews added 2026-04-16', push live"
Me: "Done. https://.../vivian/ updated. 3 changes, 8K tokens"
= 1 message, 8K tokens
```

---

## 📋 BATCHED REQUEST TEMPLATES

### Template A: Tracker Update (Full)
```
[CLIENT] tracker:
- Add images: [file1.jpg] ([desc]), [file2.jpg] ([desc])
- Update stage: [Current] → [New]
- Timeline: [Entry text]
- Push: [yes/no]
```

### Template B: Git Operations
```
Git push [repo]:
- Files: [list or "all"]
- Commit: "[message]"
- Push: [yes/no]
```

### Template C: Multi-Client Update
```
Update trackers:
- Helena: [changes]
- Vivian: [changes]
- Jamal: [changes]
- Push all: [yes/no]
```

### Template D: Content Creation
```
Create [type]:
- Topic: [subject]
- Tone: [professional/casual/punchy]
- Length: [short/medium/long]
- Include: [specific points]
- Output: [deliverable format]
```

---

## 🤖 AUTOMATION LEVELS

### LEVEL 1: Direct Execution (No Subagents)
**Use for:** Simple file edits, git ops, status checks
**Token cost:** 500-4K
**Examples:**
- Single file edit
- Git commit/push
- URL lookup
- Memory search

### LEVEL 2: Batched Execution (1 Subagent)
**Use for:** Multi-file updates, standard tracker builds
**Token cost:** 8K-20K
**Examples:**
- Tracker with images + stage update + timeline
- 3-5 file coordinated changes
- Batch git operations across repos

### LEVEL 3: Complex Orchestration (Multiple Subagents)
**Use for:** System builds, multi-repo coordination
**Token cost:** 25K-50K
**Examples:**
- Build new tracker from scratch
- Restructure entire website
- Cross-project automation setup

### LEVEL 4: Strategic Design (Main Session Only)
**Use for:** Architecture decisions, new systems
**Token cost:** 10K-30K (no subagents)
**Examples:**
- Design new automation workflow
- Plan Neo node architecture
- Strategic pivots

---

## 🚫 TOKEN WASTE PATTERNS (STOP DOING)

| Pattern | Why It Burns Tokens | Fix |
|---------|---------------------|-----|
| "Show me the file" → "Now edit it" | Double context load | "Edit [file] to [exact change]" |
| "Update tracker" → "Which one?" → "Vivian's" → "What changes?" | 4 messages for 1 task | Batch everything in first message |
| Spawning subagent for single git push | 20K overhead for 500 token task | Direct execution |
| "Is this good?" → "Yes" → "Push it" | Confirmation loops | "Push if looks correct" or trust |
| Vision model for every image | 10K per image | Text description when possible |

---

## ✅ TOKEN EFFICIENCY PATTERNS (DO THIS)

| Pattern | Tokens Saved | Example |
|---------|--------------|---------|
| Batch 5 tracker updates | ~80K | One message, 5 changes |
| Direct git vs subagent | ~18K | `git add -A && git push` |
| Memory search vs file read | ~2K | `memory_search` tool |
| Turbo model for simple | ~50% | Default to glm-5-turbo |
| Skip confirmations | ~5K per | "Push live" not "Should I push?" |

---

## 🔄 AUTOMATED WORKFLOWS (Set & Forget)

### Workflow 1: New Client Tracker
**Trigger:** You send client details
**Auto-actions:**
1. Create tracker directory
2. Generate HTML from template
3. Add to admin dashboard
4. Update MEMORY.md
5. Push to GitHub
6. Return tracker URL

**Your input:**
```
New client: [Name], [Business], [Service], [$Amount], [Status]
Reference: [image if any]
```

**My output:**
```
Tracker live: [URL]
Admin updated: [URL]
Memory updated: [Entry]
```

---

### Workflow 2: Daily Betting Tracker
**Trigger:** You send parlay screenshot
**Auto-actions:**
1. Extract details from image (if needed)
2. Add to daily-picks.html
3. Update stats
4. Push live

**Your input:**
```
Day [X]: [Wager] → [Potential], [Legs description], [Status]
```

**My output:**
```
Added: [URL]
```

---

### Workflow 3: Client Feedback → Auto-Update
**Trigger:** Client types "APPROVED" in tracker
**Auto-actions:**
1. Detect approval keyword
2. Move stage forward
3. Add timeline entry
4. Send you ntfy notification
5. Update admin dashboard

**Your involvement:** None (fully automated)

---

## 🧠 WHAT YOU SHOULD DELEGATE TO NEO

**Neo handles (no tokens, just execution):**
- Git commits/pushes
- File copying between projects
- Image optimization
- Basic HTML edits (text swaps)
- Cron job execution
- Local server hosting
- Backup/sync operations

**Main MacBook handles (tokens for thinking):**
- Strategy decisions
- Complex design work
- Client communication
- New system architecture
- Creative direction

---

## 📊 EXPECTED SAVINGS

| Metric | Before | After | Savings |
|--------|--------|-------|---------|
| Messages per task | 6-10 | 1-2 | 80% |
| Tokens per tracker update | 45K | 8K | 82% |
| Session total | 164K | ~40K | 75% |
| Time to complete | 30 min | 5 min | 83% |

---

## 🚀 IMPLEMENTATION CHECKLIST

- [ ] User adopts batch request format
- [ ] Neo node fully configured for execution
- [ ] Automated workflows deployed
- [ ] Confirmation loops eliminated
- [ ] Memory.md caching optimized
- [ ] Subagent spawning minimized

---

> "Evolution favors action. Batch the action. Automate the routine." — InnerG
