# Vibe Coding Quick Start Guide
**For first-time builders who want to ship something today**

This is the streamlined version. Want more depth? Check out the [Comprehensive Guide](./vibe_coding_framework_v1_updated.md).

---

## What is Vibe Coding?

Vibe coding is building software through conversation with AI. Instead of writing code yourself, you describe what you want in plain language, see what the AI builds, and iterate until it works.

Think of it like working with a really fast junior developer who:
- ✅ Understands natural language
- ✅ Builds things instantly
- ✅ Never gets tired of changes
- ❌ Needs clear instructions
- ❌ Sometimes misunderstands what you want
- ❌ Can't make product decisions for you

**You DON'T need:**
- Coding experience
- Technical background
- Computer science degree

**You DO need:**
- Clear idea of the problem you're solving
- Patience to iterate (first version won't be perfect)
- Willingness to test and get feedback

---

## Before You Start (5 minutes)

Answer these three questions. Seriously - write them down.

### 1. What problem am I solving?

**Bad:** "We need better customer management"  
**Good:** "Sales reps forget to follow up with leads, causing us to lose deals"

Be specific. Use a real example:
- "It takes our team 2 hours to create the weekly report manually"
- "Customers can't track their order status, so they email us constantly"

**Your turn:** _______________________________________________

### 2. Who is this for?

**Bad:** "Business users"  
**Good:** "Sales reps who are always on the road, use mobile primarily, and hate complex software"

Think about:
- Role: [Specific job title]
- Context: [When/where they'll use this]
- Tech comfort: [Low/Medium/High]

**Your turn:** _______________________________________________

### 3. How will I know it works?

**Bad:** "Users like it"  
**Good:** "3 test users can complete the main task in under 2 minutes without help"

Make it measurable:
- "5 team members use it daily"
- "Reduces task time from 30 min to 5 min"
- "Users rate it 7+ out of 10"

**Your turn:** _______________________________________________

💡 **Pro Tip:** If you can't answer these clearly, spend 10 more minutes thinking. Every minute here saves 30 minutes later.

---

## Setup: Choose Your Workspace (5 minutes)

For your first project, use **Claude.ai Artifacts** (the simplest option).

### Option 1: Claude.ai Artifacts (Recommended for Beginners)

**Best for:**
- Your first vibe coding project
- Single-page apps, forms, dashboards
- Quick demos (1-2 session builds)

**Setup:**
1. Go to claude.ai
2. Start a new conversation
3. That's it! No installation needed

**You'll see:** A preview panel appears on the right when Claude builds your app.

### Option 2: Claude.ai Projects (For Multi-Day Work)

**Use this when:**
- Building over multiple days
- Need to reference documents
- Want to save progress between sessions

**Setup:**
1. Go to claude.ai
2. Click "Projects" in sidebar
3. Create new project with descriptive name
4. Start chatting within the project

💡 **Pro Tip:** Start with Artifacts. You can always move to Projects later.

---

## Pressure-Test Your Idea (10 minutes)

Before building, let Claude poke holes in your thinking. This catches problems early.

**Copy this template into Claude:**

```
I'm planning to build [type of tool/app].

CONTEXT:
Problem: [Your problem from above]
Target users: [Your user from above]  
Success looks like: [Your success metric from above]

CHALLENGE THIS IDEA:
1. What am I assuming that might be wrong?
2. What are 3 simpler alternatives I haven't considered?
3. What will be hardest to build?
4. Is there an existing tool I should use instead?

Be skeptical and direct. I want to know if this is a bad idea before I invest time.
```

**What to look for:**
- 🚩 "This might be too complex for a prototype"
- 🚩 "Existing tool X already does most of this"
- 🚩 "The hardest part will be [thing you underestimated]"

**Common outcomes:**
1. Claude confirms it's feasible → Great! Continue
2. Claude suggests simplifications → Update your plan
3. Claude identifies missing pieces → Add them now
4. Claude recommends alternatives → Investigate first

⚠️ **Red Flag:** If Claude says "this requires [authentication/payments/complex integrations]", consider simplifying or using existing tools for those parts.

---

## Your First Build Session

### Step 1: Your First Prompt (Use This Template)

```
I want to build [one-sentence description].

CONTEXT:
Users: [Who they are and key traits]
Problem it solves: [Specific problem]
Success looks like: [What success means]

TECHNICAL:
- Device: [Mobile/Desktop/Both]
- Keep it simple (no complex features yet)

LET'S START WITH:
[Just ONE feature - the most important one]

Specifically, I want:
- [Specific detail]
- [Specific detail]
- [Specific detail]

Design: [Clean/modern/simple/etc.]

Please build this first feature and ask clarifying questions if anything is unclear.
```

**Real Example:**
```
I want to build a simple customer feedback form where people can submit product feedback.

CONTEXT:
Users: B2B customers (technical and non-technical)
Problem it solves: Feedback currently scattered across emails and Slack
Success looks like: Customer can submit feedback in under 60 seconds

TECHNICAL:
- Device: Mobile-first but works on desktop
- Keep it simple (no complex features yet)

LET'S START WITH:
Build the feedback submission form.

Specifically, I want:
- Fields: Name (optional), Email (required), Feedback message (textarea), Category (dropdown: Bug Report, Feature Request, General Feedback)
- Submit button that shows success message after submission
- Form validation (proper email format, message can't be empty)

Design: Clean and modern, friendly (not corporate-looking)

Please build this first feature and ask clarifying questions if anything is unclear.
```

### Step 2: Build One Feature at a Time

The cycle looks like this:

```
┌─────────────────────────────────────┐
│    1. DESCRIBE what you want        │
│    (Be specific and clear)          │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│    2. REVIEW what Claude built      │
│    (Look at the preview)            │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│    3. TEST it yourself              │
│    (Click, type, interact)          │
└──────────────┬──────────────────────┘
               │
               ▼
┌─────────────────────────────────────┐
│    4. GIVE FEEDBACK                 │
│    ("Change X because...")          │
└──────────────┬──────────────────────┘
               │
               └──────> Repeat until it works
```

**After first feature works:**
```
Now let's add [next feature].

What it should do:
- [Specific behavior]
- [Specific behavior]

Keep the existing [previous feature] working.
```

### Step 3: Quality Checkpoints

After every 2-3 features, pause and test thoroughly:

**Quick Check:**
- [ ] Can you complete the main task without errors?
- [ ] Did you test on mobile (resize browser window)?
- [ ] Does it handle empty/invalid inputs?
- [ ] Is anything confusing or broken?

**Ask Claude:**
```
Please review what we've built so far:
1. What are the main parts?
2. Any potential issues?
3. Any security concerns I should know about?
```

---

## Test with Real Users (Critical!)

Don't skip this. Seriously. You'll learn more in 30 minutes of user testing than 3 hours of building alone.

### Who Should Test?
- 2-3 people who match your target user
- They should be unfamiliar with your project
- Available for 15-30 minutes

### How to Test

**1. Set up the test:**
- Share the Claude Artifacts link (or screen share)
- Don't explain how it works
- Ask them to complete the main task

**2. Script to use:**
```
"Hi! I built a prototype and want to see if it makes sense. 
I'm testing the tool, not you, so there are no wrong answers. 
Please think out loud as you use it.

[Brief context]: This tool is for [brief description].

Task: I'd like you to [realistic task]. Take your time, 
and let me know if anything is confusing."
```

**3. Watch for:**
- Where do they pause or hesitate?
- Do they re-read instructions?
- Do they accomplish the task?
- What do they say out loud?

**Don't:**
- ❌ Help them or give hints
- ❌ Explain how it works
- ❌ Interrupt their process

**4. Follow-up questions:**
- "What do you think this tool does?"
- "On a scale of 1-10, how easy was that?"
- "What was most confusing?"
- "Would you actually use this?"

### Analyze the Feedback

**Look for patterns:**
- If 2+ users struggle with same thing → Fix it
- If everyone completes successfully → Polish and ship
- If no one completes the task → Redesign needed

**Decision framework:**
- ✅ **Users complete task easily** → Polish minor issues, then share
- ⚠️ **Users complete after struggling** → Fix friction points, test with 1-2 more users
- 🚩 **Users can't complete** → Major redesign needed, revisit your problem definition

---

## Prompting Patterns That Work

### The Simple Request
```
Add a [specific feature] that [does specific thing].
Make it [style preference].
```

Example: "Add a download button that saves the invoice as PDF. Make it green and prominent."

### When Something Breaks
```
The [specific thing] isn't working. When I [action], it [wrong behavior].
Expected: [what should happen]
```

Example: "The download button isn't working. When I click it, nothing happens. Expected: PDF should download."

### When You're Stuck
```
I need to [accomplish something] but I'm not sure how.
Please suggest 2-3 simple approaches and explain the trade-offs.
```

### The Simplify Request
```
This feels too complex. Can you simplify it to just the essential functionality?
```

---

## Common Beginner Mistakes

### ❌ Mistake 1: Skipping Problem Definition
Jumping straight to building without clear answers to the 3 questions.

**Result:** You build something nobody needs or can't measure success.

**Fix:** Spend 5 minutes on the 3 questions before touching Claude. Write them down.

### ❌ Mistake 2: Building Everything at Once
Starting with "build a complete X with features A, B, C, D..." leads to overwhelming code you can't debug.

**Result:** Complex, buggy code that breaks constantly.

**Fix:** Build one tiny feature. Test it. Then add the next piece.

### ❌ Mistake 3: No User Testing
Building something you think is great but users find confusing.

**Result:** You waste time polishing something that doesn't solve the problem.

**Fix:** Test with 2-3 target users after your core features work. Watch them use it without helping.

### ❌ Mistake 4: Vague Instructions
"Make it better" or "fix the design" gives AI nothing to work with.

**Result:** Claude makes random changes that don't address your real concern.

**Fix:** Be specific. "Make the text larger (18px)" or "Change button color to blue (#4A90E2)."

### ❌ Mistake 5: Accepting First Output Without Testing
AI code usually needs 2-3 rounds of refinement.

**Result:** Subtle bugs and poor UX that compound over time.

**Fix:** Always test. Click every button. Try invalid inputs. Give specific feedback.

### ❌ Mistake 6: Trying to Build Production Systems
Treating this like a replacement for engineering instead of rapid prototyping.

**Result:** You hit walls around security, scale, or complexity.

**Fix:** Accept that vibe coding is for prototypes. Plan to hand off to engineering if it proves valuable.

---

## Your First Project Checklist

Use this for your first build:

### Phase 1: Before Starting (5-10 min)
- [ ] I answered the 3 questions clearly (problem, user, success metric)
- [ ] I pressure-tested my idea with Claude
- [ ] I chose my workspace (Artifacts or Projects)
- [ ] I know what the ONE core feature is

### Phase 2: While Building (2-4 hours)
- [ ] I'm building one small feature at a time
- [ ] I'm testing each piece before moving on
- [ ] I'm giving specific feedback, not vague requests
- [ ] I'm doing quality checkpoints every 2-3 features

### Phase 3: Before Sharing (30-60 min)
- [ ] The main user task works without errors
- [ ] I tested it on both desktop and mobile (resize browser)
- [ ] At least 2-3 target users tested it successfully
- [ ] I made fixes based on user feedback

### Phase 4: Share (10-20 min)
- [ ] I have a shareable link or can demo via screen share
- [ ] I know what worked well and what needs improvement
- [ ] I documented my learnings

---

## Simple Project Ideas to Start

Good first projects (1-3 hours each):

1. **Personal Dashboard** - Shows your daily schedule, weather, and tasks in one page
2. **Simple Calculator** - Specialized for your field (tip calculator, freelance rate calculator, etc.)
3. **Mini Form Builder** - Create and share simple surveys
4. **Text Transformer** - Convert text formats (markdown to HTML, etc.)
5. **File Organizer** - Upload files, auto-categorize them

Start with the absolute simplest version. Add features only after the core works.

---

## When Things Go Wrong

### "Claude Keeps Breaking Previous Features"

**What's happening:** You fix one thing, another breaks. Features that worked now don't.

**Fix:**
```
I'm continuing work on [project].

COMPLETED FEATURES:
✅ [Feature 1] 
✅ [Feature 2]
✅ [Feature 3]

CURRENT ISSUE:
[Specific problem]

Please fix this without breaking existing features. 
Only modify the specific feature I mentioned.
```

### "The Code is Too Complex / I Don't Understand It"

**What's happening:** Code looks overwhelming, you can't explain what it does.

**Fix:**
```
Please explain what you just built:
1. What are the main parts?
2. What does each part do?
3. How do they work together?

Use simple language (I'm not a developer).
```

If still too complex:
```
This feels too complex. Can you rebuild this feature in the simplest possible way?
```

### "A Feature is Taking Forever (2+ Hours)"

**What's happening:** Lots of back-and-forth without progress, feature getting more complex.

**Fix - Simplify:**
```
This feature is taking too long. Let's simplify.

CURRENT: [Complex version]
SIMPLIFIED: [Just the essential parts]

Build the simplified version first.
```

**Fix - Break it down:**
```
Let's break [feature] into smaller steps:

STEP 1: [Smallest possible first step]
Build just this first. I'll test it before we continue.
```

### "I Want to Start Over"

**What's happening:** Project feels messy, or you realized you should approach it differently.

**Fix:** That's fine! You learned something. Start a new conversation and apply what you learned:
- Write a clearer first prompt
- Build in smaller increments  
- Reference what you learned: "I tried X approach before but it got too complex. This time I want to try Y."

### "It Works for Me But Not for Test Users"

**What's happening:** Prototype works on your device but others get errors or confusion.

**Fix - Different device/browser:**
- Test in incognito mode (clears all local data)
- Try on mobile device
- Ask users what device/browser they're using

**Fix - User confusion:**
- Watch where they get stuck (don't interrupt)
- Ask: "What were you expecting to happen?"
- Fix those specific friction points

---

## Next Steps

### After Your First Working Project

**Ask yourself: Did user testing validate the idea?**

**✅ YES - Users completed task & would use it:**

1. **Polish the prototype** (1-2 hours)
   - Fix issues 2+ users mentioned
   - Test with 1-2 more users
   - Make it presentable

2. **Decide what happens next:**
   - **Internal tool?** Set up simple maintenance plan (who updates it when it breaks)
   - **Proving an idea?** Create handoff doc for engineering with: what worked, what users wanted, what to build
   - **Just exploring?** Document learnings and move on

**⚠️ PARTIAL - Users struggled but completed:**

1. **Fix friction points** (1-2 hours)
   - Address specific issues where users hesitated
   - Simplify confusing parts
   
2. **Test with 2-3 new users**
   - See if fixes worked
   - Then decide like "YES" path above

**🚩 NO - Users couldn't complete or wouldn't use it:**

1. **Don't polish** - You might have built the wrong thing
2. **Go back to your 3 questions:**
   - Is this the right problem?
   - Is this the right solution?
   - Who is this really for?
3. **Options:**
   - Start over with simpler approach
   - Solve a different problem
   - Use existing tool instead

### Want to Deploy It?

**For sharing/demos:**
- Claude Artifacts already has a shareable link
- Or use screen share for demos

**For ongoing use:**
Simple options:
- **Vercel** (web apps): Free tier, easy deployment
- **Netlify** (web apps): Drag and drop
- **Replit** (any code): Free hosting with some limitations

Ask Claude: "How do I deploy this to [platform]?"

### Ready for More Depth?

Read the [Comprehensive Vibe Coding Framework](./vibe_coding_framework_v1_updated.md) for:
- Advanced prompting techniques
- Architecture patterns for complex apps
- Production deployment strategies
- Maintenance planning
- Engineering handoff processes
- Complete case studies

---

## Key Mindset Shifts

### 1. You're the Director, Not the Actor
- **You:** Make product decisions, define success, validate with users
- **Claude:** Executes your vision, handles implementation
- **Your job:** Guide, test, decide. NOT write code.

### 2. Iteration is Expected
Your first prompt won't be perfect. That's normal!
- First version: Usually 60-70% right
- After 2-3 iterations: Gets much better
- Most successful features take 5-10 rounds of refinement

### 3. Specificity Beats Cleverness
**Bad:** "Build a user dashboard"  
**Good:** "Create a dashboard showing: total sales this month (big number at top), list of recent orders (last 10), bar chart of sales by day"

More details = better results. Always.

### 4. Test Early, Test Often
Don't wait until "it's done" to test:
- After first feature: Does core idea work?
- After 2-3 features: Can users complete the main task?
- Before sharing: Full usability test with target users

### 5. Simple > Complex
If you can't explain what you built in one sentence, it's probably too complex. When in doubt, simplify.

### 6. Know Your Limits
Vibe coding is for **prototypes**, not production systems.
- ✅ Good for: Validating ideas, demos, simple internal tools
- ❌ Not for: Customer-facing products, payment processing, anything requiring 100+ concurrent users

If your prototype proves valuable, hand it to engineering for proper implementation.

---

## Emergency Simplification Template

When your project feels overwhelming, copy this into Claude:

```
I've overcomplicated this. Let me refocus on the core:

ORIGINAL GOAL: [What you wanted to achieve]

The ONE thing users need to do: [specific action]
The ONE result they need: [specific output]

CURRENT PROBLEM: [Why current approach isn't working]

Please suggest the absolute simplest implementation that achieves just this core functionality.
Ignore all nice-to-have features for now.
```

---

## Key Reminders

### ⏰ Time Guidelines
- Planning (3 questions + pressure test): 10-15 min
- Building your first feature: 30-60 min
- Building each additional feature: 15-45 min
- User testing: 30-60 min
- Total for first project: 2-4 hours

**⚠️ Red Flag:** If a single feature takes 2+ hours, it's too complex. Simplify or break it down.

### 🎯 Success Metrics
Your first project is successful if:
- ✅ You learned how vibe coding works
- ✅ You built something that runs without errors
- ✅ At least 1 person (besides you) tested it
- ✅ You can explain what you built and what you learned

Don't aim for perfect. Aim for done and learned.

---

## Resources

**Essential Reading:**
- [Comprehensive Vibe Coding Framework](./vibe_coding_framework_v1_updated.md) - Deep dive into all phases, complete case studies, troubleshooting
- [Claude.ai Documentation](https://docs.anthropic.com) - Official docs and best practices

**When You Need Help:**
- Try the Troubleshooting section above first
- Ask Claude: "I'm stuck on [specific issue]. Can you help?"
- Start a fresh conversation if Claude seems confused

**Community:**
- Share what you build (Twitter, LinkedIn)
- Teach others (best way to learn)
- Document your learnings

---

## Remember

**Perfect is the enemy of done.**

Your goal isn't to build the perfect application - it's to:
1. **Validate** an idea quickly
2. **Learn** what users actually need
3. **Decide** if it's worth building properly

You can always improve later. For now: Start small. Test with users. Ship something.

**Now stop reading and start building!** 🚀

---

*Quick Start Guide v1.1 - Based on the Comprehensive Vibe Coding Framework*  
*Questions? Improvements? Share your feedback and help make this guide better.*
