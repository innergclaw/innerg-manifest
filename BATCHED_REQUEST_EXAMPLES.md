# BATCHED REQUEST EXAMPLES — Copy & Paste These

> Real examples showing old vs new format
> Use these as templates

---

## EXAMPLE 1: Tracker Update (OLD vs NEW)

### ❌ OLD WAY (6 messages, 45K tokens)
```
You: Add this image to a tracker
Me: Which tracker?
You: Vivian
Me: What should the caption be?
You: Logo concept approved
Me: What stage?
You: Move to Revisions
Me: Pushing now...
```

### ✅ NEW WAY (1 message, 8K tokens)
```
Vivian tracker update:
- Add images: preview-3.jpg (final logo approved)
- Stage: Review → Revisions
- Timeline: "Client approved mark — proceeding to final files"
- Push: yes
```

**Result:** Done in 1 message. URL returned.

---

## EXAMPLE 2: Multi-Client Update

### ✅ BATCHED REQUEST
```
Update all trackers:

HELENA:
- Add preview-4.jpg (brand guidelines)
- Stage stays: Revisions
- Timeline: "Brand guide delivered"

VIVIAN:
- Stage: Revisions → Launch
- Timeline: "Final files delivered"

JAMAL:
- Add reference-4.jpg (client feedback)
- Stage stays: Design

Push all: yes
```

**Result:** 3 trackers updated, 1 push, 1 message.

---

## EXAMPLE 3: Git Operations

### ❌ OLD WAY
```
You: Push the changes
Me: Which files?
You: All of them
Me: Commit message?
You: "Updates"
Me: Pushing...
```

### ✅ NEW WAY
```
Git push shopnasgfx-tracker:
- Files: all
- Commit: "feat: add Vivian final logo + Helena brand guide"
- Push: yes
```

**Result:** Committed and pushed. Link returned.

---

## EXAMPLE 4: New Client Setup

### ✅ SINGLE MESSAGE SETUP
```
New client tracker:
- Name: Marcus Johnson
- Business: MJ Fitness
- Service: Logo + Brand Identity
- Amount: $299
- Status: Deposit paid ($100)
- Email: mj@email.com
- Notes: Wants bold, athletic style, red/black colors
```

**Auto-actions:**
1. Create tracker directory
2. Generate HTML
3. Add to admin dashboard
4. Update MEMORY.md
5. Push to GitHub
6. Return URLs

**Result:**
```
Tracker: https://innergclaw.github.io/shopnasgfx-tracker/marcus/
Admin: https://innergclaw.github.io/shopnasgfx-tracker/admin/
Memory: Updated
```

---

## EXAMPLE 5: Content Creation

### ✅ BATCHED CONTENT REQUEST
```
Create Instagram post:
- Topic: New ShopNasGfx tracker system
- Hook: "Clients never ask 'where's my stuff?' anymore"
- Body: Explain tracker benefits, auto-updates, approval flow
- CTA: "Link in bio to see example"
- Tone: Professional but confident
- Length: Short (2-3 sentences)
- Hashtags: 5 relevant ones
```

**Result:** Full caption ready to copy/paste.

---

## EXAMPLE 6: Betting Tracker

### ✅ SINGLE MESSAGE
```
Day 10 parlay:
- Wager: $30
- Odds: +275
- Legs: 3 (DET +1.5, CLE ML, Under 8.5)
- Potential: $112.50
- Status: Pending
- Screenshot attached
```

**Auto-actions:**
1. Extract details from image (if needed)
2. Add to daily-picks.html
3. Update stats
4. Push live

**Result:** https://innergclaw.github.io/outs-and-odds-thankyou/prop-of-the-day/

---

## EXAMPLE 7: Complex Multi-Task

### ✅ STRATEGIC BATCH
```
ShopNasGfx system upgrade:
1. Make all tracker images clickable (full view)
2. Add ntfy notifications to Herk tracker (when payment comes)
3. Update admin dashboard with new revenue stats
4. Create template for "new client" workflow
5. Push everything live

Priority: High
Confirm before push: no (just do it)
```

**Result:** Full system update, 1 push, 1 message.

---

## 🎯 THE PATTERN

**Every message should include:**
1. **What** you want done
2. **Specifics** (files, names, values)
3. **Decisions** (push yes/no, approve approach)
4. **Context** only if necessary

**Never:**
- Ask "can you..." (just state it)
- Send one file at a time
- Wait for confirmation on obvious steps
- Use 6 messages for 1 task

**Always:**
- Batch related tasks
- Assume competence (I'll ask if unclear)
- Trust the automation
- Optimize for throughput

---

> "One message. Full context. No back-and-forth." — The New Way
