# VIBE CODING FRAMEWORK
## Building Apps with AI: A Guide for Product Managers

**Version 1.0**  
*For non-technical builders who want to turn ideas into working prototypes*

---

# TABLE OF CONTENTS

## PART 1: UNDERSTANDING VIBE CODING
- [What is Vibe Coding?](#what-is-vibe-coding)
- [Who This Guide is For](#who-this-guide-is-for)
- [When to Use (and Not Use) Vibe Coding](#when-to-use-vibe-coding)
- [How This Guide Works](#how-this-guide-works)

## PART 2: GETTING READY
- [Pre-Flight Checklist](#pre-flight-checklist)
- [Setting Up Your Workspace](#setting-up-workspace)
- [The Vibe Coding Mindset](#vibe-coding-mindset)

## PART 3: THE FRAMEWORK

### PHASE 1: THINK BEFORE YOU BUILD (30-60 min)
- [Step 1: Define the Problem](#step-1-define-problem)
- [Step 2: Pressure-Test with AI](#step-2-pressure-test)
- [Step 3: Choose Your Target](#step-3-choose-target)

### PHASE 2: PLAN YOUR BUILD (30-60 min)
- [Step 4: Describe What You Want](#step-4-describe-build)
- [Step 5: Break Down Features](#step-5-break-down-features)
- [Step 6: Prepare Your First Prompt](#step-6-first-prompt)

### PHASE 3: BUILD WITH CLAUDE (2-8 hours)
- [Step 7: Start the Conversation](#step-7-start-conversation)
- [Step 8: The Build-Test-Iterate Loop](#step-8-build-test-iterate)
- [Step 9: Quality Checkpoints](#step-9-quality-checkpoints)

### PHASE 4: VALIDATE (2-4 hours)
- [Step 10: Test with Real Users](#step-10-test-users)
- [Step 11: Analyze Feedback](#step-11-analyze-feedback)
- [Step 12: Polish or Pivot](#step-12-polish-pivot)

### PHASE 5: SHARE & DECIDE (1-2 hours)
- [Step 13: Deploy Your Prototype](#step-13-deploy)
- [Step 14: Plan What's Next](#step-14-whats-next)

## PART 4: COMPLETE WALKTHROUGH
- [Case Study: Building a Customer Feedback Tool](#walkthrough-feedback-tool)

## PART 5: RESOURCES
- [Prompt Library](#prompt-library)
- [Common Scenarios](#common-scenarios)
- [Troubleshooting Guide](#troubleshooting-guide)
- [Glossary](#glossary)

---

# PART 1: UNDERSTANDING VIBE CODING

<a id="what-is-vibe-coding"></a>
## What is Vibe Coding?

Vibe Coding is building software through conversation with AI. Instead of writing code yourself, you describe what you want in plain language, see what the AI builds, and iterate until it works.

Think of it like working with a really fast junior developer who:
- ✅ Understands natural language
- ✅ Builds things instantly
- ✅ Never gets tired of changes
- ❌ Needs clear instructions
- ❌ Sometimes misunderstands what you want
- ❌ Can't make product decisions for you

**Example Conversation:**
```
You: "Create a form where sales reps can log customer calls. 
      Include fields for customer name, call date, and notes."

Claude: [Builds a working form with those fields]

You: "The notes field is too small. Make it bigger and add 
      a character counter."

Claude: [Updates the form]

You: "Perfect! Now add a submit button that shows a success 
      message."

Claude: [Adds the button and success state]
```

That's Vibe Coding. You're guiding, testing, and refining—not writing code.

---

<a id="who-this-guide-is-for"></a>
## Who This Guide is For

**Perfect for:**
- 🎯 Product Managers who want to prototype ideas quickly
- 🎯 Project Managers building internal tools
- 🎯 Sales/Marketing professionals who need simple apps
- 🎯 Anyone with an idea and a willingness to iterate

**You DON'T need:**
- ❌ Coding experience
- ❌ Technical background
- ❌ Computer science degree
- ❌ Understanding of frameworks, databases, or deployment

**You DO need:**
- ✅ Clear idea of the problem you're solving
- ✅ Ability to describe what you want
- ✅ Patience to iterate (first version won't be perfect)
- ✅ Willingness to test and get feedback

---

<a id="when-to-use-vibe-coding"></a>
## When to Use (and Not Use) Vibe Coding

### ✅ Use Vibe Coding For:

**Quick Prototypes**
- Testing an idea before investing engineering time
- Showing "what if we built this?" to stakeholders
- Validating assumptions with working demos

**Simple Internal Tools**
- Sales trackers
- Content calendars
- Simple calculators
- Form builders
- Dashboard prototypes

**Demos & Presentations**
- Investor pitches
- Stakeholder reviews
- User research sessions

**Learning & Exploration**
- Understanding technical constraints
- Exploring UX approaches
- Testing feasibility

### ❌ Don't Use Vibe Coding For:

**Production Systems**
- Customer-facing products (without engineering review)
- Apps with 100+ concurrent users
- Systems handling payments or sensitive data
- Mission-critical internal tools

**Complex Integrations**
- Connecting to multiple existing systems
- Complex business logic with many edge cases
- Apps requiring deep system knowledge

**Compliance Requirements**
- HIPAA, SOC2, GDPR-regulated apps
- Financial services applications
- Healthcare applications

**When You Need:**
- High availability (24/7 uptime)
- Real-time performance at scale
- Advanced security features
- Complex authentication systems

---

<a id="how-this-guide-works"></a>
## How This Guide Works

This guide follows a **5-phase framework**:

```
PHASE 1: THINK → Define problem, test assumptions, choose target
PHASE 2: PLAN → Describe what you want, break down features
PHASE 3: BUILD → Talk to Claude, iterate, checkpoint
PHASE 4: VALIDATE → Test with users, analyze, decide
PHASE 5: SHARE → Deploy, plan next steps
```

**Each phase includes:**
- Clear steps with time estimates
- Real examples and templates
- Common mistakes to avoid
- Checkpoints to ensure quality

**Special features:**
- 🎯 **Reality Checks** - Make sure you're on track
- 💡 **Pro Tips** - Shortcuts that work
- ⚠️ **Red Flags** - Warning signs to watch for
- ✅ **Checkpoints** - Verify before moving forward

**How to use this guide:**
1. Read Part 1-2 first (15 minutes)
2. Follow the framework step-by-step
3. Reference the walkthrough (Part 4) when stuck
4. Use the Prompt Library (Part 5) for copy-paste templates

Let's get started!

---

# PART 2: GETTING READY

<a id="pre-flight-checklist"></a>
## Pre-Flight Checklist

Before you start vibe coding, make sure you have:

### ✅ Prerequisites

**Time & Focus**
- [ ] 30-60 minutes for planning (uninterrupted)
- [ ] 2-8 hours for building (can be spread across days)
- [ ] 2-4 hours for testing with users

**Tools & Access**
- [ ] Claude.ai account (Free or Pro - Pro recommended for complex projects)
- [ ] Modern web browser (Chrome, Firefox, Safari)
- [ ] Way to take screenshots (for sharing progress)

**People & Validation**
- [ ] 2-3 potential users identified for testing
- [ ] Stakeholder who cares about this problem
- [ ] Someone technical to consult if needed (optional but helpful)

**Clarity & Preparation**
- [ ] Clear problem statement (can explain in 1-2 sentences)
- [ ] Specific target user in mind (not "everyone")
- [ ] Examples of similar tools/apps (even if imperfect)
- [ ] Success criteria defined (how you'll know it worked)

### 🎯 Reality Check #1
**Have you used Claude.ai before?**
- **Yes?** Great! Skip to the next section.
- **No?** Spend 15 minutes chatting with Claude first. Ask it to:
  - Explain something you're curious about
  - Generate a simple artifact (like a todo list)
  - Get comfortable with the interface

---

<a id="setting-up-workspace"></a>
## Setting Up Your Workspace

### Option 1: Claude.ai Artifacts (Recommended for First-Timers)

**Best for:**
- Single-page apps
- Dashboards and forms
- Simple calculators or tools
- Anything that fits on one screen

**Pros:**
- Instant preview—see your app as it's built
- No setup required
- Easy to share with others
- Perfect for demos

**Cons:**
- Limited to browser-based apps
- Can't save files or connect to databases
- Everything resets if you close the chat

**How to start:**
1. Go to claude.ai
2. Start a new conversation
3. Ask Claude to "create an artifact showing a simple form"
4. You'll see a preview panel appear on the right
5. That's where your app will appear!

### Option 2: Claude.ai Projects (For Multi-Session Work)

**Best for:**
- Multi-page applications
- Projects that take multiple days
- When you need to save progress
- Referencing multiple documents/files

**Pros:**
- Saves your work between sessions
- Can reference multiple files
- Better for complex projects
- Keeps context across conversations

**Cons:**
- Slight learning curve
- Need to understand basic file structure
- Requires organization

**How to start:**
1. Go to claude.ai
2. Click "Projects" in the sidebar
3. Create new project with a descriptive name
4. Add any relevant documents (user research, specs, etc.)
5. Start chatting within the project

### Which Should You Choose?

**Start with Artifacts if:**
- This is your first vibe coding project
- You're building something simple
- You want to show results fast
- Project will take 1-2 sessions max

**Use Projects if:**
- Building over multiple days
- Need to reference documents
- Want to save your progress
- Planning to iterate significantly

💡 **Pro Tip:** Start with Artifacts for your first project. You can always move to Projects later.

---

<a id="vibe-coding-mindset"></a>
## The Vibe Coding Mindset

Before you dive in, understand these key principles:

### 1. You're the Director, Not the Actor

**Think of it this way:**
- You're the movie director (making creative decisions)
- Claude is the crew (executing your vision)
- The prototype is the film (what users experience)

**Your job:**
- ✅ Define what success looks like
- ✅ Make product decisions
- ✅ Validate with users
- ✅ Guide the conversation
- ✅ Ensure quality

**NOT your job:**
- ❌ Write the code
- ❌ Understand technical implementation
- ❌ Debug syntax errors
- ❌ Optimize performance

### 2. Iteration is Expected

Your first prompt won't be perfect. That's normal!

**The Vibe Coding Cycle:**
```
    ┌─────────────────────────────────────┐
    │         1. DESCRIBE                 │
    │   Tell Claude what you want         │
    │   (Be specific and clear)           │
    └──────────────┬──────────────────────┘
                   │
                   ▼
    ┌─────────────────────────────────────┐
    │         2. ASSESS                   │
    │   Claude builds it instantly        │
    │   (Review what you see)             │
    └──────────────┬──────────────────────┘
                   │
                   ▼
    ┌─────────────────────────────────────┐
    │         3. TEST                     │
    │   Try using it yourself             │
    │   (Click, type, interact)           │
    └──────────────┬──────────────────────┘
                   │
                   ▼
    ┌─────────────────────────────────────┐
    │         4. REFINE                   │
    │   Give specific feedback            │
    │   ("Change X to Y because...")      │
    └──────────────┬──────────────────────┘
                   │
                   ▼
    ┌─────────────────────────────────────┐
    │         5. REPEAT                   │
    │   Keep cycling until it works       │
    │   (Typically 5-15 iterations)       │
    └──────────────┬──────────────────────┘
                   │
                   └──────> Back to DESCRIBE
```

**Example of one full cycle:**
- **Describe:** "Add a submit button to the form"
- **Assess:** Claude adds button, you see it in preview
- **Test:** You click it, notice it's too small on mobile
- **Refine:** "Make the button taller (48px) for easier mobile tapping"
- **Repeat:** Claude updates it, you test again

Most successful projects go through **5-15 iterations** on each feature.

### 3. Specificity Beats Cleverness

**Bad prompt (too vague):**
"Build a user dashboard"

**Good prompt (specific):**
"Create a dashboard showing:
- Total sales this month (big number at top)
- List of recent orders (last 10)
- Bar chart of sales by day
Use a clean, modern design with blue colors"

More details = better results.

### 4. Test Early, Test Often

Don't wait until "it's done" to test. Test after every major feature.

**Testing rhythm:**
- After first feature: Does core idea work?
- After 2-3 features: Does user flow make sense?
- After most features: Full usability test
- Before sharing: Polish and edge cases

### 5. Know When to Start Over

Sometimes it's faster to start fresh than to fix a messy project.

**Signs you should restart:**
- Same bug keeps appearing after 3+ fix attempts
- You don't understand what Claude built
- New features consistently break old features
- The conversation has 30+ exchanges

**How to restart well:**
1. Document what you learned
2. Write a clearer first prompt
3. Start a new chat/project
4. Build in smaller increments this time

### 6. It's Collaboration, Not Magic

Claude is powerful but not perfect. You need to:
- Review what it builds
- Ask "why did you do it this way?"
- Challenge approaches that seem overly complex
- Provide examples when your description isn't clear

Think: "Working with a capable but junior team member"

---

# PART 3: THE FRAMEWORK

# PHASE 1: THINK BEFORE YOU BUILD
**Time Investment: 30-60 minutes**  
**Why it matters: Every minute here saves 30 minutes in Phase 3**

<a id="step-1-define-problem"></a>
## Step 1: Define the Problem (15-20 min)

Before asking Claude to build anything, get crystal clear on what you're solving and why.

### The 6 Essential Questions

Answer these in writing (yes, actually write them down):

#### 1. What problem are you solving?

**Bad:** "We need better customer management"  
**Good:** "Sales reps forget to follow up with leads, causing us to lose deals"

Be specific. Use real examples:
- "It takes our team 2 hours to create the weekly report manually"
- "Customers can't track their order status, so they email us constantly"
- "We lose visibility when projects span multiple team members"

#### 2. Who is this for?

**Bad:** "Business users"  
**Good:** "Sales reps who are always on the road, use mobile primarily, and hate complex software"

Create a mini user profile:
- Role: [Specific job title]
- Context: [When/where they'll use this]
- Tech comfort: [Low/Medium/High]
- Pain points: [What frustrates them today]
- Success for them: [What makes their day better]

#### 3. What already exists? Why isn't it enough?

Research 2-3 existing tools:
- What do they do well?
- What do they do poorly?
- Why can't you just use them?
- What gaps will you fill?

💡 **Pro Tip:** Spend 15 minutes using a competitor's tool. Take screenshots. This gives Claude context about what to emulate (or avoid).

#### 4. How will you know it worked?

**Bad:** "Users like it"  
**Good:** "3 out of 5 test users can complete the core task in under 2 minutes without help"

Define success metrics:
- **Usage metric:** "5 team members use it daily"
- **Speed metric:** "Reduces task time from 30 min to 5 min"
- **Quality metric:** "Zero calculation errors in testing"
- **Feedback metric:** "Users rate it 7+ out of 10"

#### 5. What are you NOT solving?

This is crucial—scope creep kills projects.

**Example:**
- ✅ Building: Simple lead tracker
- ❌ Not building: Full CRM with email integration
- ✅ Building: Manual data entry
- ❌ Not building: Automated import from other systems

#### 6. Why solve this with software?

Could this be:
- A spreadsheet? (If yes, might be better!)
- A simple form tool? (Google Forms, Typeform?)
- A manual process? (Sometimes that's fine!)
- An existing tool you haven't discovered?

If software isn't clearly the best answer, pause and reconsider.

### Template: Problem Definition

```
PROBLEM STATEMENT:
[One paragraph describing the problem with specific examples]

TARGET USER:
Role: [Title/description]
Context: [When/where they use it]
Tech level: [Low/Medium/High]
Key frustrations: [What bothers them]
Success for them: [What gets better]

EXISTING SOLUTIONS:
Tool 1: [Name] - Good: [X] / Bad: [Y]
Tool 2: [Name] - Good: [X] / Bad: [Y]
Our advantage: [What we do differently]

SUCCESS CRITERIA:
- [Measurable outcome 1]
- [Measurable outcome 2]
- [Measurable outcome 3]

OUT OF SCOPE:
- [What we're not building]
- [What we're not building]

WHY SOFTWARE?
[Why this needs to be custom-built vs using existing tools]
```

### ✅ Checkpoint #1

Before moving forward, verify:
- [ ] You can explain the problem in 2 sentences to anyone
- [ ] You have a specific person in mind (not "everyone")
- [ ] You know how you'll measure success
- [ ] You've looked at 2-3 existing alternatives
- [ ] You can justify why this needs to be built

🎯 **Reality Check:** If you can't confidently check all boxes, spend more time in Step 1. This foundation determines everything.

---

<a id="step-2-pressure-test"></a>
## Step 2: Pressure-Test with AI (10-15 min)

Now use Claude to poke holes in your thinking BEFORE you start building.

### Why This Matters

You might be:
- Solving the wrong problem
- Missing simpler alternatives
- Overlooking technical constraints
- Building something nobody wants

Better to discover this now than after 8 hours of building!

### The Pressure-Test Prompt

Copy and customize this template:

```
I'm planning to build [type of tool/app].

CONTEXT:
Problem: [Your problem statement]
Target users: [Your user profile]
Success looks like: [Your criteria]

CHALLENGE THIS IDEA:
1. What am I assuming that might be wrong?
2. What are 3 alternative approaches I haven't considered?
3. What will be hardest to build or maintain?
4. What could make this fail with users?
5. What's the absolute simplest version that could work?
6. Is there an existing tool I should use instead?

Be skeptical and direct. I want to know if this is a bad idea before I invest time.
```

### What to Do with Claude's Response

**Look for these red flags:**
- 🚩 "This might be too complex for a prototype"
- 🚩 "Users typically need [feature you haven't considered]"
- 🚩 "Existing tool X already does most of this"
- 🚩 "The hardest part will be [thing you underestimated]"

**Common outcomes:**
1. **Claude confirms it's feasible** → Great! Proceed to Step 3
2. **Claude suggests simplifications** → Update your scope
3. **Claude identifies missing requirements** → Add to your plan
4. **Claude recommends alternatives** → Investigate before proceeding

### Real Example

**User's initial idea:**
"Build a tool for managing customer subscriptions with payment processing"

**Claude's pressure-test response:**
"Payment processing adds significant complexity and compliance requirements. Consider:
- Alternative 1: Build the subscription management UI only, integrate with existing payment system
- Alternative 2: Use Stripe's customer portal for subscriptions
- Alternative 3: Start with manual subscription tracking before automating payments
The hardest part will be handling payment failures, prorated billing, and PCI compliance."

**User's response:**
"You're right—payments are out of scope. I'll build just the subscription tracking interface and leave payment processing to our existing system."

### ✅ Checkpoint #2

After pressure-testing:
- [ ] You still believe this is worth building
- [ ] You've simplified or adjusted based on feedback
- [ ] You understand what will be challenging
- [ ] You have a backup plan if this approach doesn't work
- [ ] You're excited to start building (not overwhelmed)

---

<a id="step-3-choose-target"></a>
## Step 3: Choose Your Target (5-10 min)

Not all prototypes are created equal. Define what you're building toward.

### The 4 Target Types

#### POC (Proof of Concept)
**Goal:** Prove the core idea is technically possible  
**Audience:** Just you (maybe 1-2 teammates)  
**Quality bar:** Rough edges are fine, bugs are okay  
**Time investment:** 2-4 hours  
**Example:** "Can we extract data from PDFs automatically?"  
**What's next:** If it works → Enhance to MVP/Demo or hand to engineering

#### MVP (Minimum Viable Product)
**Goal:** Test with real users to validate need  
**Audience:** 5-10 alpha/beta users (real usage scenario)  
**Quality bar:** Core flow works reliably, handles real data  
**Time investment:** 1-3 days  
**Example:** "Let's see if sales reps actually use this lead tracker"  
**⚠️ Important:** MVPs used by real users often need engineering involvement for:
- Security review
- Data persistence that works at scale
- Production-grade error handling
- Integration with existing systems

**When to involve engineering:**
- If users will rely on it daily
- If it handles sensitive data
- If it needs to integrate with other systems
- If downtime would cause real problems

#### Demo (Stakeholder Presentation)
**Goal:** Get buy-in, funding, or approval  
**Audience:** Executives, investors, partners  
**Quality bar:** Polished UI, handles realistic data, no crashes  
**Time investment:** 2-4 days  
**Example:** "Show the CEO why we should build this feature"  
**What's next:** Usually handed to engineering for proper build

#### Internal Tool
**Goal:** Solve an operational problem for your team  
**Audience:** Specific team or department  
**Quality bar:** Works reliably with real data (UI can be simple)  
**Time investment:** 1-4 days  
**Example:** "Automate our weekly reporting process"  
**⚠️ Important:** Plan for maintenance! These tools will break and need updates.

### Evolution Path: Start Small, Scale Up

```
POC (2-4 hrs)
    ↓ Works? Like it?
    ├─> Enhance to MVP (add polish, real data handling)
    ├─> Enhance to DEMO (add visual polish, remove bugs)
    └─> Enhance to INTERNAL TOOL (add error handling, documentation)
```

**You don't need to choose the final target immediately.** Many successful projects:
1. Start as POC to prove feasibility
2. Show promise, so enhance to Demo for stakeholders
3. Get buy-in, hand to engineering for production MVP

Or:
1. Start as POC for an internal problem
2. Works well, enhance to Internal Tool
3. Team loves it, engineering makes it production-grade

### Decision Tree: Choose Your Target

```
START: What do you need to accomplish?
│
├─> "I want to prove this is technically possible"
│   └─> POC (Proof of Concept)
│       Time: 2-4 hours
│       Quality: Rough, bugs okay
│       Audience: Just you + maybe 1-2 teammates
│
├─> "I need to test if users actually want this"
│   └─> MVP (Minimum Viable Product)
│       Time: 1-3 days
│       Quality: Core works reliably
│       Audience: 5-10 real users (alpha/beta)
│       ⚠️ May need engineering for production use
│
├─> "I need to get buy-in from stakeholders/executives"
│   └─> DEMO (Stakeholder Presentation)
│       Time: 2-4 days
│       Quality: Polished, no crashes
│       Audience: Executives, investors, partners
│
└─> "I need to solve a problem my team has right now"
    └─> INTERNAL TOOL
        Time: 1-4 days
        Quality: Works with real data
        Audience: Your team or department
        ⚠️ Plan for ongoing maintenance
```

**Quick Questions to Decide:**

| If you answer... | Choose... |
|------------------|-----------|
| "Will anyone else see this?" → No | **POC** |
| "Do I need real user feedback?" → Yes | **MVP** |
| "Am I presenting to leadership?" → Yes | **DEMO** |
| "Will my team use this daily?" → Yes | **INTERNAL TOOL** |

💡 **Pro Tip:** Start with POC, then evolve it! Build a quick proof of concept first. If it works and you like it, you can enhance the same prototype into an MVP, Demo, or Internal Tool by adding polish and features.

### How This Affects Your Approach

| Aspect | POC | MVP | Demo | Internal Tool |
|--------|-----|-----|------|---------------|
| **UI Polish** | Skip it | Important | Very important | Nice-to-have |
| **Error Handling** | Happy path only | Comprehensive | Handle gracefully | Comprehensive |
| **Mobile Support** | If needed for test | Usually yes | Usually yes | Depends on use |
| **Documentation** | None | Essential for users | User-facing only | Essential + technical |
| **Engineering Involvement** | No | Likely for production | For next phase | For scale/reliability |
| **Phase 2 Planning** | Skip to Phase 3 | Do Steps 4-5 | Do Steps 4-6 | Do Steps 4-6 |

### Template: Target Definition

```
TARGET TYPE: [POC / MVP / Demo / Internal Tool]

PRIMARY GOAL:
[What you're trying to achieve]

AUDIENCE:
[Who will use/see this]

QUALITY BAR:
Must work: [Essential features]
Should work: [Important but not critical]
Nice to have: [Polish/extras]

SUCCESS METRIC:
[How you'll know this achieved its goal]

WHAT HAPPENS NEXT:
[Throw away / Hand to eng / Keep using / Iterate on feedback]
```

### ✅ Checkpoint #3

Before proceeding:
- [ ] You've chosen one target type (not "maybe MVP, maybe Demo")
- [ ] You understand what quality bar is needed
- [ ] You know who will evaluate this
- [ ] You're clear on what happens after this prototype

🎯 **Reality Check:** Most people should start with POC or MVP. Demo requires significantly more polish. Be honest about your timeline and goals.

---

# PHASE 2: PLAN YOUR BUILD
**Time Investment: 30-60 minutes**  
**Skip if building POC. Optional for MVP. Required for Demo/Internal Tool.**

<a id="step-4-describe-build"></a>
## Step 4: Describe What You Want (20-30 min)

This step translates your problem into a clear description Claude can work with.

### The 5-Part Description

#### Part 1: One-Sentence Summary

Force yourself to describe it in ONE sentence:

**Examples:**
- "A form where sales reps log customer calls and see their call history"
- "A dashboard showing our team's project progress in real-time"
- "A calculator that estimates project costs based on team size and duration"

**Test:** Can someone who knows nothing about your company understand what this does?

#### Part 2: User Flow

Describe the step-by-step journey:

```
USER FLOW:
1. [User starts at...]
2. [User does...]
3. [System shows/does...]
4. [User completes when...]
```

**Example: Lead Tracker**
```
USER FLOW:
1. Sales rep opens the app on their phone
2. Taps "Add Lead" button
3. Fills in: Company name, Contact person, Phone, Interest level
4. Taps "Save"
5. Sees confirmation message
6. Can view list of all their leads sorted by date
```

**Keep it to 4-8 steps max.** If it's longer, you might be building too much.

#### Part 3: Success Outcome

What does success look like for the user?

**Examples:**
- "Sales rep can log a call in under 30 seconds"
- "Manager can see project status without asking anyone"
- "User gets accurate cost estimate without using spreadsheet"

#### Part 4: Constraints

Technical or design requirements:

```
CONSTRAINTS:
- Device: [Mobile-first / Desktop / Both]
- Data: [Where does it come from? Where does it go?]
- Design: [Any style requirements?]
- Performance: [Speed needs?]
```

**Example:**
```
CONSTRAINTS:
- Mobile-first (sales reps mostly on phones)
- Data stays in browser (no backend needed)
- Simple, fast interface (no unnecessary clicks)
- Works without internet for data entry (syncs later)
```

#### Part 5: Reference Examples

Show Claude what you like:

"Make it look similar to [Trello's card interface]"
"Use a layout like [Google Calendar's day view]"
"Style should feel like [Stripe's dashboard] - clean and modern"

💡 **Pro Tip:** Take screenshots of UIs you like and describe what specifically appeals to you.

### Template: Build Description

```
ONE-SENTENCE SUMMARY:
[What this tool does in one sentence]

USER FLOW:
1. [Step 1]
2. [Step 2]
3. [Step 3]
4. [Step 4]
5. [Result/completion]

SUCCESS OUTCOME:
[What success looks like for user]

CONSTRAINTS:
Device: [Mobile/Desktop/Both]
Data: [Where from, where to]
Design: [Style requirements]
Performance: [Speed needs]

REFERENCE EXAMPLES:
[What this should look/feel like]

NOT INCLUDED (YET):
[Features you're deliberately leaving out]
```

### Real Example: Customer Feedback Tool

```
ONE-SENTENCE SUMMARY:
A simple form where customers can submit product feedback and see the status of their previous submissions.

USER FLOW:
1. Customer lands on feedback page
2. Sees simple form: Name (optional), Email, Feedback (text area), Category (dropdown)
3. Clicks "Submit Feedback"
4. Sees confirmation: "Thanks! We'll review your feedback."
5. Can optionally view "My Previous Feedback" showing their submission history
6. Each past submission shows: Date, Category, Status (New/Reviewing/Implemented)

SUCCESS OUTCOME:
Customer can submit feedback in under 60 seconds. They feel heard because they can track what happens to their feedback.

CONSTRAINTS:
Device: Both mobile and desktop (mobile-first design)
Data: Store submissions (needs simple database or backend)
Design: Clean, friendly, not corporate-feeling
Performance: Form submit under 2 seconds

REFERENCE EXAMPLES:
- Form design like Typeform (one question at a time feel, but all on one page)
- Status tracking like package tracking (clear progress states)
- Overall vibe like Notion (modern, clean, not intimidating)

NOT INCLUDED (YET):
- User accounts/login
- Admin panel to respond to feedback
- Email notifications
- Voting on others' feedback
- File attachments
```

### ✅ Checkpoint #4

Review your description:
- [ ] One sentence summary is clear
- [ ] User flow has 4-8 specific steps
- [ ] Success outcome is measurable
- [ ] Constraints are realistic
- [ ] You have reference examples
- [ ] You've listed what's NOT included

🎯 **Reality Check:** If your user flow has more than 10 steps, you're trying to do too much in one go. Here's what to do:

**Option 1: Simplify the flow**
- Remove non-essential steps
- Combine steps where possible
- Focus on the absolute core journey

**Option 2: Break into phases (not separate projects)**
- **Phase 1:** Build steps 1-4 (core value)
- Test and validate
- **Phase 2:** Add steps 5-7 (important additions)
- Test again
- **Phase 3:** Add remaining steps (nice-to-haves)

**Example: Complex Onboarding Flow**

❌ **Too much at once (12 steps):**
1. User signs up
2. Email verification
3. Company profile setup
4. Team invitation
5. Integration selection
6. API key setup
7. Data import
8. Workspace customization
9. Role assignment
10. Notification preferences
11. Tutorial walkthrough
12. First project creation

✅ **Phase 1 - Core Flow (4 steps):**
1. User signs up
2. Email verification  
3. Simple company profile (just name)
4. Create first project

✅ **Phase 2 - Team Features (3 steps added):**
5. Invite team members
6. Assign roles
7. Set up workspace

✅ **Phase 3 - Advanced Setup (remaining steps):**
8. Connect integrations
9. Import existing data
10. Customize preferences

**Why this matters:** Building everything at once leads to:
- Context overload for Claude
- Harder to debug when things break
- Difficult to test properly
- Higher chance of giving up

**The right approach:** Build Phase 1, test it, make sure it works, THEN build Phase 2. Each phase is still part of the same app, you're just building it incrementally.

---

<a id="step-5-break-down-features"></a>
## Step 5: Break Down Features (15-20 min)

Now break your idea into bite-sized pieces you'll build one at a time.

### The MoSCoW Method

Categorize every feature:

**MUST HAVE** - Without this, it doesn't work
**SHOULD HAVE** - Important but not critical
**COULD HAVE** - Nice to have if time permits
**WON'T HAVE** - Explicitly out of scope (for now)

### Feature Breakdown Template

```
MUST HAVE (Core Value):
- [ ] Feature 1 [Why it's critical]
- [ ] Feature 2 [Why it's critical]

SHOULD HAVE (Important):
- [ ] Feature 3 [Why it matters]
- [ ] Feature 4 [Why it matters]

COULD HAVE (Nice-to-have):
- [ ] Feature 5 [Why it's nice but optional]

WON'T HAVE (Out of scope):
- Feature 6 [Why not now]
- Feature 7 [Why not now]
```

### The Build Order Strategy

Build in this sequence:

**1. Happy Path First** (Build order #1-3)
The simplest version of the core feature

**2. Common User Flows** (Build order #4-6)
Secondary but frequent use cases

**3. Error Handling** (Build order #7-9)
What happens when things go wrong

**4. Polish & Nice-to-Haves** (Build order #10+)
UI improvements, convenience features

### Real Example: Feedback Tool

```
MUST HAVE (Core Value):
- [ ] #1 Feedback form (Name, Email, Message, Category dropdown)
- [ ] #2 Submit button that shows success message
- [ ] #3 Form validation (email format, required fields)

SHOULD HAVE (Important):
- [ ] #4 View past submissions (list showing date, category, status)
- [ ] #5 Mobile-responsive design
- [ ] #6 Character counter on message field

COULD HAVE (Nice-to-have):
- [ ] #7 Filter past submissions by category
- [ ] #8 Search through past feedback
- [ ] #9 Export feedback to CSV

WON'T HAVE (Out of scope):
- User authentication (we'll use email lookup only)
- Admin dashboard (separate project)
- File uploads (keep it simple)
- Real-time notifications (email is enough)
```

### Feature Assessment Questions

For each feature, ask:

**Is it critical for core value?**
- Yes → MUST HAVE
- Improves experience → SHOULD HAVE
- Just nice → COULD HAVE

**Can AI build it reliably?**
- Simple UI/logic → Yes
- Complex integrations → Maybe not (flag for engineering)
- Novel algorithms → Probably not

**Can it be tested independently?**
- Yes → Build it whenever
- No → Note what it depends on

### ✅ Checkpoint #5

Review your features:
- [ ] You have 3-5 "MUST HAVE" features (not 20)
- [ ] Build order is numbered and logical
- [ ] Each feature is testable on its own (or you noted dependencies)
- [ ] You've been ruthless about "WON'T HAVE"
- [ ] Features are specific enough to build ("add form" not "improve UX")

⚠️ **Red Flag:** If you have more than 7 MUST HAVE features, your scope is too large. Simplify or break into multiple phases.

---

<a id="step-6-first-prompt"></a>
## Step 6: Prepare Your First Prompt (10 min)

Your opening message to Claude sets the tone for the entire project. Make it count.

### The First Prompt Template

```
I want to build [one-sentence summary from Step 4].

CONTEXT:
Users: [Who and their key traits]
Problem it solves: [From Step 1]
Success looks like: [From Step 4]

TECHNICAL CONSTRAINTS:
- [Device requirements]
- [Data handling]
- [Performance needs]

LET'S START WITH:
[Feature #1 from your build order]

Specifically, I want:
- [Specific detail about feature]
- [Specific detail about feature]
- [Specific detail about feature]

Design should be: [Clean/modern/minimal/etc.]
Use: [Color preferences if any]

Please build this first feature and show me what it looks like. Ask clarifying questions if anything is unclear.
```

### Real Example: Feedback Tool First Prompt

```
I want to build a simple customer feedback form where people can submit product feedback and see their past submissions.

CONTEXT:
Users: Customers (non-technical, using mobile and desktop)
Problem it solves: Currently feedback goes to scattered emails and gets lost. We want one place to collect and track all feedback.
Success looks like: Customer can submit feedback in under 60 seconds and see the status of past submissions.

TECHNICAL CONSTRAINTS:
- Mobile-first but works on desktop
- Need to store submissions (suggest simple approach)
- Should load fast (under 2 seconds)

LET'S START WITH:
Build the feedback submission form.

Specifically, I want:
- Fields: Name (optional), Email (required), Feedback message (text area), Category (dropdown: Bug Report, Feature Request, General Feedback)
- Submit button that shows a success message after submission
- Form validation (proper email format, message can't be empty)
- Clean, friendly design (not corporate-looking)

Design should be: Modern and welcoming, similar to Typeform's aesthetic
Use: Soft blue accent color (#4A90E2)

Please build this first feature and show me what it looks like. Ask clarifying questions if anything is unclear.
```

### What Makes a Good First Prompt?

**✅ Good first prompts:**
- Focus on ONE feature
- Include specific requirements
- Provide context about users
- Mention design preferences
- Invite questions

**❌ Bad first prompts:**
- "Build a feedback tool"
- List all features at once
- No context about users
- No design guidance
- Assume Claude knows what you want

### Special Considerations by Target Type

**For POC:**
- Emphasize "quick and rough is fine"
- Focus purely on feasibility
- Skip design preferences

**For MVP:**
- Mention "clean but simple design"
- Include basic error handling
- Specify mobile/desktop needs

**For Demo:**
- Emphasize "polished and professional"
- Mention specific design aesthetic
- Include all edge cases

### ✅ Checkpoint #6

Review your first prompt:
- [ ] Focuses on just the first feature
- [ ] Includes specific requirements (not vague)
- [ ] Provides user context
- [ ] States design preferences
- [ ] Invites Claude to ask questions
- [ ] Is under 200 words (if longer, you're over-specifying)

🎯 **Reality Check:** You should be able to read this prompt aloud in under 60 seconds. If it takes longer, you're including too much.

---

# PHASE 3: BUILD WITH CLAUDE
**Time Investment: 2-8 hours (spread across multiple sessions is fine)**  
**This is where the magic happens—and where most mistakes occur**

<a id="step-7-start-conversation"></a>
## Step 7: Start the Conversation (15-30 min)

Now you'll actually talk to Claude and see your first feature come to life.

### Starting the Build

1. **Open Claude.ai**
   - Use Artifacts (for single-session builds)
   - Or start a Project (for multi-day work)

2. **Paste your first prompt** (from Step 6)

3. **Wait for Claude's response**
   - It might ask clarifying questions → Answer them
   - It might suggest alternatives → Consider them
   - It will build the first version → Review it

### What to Expect in Claude's First Response

Claude will typically:
1. Confirm understanding of what you want
2. Possibly ask 1-2 clarifying questions
3. Generate the code
4. Show a preview (in Artifacts) or explain what it built

### Responding to Claude's Questions

**If Claude asks clarifying questions:**

❌ **Don't:** "Whatever you think is best"  
✅ **Do:** Give specific answers or examples

**Example exchange:**
```
Claude: "For the category dropdown, should users be able to select multiple categories or just one?"

Bad response: "Whatever makes sense"

Good response: "Just one category per submission. If someone needs multiple categories, they can submit separate feedback."
```

### Reviewing the First Version

When Claude shows you what it built, check:

**1. Does it look right?**
- Layout makes sense?
- Readable on mobile (if needed)?
- Colors/styling acceptable?

**2. Does it do what you asked?**
- All fields present?
- Submit button works?
- Validation happening?

**3. What's confusing or wrong?**
- Anything surprising?
- Anything missing?
- Anything broken?

### The First Iteration

It's normal for the first version to need tweaks. Common issues:

**Visual Issues:**
- "The form is too wide on mobile"
- "The text is too small"
- "The colors don't match our brand"

**Functional Issues:**
- "The submit button doesn't show any feedback"
- "Email validation isn't working"
- "Dropdown options are in the wrong order"

**Missing Pieces:**
- "Can we add a character limit to the message?"
- "The success message disappears too quickly"
- "Need a 'clear form' button"

### How to Give Feedback to Claude

**Use this pattern:**
```
Looking at [the specific part], I need to change [specific thing].

Currently it: [What it does now]
I want it to: [What it should do]

[Optional: Why this matters]
```

**Real examples:**

```
Looking at the submit button, I need to change its behavior.

Currently it: Just shows "Submitted" briefly
I want it to: Show a green checkmark with "Thanks! Your feedback has been submitted" for 3 seconds, then clear the form

This matters because: Users need clear confirmation their feedback was received.
```

```
Looking at the mobile layout, the form is too cramped.

Currently it: Everything is squished and hard to tap
I want it to: Increase spacing between fields, make buttons larger (at least 44px tall), add more padding

This matters because: Sales reps use this on phones between meetings.
```

### ✅ Checkpoint #7

After building the first feature:
- [ ] The feature works on the happy path
- [ ] You understand what Claude built (even if not the code details)
- [ ] It looks acceptable (doesn't need to be perfect)
- [ ] You can describe what it does to someone else
- [ ] You're ready to add the next feature

💡 **Pro Tip:** Take a screenshot after each working feature. This helps you track progress and shows stakeholders what you built.

---

<a id="step-8-build-test-iterate"></a>
## Step 8: The Build-Test-Iterate Loop (2-6 hours)

This is the core of vibe coding. You'll repeat this cycle for each feature.

### The Loop

```
FOR EACH FEATURE:
1. REQUEST the feature (be specific)
2. REVIEW what Claude built
3. TEST it thoroughly
4. ITERATE with feedback
5. VERIFY it works
6. MOVE TO next feature

AFTER EVERY 3-5 FEATURES:
→ Do a Quality Checkpoint (Step 9)
```

### 1. REQUEST: How to Ask for Each Feature

Use this template:

```
Now let's add [feature name from your list].

What it should do:
- [Specific behavior 1]
- [Specific behavior 2]
- [Specific behavior 3]

Success looks like:
[Concrete example of it working]

Keep the existing [previous features] working.
```

**Real example:**

```
Now let's add the "View Past Feedback" feature.

What it should do:
- Show a "My Feedback" button below the submission form
- When clicked, display a list of all submissions from this user (match by email)
- Each item shows: Date submitted, Category, Message preview (first 50 characters), Status badge
- Status badges: "New" (blue), "Reviewing" (yellow), "Implemented" (green)
- List sorted by date (most recent first)
- If no past feedback, show friendly message: "You haven't submitted any feedback yet"

Success looks like:
User enters their email, clicks "My Feedback", and sees their submission history in a clean list format.

Keep the existing submission form working.
```

### 2. REVIEW: First Look at What Claude Built

Don't just accept it. Actually look at it:

**Visual check:**
- Does it look how you imagined?
- Is anything obviously broken?
- Does it fit with existing features?

**Functional check:**
- Did Claude add what you asked for?
- Did Claude add things you DIDN'T ask for? (Sometimes good, sometimes not)
- Are there obvious issues?

### 3. TEST: Actually Use It

Don't just look—interact with it!

**Basic testing:**
- [ ] Click every button
- [ ] Fill out every form field
- [ ] Try the happy path (everything works)
- [ ] Try leaving fields empty
- [ ] Try weird inputs (special characters, very long text)
- [ ] Test on mobile (if relevant)
- [ ] Test on desktop (if relevant)

**Specific tests by feature type:**

**Forms:**
- Submit with all fields filled
- Submit with required fields empty
- Submit with invalid data (bad email, etc.)
- Submit twice quickly
- Submit with very long text

**Lists/Tables:**
- View with no data
- View with 1 item
- View with many items (10+)
- Try any sorting/filtering
- Try any interactive elements

**Calculations:**
- Try with normal numbers
- Try with zero
- Try with negative numbers
- Try with very large numbers
- Try with text instead of numbers

### 4. ITERATE: Give Specific Feedback

When something needs fixing, be specific:

**Pattern for bug fixes:**
```
Found an issue with [feature].

What I did: [Steps to reproduce]
What happened: [Actual behavior]
What should happen: [Expected behavior]

Can you fix this?
```

**Pattern for improvements:**
```
The [feature] works, but I want to improve [aspect].

Currently: [How it is now]
Change to: [How it should be]
Reason: [Why this matters]
```

**Real examples:**

```
Found an issue with the feedback list.

What I did: Clicked "My Feedback" without entering an email
What happened: Shows error "Cannot read property 'filter' of undefined"
What should happen: Should show a message like "Please enter your email to view your feedback"

Can you fix this?
```

```
The feedback list works, but I want to improve readability.

Currently: All submissions are in one long list with no visual separation
Change to: Add a subtle border between items, increase spacing, and make the date smaller/lighter
Reason: Right now it's hard to scan through multiple items quickly
```

### 5. VERIFY: Confirm the Fix

After Claude makes changes:
- [ ] Test the original issue again
- [ ] Make sure the fix didn't break anything else
- [ ] Verify it works on both mobile and desktop (if needed)

### 6. MOVE TO NEXT: Know When You're Done with a Feature

A feature is "done" when:
- ✅ Happy path works smoothly
- ✅ Common errors are handled
- ✅ It looks acceptable (not perfect, just acceptable)
- ✅ You can demo it to someone
- ✅ It doesn't break other features

**Don't aim for perfect.** You're building a prototype, not a production app.

### How Long Should Each Feature Take?

**Rough guidelines:**
- Simple form field: 5-10 minutes
- Basic list/table: 15-30 minutes
- Interactive component: 30-60 minutes
- Feature with logic: 45-90 minutes

⚠️ **Red Flag:** If a single feature takes more than 2 hours of back-and-forth:
- The feature is too complex (break it down)
- You're not being specific enough (clarify your requirements)
- Claude is confused (start a new chat with clearer context)
- This might need engineering (consider whether it's feasible)

### Managing Multiple Features

**Track your progress systematically:**

#### Simple Tracking Template

```
PROJECT: [Your App Name]
STARTED: [Date]
TARGET: [POC/MVP/Demo/Internal Tool]

═══════════════════════════════════════════════════════

FEATURE TRACKER

Feature #1: [Feature Name]
Status: ✅ DONE
Built: [Date]
Tested: ✅ Works on happy path | ✅ Tested on mobile | ✅ Tested on desktop
Notes: [Any known issues or things to remember]

Feature #2: [Feature Name]  
Status: ✅ DONE
Built: [Date]
Tested: ✅ Works on happy path | ✅ Tested on mobile | ⚠️ Minor issue on desktop (acceptable)
Notes: [Description of minor issue and why it's acceptable]

Feature #3: [Feature Name]
Status: 🔄 IN PROGRESS
Built: [Date started]
Tested: ⏳ Waiting to complete
Notes: [What you're currently working on]

Feature #4: [Feature Name]
Status: ⏳ PLANNED
Built: —
Tested: —
Notes: [What needs to happen first before building this]

═══════════════════════════════════════════════════════

KNOWN ISSUES:
• [Issue 1]: [Impact - Critical/Minor/Cosmetic]
• [Issue 2]: [Impact - Critical/Minor/Cosmetic]

DEPENDENCIES:
• Feature #5 requires Feature #3 to be complete
• Feature #7 needs real data before testing

NEXT SESSION GOALS:
□ Finish Feature #3
□ Build Feature #4
□ Test Feature #2 on desktop and fix issue
□ Do quality checkpoint after Feature #5
```

#### Real Example

```
PROJECT: Customer Feedback Tool
STARTED: Oct 20, 2024
TARGET: MVP

═══════════════════════════════════════════════════════

FEATURE TRACKER

Feature #1: Feedback submission form
Status: ✅ DONE
Built: Oct 20, 2pm
Tested: ✅ Happy path | ✅ Mobile | ✅ Desktop
Notes: All validation working correctly

Feature #2: Form validation & error messages
Status: ✅ DONE
Built: Oct 20, 3pm
Tested: ✅ Happy path | ✅ Edge cases | ✅ Mobile
Notes: Shows clear errors for empty fields and bad email

Feature #3: Success message after submission
Status: ✅ DONE
Built: Oct 20, 3:30pm
Tested: ✅ Happy path | ✅ Mobile | ✅ Desktop
Notes: Displays for 3 seconds then clears form

Feature #4: View past feedback by email
Status: 🔄 IN PROGRESS
Built: Oct 20, 4pm (partial)
Tested: ⏳ Basic version works, needs refinement
Notes: Working on styling and empty states

Feature #5: Status badges (New/Reviewing/Implemented)
Status: ⏳ PLANNED
Built: —
Tested: —
Notes: Needs Feature #4 complete first

Feature #6: Mobile responsive design polish
Status: ⏳ PLANNED
Built: —
Tested: —
Notes: Will do after all features work functionally

═══════════════════════════════════════════════════════

KNOWN ISSUES:
• Past feedback list: No empty state message - Minor (fixing in #4)
• Submit button: Could be larger on mobile - Cosmetic (will fix in #6)

DEPENDENCIES:
• Feature #5 requires Feature #4 complete
• Feature #6 (mobile polish) should be done after all features exist

NEXT SESSION GOALS:
□ Complete Feature #4 (finish styling)
□ Build Feature #5 (status badges)
□ Do quality checkpoint after Feature #5
□ Start mobile polish if time permits
```

#### Checkpoint Tracking

After every 3-5 features, add a checkpoint entry:

```
═══════════════════════════════════════════════════════
CHECKPOINT #1 - Oct 20, 5pm
Features complete: #1, #2, #3, #4, #5

✅ WHAT'S WORKING WELL:
- All core submission flow works
- Mobile experience is decent
- No critical bugs

⚠️ NEEDS ATTENTION:
- Past feedback list styling needs work
- Status badges color scheme unclear

🔄 NEXT FOCUS:
- Polish the past feedback view
- Add mobile responsive improvements
- Test with first user
═══════════════════════════════════════════════════════
```

**Keep this tracking document open** while you work. Update it after every feature completion. This helps you:
- Know exactly where you are
- Remember what works and what doesn't
- Avoid rebuilding things that already work
- Communicate progress to stakeholders

### When to Take a Break

Building is intense. Take breaks:
- After every 2 hours of active building
- After completing 3-5 features
- When you start feeling frustrated
- Before major features that require focus

Fresh eyes spot issues faster.

### ✅ Checkpoint #8

After each feature:
- [ ] Feature works on the happy path
- [ ] Tested with several scenarios
- [ ] Handles errors gracefully (doesn't crash)
- [ ] Looks acceptable
- [ ] Doesn't break previous features
- [ ] You understand what it does

🎯 **Reality Check:** If you're 4+ hours into building and still on your first feature, something's wrong. Simplify the feature or restart with clearer requirements.

---

<a id="step-9-quality-checkpoints"></a>
## Step 9: Quality Checkpoints (30-45 min per checkpoint)

Every 3-5 features, pause and do a quality check. This prevents technical debt from piling up.

### When to Do a Quality Checkpoint

**Do a checkpoint after:**
- Every 3-5 features added
- Before adding a complex feature
- When you notice features starting to break each other
- Before user testing
- At the end of each session (if multi-day project)

### The Quality Checkpoint Process

#### 1. Full Walkthrough Test

Pretend you're a user seeing this for the first time:
- [ ] Can you complete the main task without errors?
- [ ] Is the user flow intuitive?
- [ ] Are there any confusing elements?
- [ ] Does everything load quickly?
- [ ] Are there any visual bugs?

#### 2. Mobile & Desktop Check

If your app needs to work on both:
- [ ] Test every feature on mobile viewport (resize browser)
- [ ] Test every feature on desktop viewport
- [ ] Check that nothing is cut off or unclickable
- [ ] Verify text is readable on small screens
- [ ] Test touch interactions (if mobile)

#### 3. Edge Cases Review

Test unusual scenarios:
- [ ] What happens with no data?
- [ ] What happens with lots of data (100+ items)?
- [ ] What happens with very long text inputs?
- [ ] What happens if user clicks rapidly?
- [ ] What happens with special characters?

#### 4. Ask Claude for a Code Walkthrough

Even if you're not technical, this helps:

**Prompt:**
```
Please review what we've built so far and explain:
1. What are the main components/parts?
2. Are there any potential issues or areas that might cause problems?
3. Is the code organized well or is it getting messy?
4. Are there any security concerns I should know about?
5. What would be hardest to change later?
```

Claude will give you a high-level overview. Look for:
- 🚩 "The code is getting repetitive" → Might need refactoring
- 🚩 "This approach won't scale well" → Consider alternatives
- 🚩 "There's a security issue with [X]" → Fix it now
- ✅ "The architecture is clean and maintainable" → Keep going!

#### 5. Performance Check

For web apps, check:
- [ ] Page loads in under 3 seconds
- [ ] Forms submit in under 2 seconds
- [ ] Interactions feel instant (not laggy)
- [ ] No frozen screens or endless loading

**If things are slow:**
```
The app is loading slowly, especially [specific action].
Can you optimize this for better performance?
```

#### 6. Security Review

Ask Claude about security:

```
Review the current implementation for security issues:
- Are there any ways a user could access data they shouldn't?
- Is user input being validated properly?
- Are there any exposed API keys or sensitive data?
- What are the biggest security risks right now?
```

**Common issues in prototypes:**
- Exposed API keys (if you added any)
- No input validation
- No authentication (if needed)
- Data stored insecurely

### Red Flags During Checkpoints

Stop and fix if you notice:

🚩 **Context is getting messy**
- Chat has 30+ exchanges
- Claude keeps forgetting earlier decisions
- New features breaking old features consistently

**Solution:** Start fresh chat with full context:
```
I'm continuing work on [project]. Here's what we've built so far:
[List of completed features]

Current issues: [Any problems]

Let's continue by [next feature].
```

🚩 **You don't understand what Claude built**
- Can't explain it to someone else
- Don't know where to look when something breaks
- Afraid to ask for changes

**Solution:**
```
I need you to explain the current implementation at a high level.
What are the main parts and how do they work together?
Use simple language (I'm not a developer).
```

🚩 **Same issues keep appearing**
- Same bug fixed 3+ times
- Similar problems across features
- Fundamental architectural issue

**Solution:**
```
We keep running into [specific issue]. 
This suggests a fundamental problem.

Can you suggest a better approach that prevents this issue?
I'm willing to rebuild parts if needed.
```

### Refactoring When Needed

If the checkpoint reveals serious issues, you can ask Claude to refactor:

```
The code is getting messy. Let's clean it up before adding more features.

Specifically:
- [Issue 1 from checkpoint]
- [Issue 2 from checkpoint]
- [Issue 3 from checkpoint]

Please refactor the code to address these issues while keeping all existing functionality working.

After refactoring, let me test everything to make sure nothing broke.
```

### Documentation Checkpoint

Every checkpoint, update your notes:
```
COMPLETED FEATURES:
✅ [Feature 1] - Works well
✅ [Feature 2] - Works well
✅ [Feature 3] - Has minor issue: [describe], acceptable for now

KNOWN ISSUES:
- [Issue 1]: [Impact and whether it matters]
- [Issue 2]: [Impact and whether it matters]

NEXT UP:
- [Next feature to build]
- [Any dependencies or concerns]
```

### ✅ Checkpoint #9

After each quality checkpoint:
- [ ] All features tested end-to-end
- [ ] Tested on both mobile and desktop (if needed)
- [ ] Edge cases identified and handled (or documented)
- [ ] Got code walkthrough from Claude
- [ ] No critical security issues
- [ ] Performance is acceptable
- [ ] You understand what's been built
- [ ] Known issues are documented

🎯 **Reality Check:** If quality checkpoints reveal more than 3 serious issues, consider whether you need to restart with a cleaner approach.

---

# PHASE 4: VALIDATE
**Time Investment: 2-4 hours**  
**This is where you find out if your prototype actually solves the problem**

<a id="step-10-test-users"></a>
## Step 10: Test with Real Users (1-2 hours)

Now get your prototype in front of real users. This is non-negotiable.

### Before User Testing

**Preparation checklist:**
- [ ] All "Must Have" features are working
- [ ] You've tested it yourself thoroughly
- [ ] You can load/share the prototype easily
- [ ] You have 3-5 users lined up
- [ ] You've prepared test scenarios
- [ ] You have a way to take notes

### Who Should Test?

**Ideal test users:**
- Match your target user profile
- Unfamiliar with your project
- Will give honest feedback
- Available for 15-30 minutes

**How many users?**
- POC: 1-2 users (just you and maybe one other)
- MVP: 3-5 users minimum
- Demo: 2-3 users before the actual presentation
- Internal Tool: 3-5 team members who will actually use it

### How to Share Your Prototype

**If using Claude Artifacts:**
1. Get the artifact URL (click share icon)
2. Send link to user
3. Note: They'll need Claude access to view
4. Alternative: Screen share during a call

**If using Claude Projects:**
1. Export the code
2. Deploy to simple hosting (Replit, Vercel free tier)
3. Share the live URL

**If not deployed:**
1. Schedule a screen-sharing call
2. You control the prototype while they guide you
3. More manual but works fine for testing

### The User Testing Script

Use this structure:

```
[INTRODUCTION - 2 minutes]
"Hi! Thanks for helping me test this. I built a prototype and want to see if it makes sense. I'm testing the tool, not you, so there are no wrong answers. Please think out loud as you use it."

[CONTEXT - 1 minute]
"This tool is for [brief context about what it does]."

[TASK - 10-15 minutes]
"I'd like you to [realistic task that matches your user flow]. Take your time, and let me know if anything is confusing. Don't feel like you need to be polite about issues—honest feedback helps me improve it."

[FOLLOW-UP - 5 minutes]
Ask the follow-up questions below.
```

### What to Observe (Don't Interrupt!)

**Watch for:**
- Where do they pause or hesitate?
- Do they re-read instructions multiple times?
- Do they try clicking things that aren't clickable?
- Do they accomplish the task successfully?
- How long does it take them?
- What do they say out loud?

**Don't:**
- ❌ Help them or give hints
- ❌ Explain how it works
- ❌ Defend your design choices
- ❌ Interrupt their process

**Do:**
- ✅ Take detailed notes
- ✅ Ask "what are you thinking?" if they're silent
- ✅ Let them struggle (that's the point!)
- ✅ Bite your tongue when they misunderstand

### Follow-Up Questions

After they complete (or fail to complete) the task:

**Understanding:**
1. "What do you think this tool does?"
2. "Who do you think it's for?"

**Experience:**
3. "On a scale of 1-10, how easy was that to use?"
4. "What was most confusing?"
5. "What worked well?"

**Value:**
6. "Would you actually use this?"
7. "What's missing that you expected to see?"
8. "If you could change one thing, what would it be?"

**Comparison:**
9. "How does this compare to [existing tool/process]?"
10. "What would make you choose this over [alternative]?"

### Note-Taking Template

For each user, capture:

```
USER: [Name/Role]
DATE: [When you tested]

TASK COMPLETION:
✅ or ❌ Did they complete the main task?
Time taken: [X minutes]

OBSERVATIONS:
[Specific moments where they struggled]
[Things they said out loud]
[Unexpected behaviors]

DIRECT QUOTES:
"[Memorable thing they said]"
"[Another quote]"

FEEDBACK:
What worked: [Positive points]
What didn't work: [Issues]
Suggestions: [Their ideas]

SUCCESS METRIC:
[Your metric from Step 1]: ✅ or ❌ Met or not?
```

### Real Example: Feedback Tool Testing

```
USER: Sarah (Marketing Manager)
DATE: Oct 20, 2024

TASK COMPLETION:
✅ Completed: Submitted feedback successfully
Time taken: 1 min 45 sec

OBSERVATIONS:
- Paused for 10 seconds looking at Category dropdown (wasn't sure which to pick)
- Tried to click "Submit" without filling email (validation worked correctly)
- Smiled when she saw the success message
- Didn't notice the "View Past Feedback" button initially (had to scroll)

DIRECT QUOTES:
"Oh, this is way easier than emailing support!"
"I wish the category options were explained a bit more"
"Wait, I can see my past feedback? That's actually really useful"

FEEDBACK:
What worked: 
- Form was simple and fast
- Validation was clear
- Success message felt rewarding

What didn't work:
- Category options unclear ("Bug Report" vs "Feature Request" - what's the difference?)
- "View Past Feedback" button too subtle
- Wanted to know response time expectations

Suggestions:
- Add tooltip explaining each category
- Make past feedback button more prominent
- Add text like "We typically respond within 48 hours"

SUCCESS METRIC:
✅ Submit feedback under 2 minutes: YES (1:45)
✅ Completed without asking for help: YES
```

### Common Testing Patterns

**Pattern 1: User completes task easily**
✅ Good sign! But still ask what could be better.

**Pattern 2: User completes task after struggling**
⚠️ Fix the friction points. The tool works but isn't intuitive.

**Pattern 3: User abandons task**
🚩 Critical issues. Core flow doesn't work. Major changes needed.

**Pattern 4: User completes task but says they wouldn't use it**
🚩 Tool works but doesn't solve the real problem. Revisit Step 1.

### Remote vs. In-Person Testing

**In-Person (Best):**
- See facial expressions and body language
- Easier to probe deeper
- Can point at screen

**Video Call (Good):**
- Screen sharing works well
- Can see reactions via webcam
- Record the session (with permission)

**Async (Okay for MVPs):**
- Send link + instructions
- Ask them to record their thoughts
- Follow up with questions
- Less rich data but better than nothing

### ✅ Checkpoint #10

After user testing:
- [ ] Tested with 3-5 users (or appropriate number for your target)
- [ ] Detailed notes from each session
- [ ] Identified patterns across users
- [ ] Know what worked well
- [ ] Know what needs fixing
- [ ] Measured against success criteria from Step 1
- [ ] Have quotes to share with stakeholders

🎯 **Reality Check:** If 3+ out of 5 users couldn't complete the core task, don't polish—redesign.

---

<a id="step-11-analyze-feedback"></a>
## Step 11: Analyze Feedback (30-60 min)

Now synthesize what you learned into actionable insights.

### Pattern Analysis

Look across all your user tests for patterns.

**Create three lists:**

```
✅ WORKED WELL (mentioned by 3+ users):
- [Thing that worked]
- [Thing that worked]
- [Thing that worked]

⚠️ FRICTION POINTS (2+ users struggled):
- [Issue 1]: [How many users hit this]
- [Issue 2]: [How many users hit this]

🚩 CRITICAL ISSUES (blocked task completion):
- [Blocker 1]: [How many users couldn't complete]
- [Blocker 2]: [How many users couldn't complete]
```

### Real Example: Feedback Tool Analysis

```
✅ WORKED WELL (mentioned by 4/5 users):
- "Super fast to submit" - all 5 users under 2 minutes
- "Success message felt good" - 4/5 mentioned they felt confirmed
- "Cleaner than emailing" - 4/5 compared favorably to current process

⚠️ FRICTION POINTS (2+ users struggled):
- Category dropdown confusion - 3/5 hesitated, not sure which to pick
- "View Past Feedback" button too hidden - 4/5 didn't see it initially
- No guidance on response time - 3/5 asked when they'd hear back

🚩 CRITICAL ISSUES (blocked task completion):
- None! All 5 users completed the core task
- One user initially missed required email field but validation caught it
```

### Success Criteria Check

Go back to your success criteria from Step 1:

```
ORIGINAL SUCCESS CRITERIA:
[Metric 1]: [Did we hit it? Yes/No/Partial]
[Metric 2]: [Did we hit it? Yes/No/Partial]
[Metric 3]: [Did we hit it? Yes/No/Partial]

EVIDENCE:
[What from testing proves/disproves each metric]
```

### Real Example:

```
ORIGINAL SUCCESS CRITERIA:
✅ 3/5 users complete task under 2 minutes: YES (all 5 users: 1:15-2:10)
✅ No user needs to ask for help: YES (all completed independently)
⚠️ Users rate it 7+ out of 10: PARTIAL (ratings: 7, 8, 6, 8, 7 - avg 7.2)

EVIDENCE:
- All users submitted feedback successfully
- Time range: 1:15 to 2:10 (target was 2:00)
- No one asked for help, but 3 users had hesitation moments
- Lower ratings mentioned: category confusion, hidden features
```

### Prioritize Fixes

Not all feedback is equally important. Prioritize:

```
MUST FIX (blocking user success):
1. [Critical issue that prevented completion]
2. [Critical issue that prevented completion]

SHOULD FIX (major friction):
3. [Issue that caused significant struggle]
4. [Issue that caused significant struggle]

COULD FIX (nice to have):
5. [Polish item that would improve experience]
6. [Feature request that's interesting]

WON'T FIX (out of scope):
- [Thing users wanted but doesn't fit your goals]
- [Feature that's too complex for this prototype]
```

### Real Example:

```
MUST FIX (blocking user success):
None! Core flow works.

SHOULD FIX (major friction):
1. Add tooltips explaining each category option
2. Make "View Past Feedback" button more prominent (larger, different color)
3. Add expected response time message

COULD FIX (nice to have):
4. Add character limit indicator on message field
5. Allow users to edit submitted feedback
6. Add ability to attach screenshots

WON'T FIX (out of scope):
- Real-time admin notification (separate admin tool needed)
- Voting on other feedback (community feature, too complex)
- Integrating with existing ticketing system (requires engineering)
```

### Unexpected Insights

**Look for surprises:**
- Features you thought were important that users didn't care about
- Features you thought were minor that users loved
- Use cases you hadn't considered
- Misunderstandings about the purpose

**Document these:**
```
SURPRISING LEARNINGS:
- [Thing you didn't expect]
- [Thing you didn't expect]
- [How this changes your thinking]
```

### Stakeholder Summary

Prepare a one-pager for stakeholders:

```
PROTOTYPE TESTING SUMMARY

WHAT WE TESTED:
[Brief description]

WHO WE TESTED WITH:
[X users, their profiles]

KEY RESULTS:
✅ [Main success]
✅ [Main success]
⚠️ [Main issue found]

SUCCESS METRICS:
[Metric 1]: [Result]
[Metric 2]: [Result]

TOP 3 FIXES NEEDED:
1. [Fix 1]
2. [Fix 2]
3. [Fix 3]

RECOMMENDED NEXT STEP:
[Polish and iterate / Pivot / Hand to engineering / etc.]
```

### ✅ Checkpoint #11

After analysis:
- [ ] Identified patterns across users (not just individual feedback)
- [ ] Checked against original success criteria
- [ ] Prioritized fixes (must/should/could/won't)
- [ ] Noted surprising insights
- [ ] Prepared stakeholder summary
- [ ] Know what decision you're making next (Step 12)

🎯 **Reality Check:** If you have 20+ "must fix" items, your prototype wasn't ready for testing. Simplify scope and retest.

---

<a id="step-12-polish-pivot"></a>
## Step 12: Polish or Pivot (1-2 hours)

Based on your analysis, decide: iterate and polish, or pivot to a different approach.

### The Decision Framework

Use this flowchart to decide your path:

```
                    START: Review User Testing Results
                                    │
                                    ▼
            ┌───────────────────────────────────────────┐
            │  Did users complete the core task?        │
            └───────────┬───────────────────────────────┘
                        │
            ┌───────────┴───────────┐
            │                       │
           YES                     NO
            │                       │
            ▼                       ▼
    ┌───────────────┐      ┌──────────────────┐
    │ Did it meet   │      │  Consider PIVOT  │
    │ success       │      │  or major        │
    │ criteria?     │      │  redesign        │
    └───────┬───────┘      └──────────────────┘
            │
    ┌───────┴────────┐
    │                │
   YES            PARTIAL
    │                │
    ▼                ▼
┌─────────────┐  ┌──────────────────┐
│   POLISH    │  │ POLISH & RETEST  │
│             │  │                  │
│ • Fix must  │  │ • Fix critical   │
│   items     │  │   issues         │
│ • Ship it!  │  │ • Test with      │
│             │  │   2-3 new users  │
└─────────────┘  └──────────────────┘


                    DECISION PATHS
                    
┌──────────────────────────────────────────────────────┐
│  Path 1: POLISH (2-4 hours)                          │
├──────────────────────────────────────────────────────┤
│  Choose when:                                        │
│  ✓ Core functionality works                          │
│  ✓ Users completed main task                         │
│  ✓ Hit most success criteria                         │
│  ✓ Feedback is about improvements, not blockers      │
│                                                      │
│  Action:                                             │
│  1. Fix "MUST FIX" items                            │
│  2. Fix "SHOULD FIX" items (time permitting)        │
│  3. Light retest (1-2 users)                        │
│  4. → Proceed to Phase 5 (Deploy)                   │
└──────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────┐
│  Path 2: POLISH & RETEST (4-8 hours)                 │
├──────────────────────────────────────────────────────┤
│  Choose when:                                        │
│  ⚠ Core works but has significant friction           │
│  ⚠ Users struggled but completed task                │
│  ⚠ Hit some success criteria but not all             │
│  ⚠ Fixes might significantly change experience       │
│                                                      │
│  Action:                                             │
│  1. Fix "MUST FIX" items                            │
│  2. Fix "SHOULD FIX" items                          │
│  3. Full retest with 2-3 NEW users                  │
│  4. Analyze again                                    │
│  5. → Then proceed to Phase 5                        │
└──────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────┐
│  Path 3: PIVOT (2-4 hours + restart)                 │
├──────────────────────────────────────────────────────┤
│  Choose when:                                        │
│  ❌ Users couldn't complete core task                │
│  ❌ Missed most success criteria                     │
│  ❌ Users said they wouldn't use it                  │
│  ❌ Built the wrong solution                         │
│                                                      │
│  Action:                                             │
│  1. Document what you learned                        │
│  2. Revisit Step 1 (problem definition)             │
│  3. Consider: Is this the right problem?            │
│  4. Choose: Restart with simpler approach OR        │
│            Solve different problem OR               │
│            Use existing tool instead                │
└──────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────┐
│  Path 4: HAND TO ENGINEERING (Documentation phase)   │
├──────────────────────────────────────────────────────┤
│  Choose when:                                        │
│  ⚠ Prototype proves value but needs production code  │
│  ⚠ Users love it but technical complexity is high    │
│  ⚠ Security/compliance requirements emerged          │
│  ⚠ Scale requirements are clear                      │
│                                                      │
│  Action:                                             │
│  1. Document everything learned                      │
│  2. Create handoff document (see Step 14)           │
│  3. Set up meeting with engineering                  │
│  4. Position as reference, not production code       │
└──────────────────────────────────────────────────────┘
```

### Making the Decision

Answer these questions to clarify your path:

**1. Did users accomplish the core task?**
- ✅ Yes → Move to polish
- ❌ No → Consider pivot

**2. Did it meet your success criteria?**
- ✅ Yes → Move to polish
- ⚠️ Partial → Fix key issues, then retest
- ❌ No → Pivot or major redesign

**3. Would users actually use this?**
- ✅ Yes → Move to polish
- ❌ No → Pivot (you built the wrong thing)

**4. Is it solving the right problem?**
- ✅ Yes → Move to polish
- ❌ No → Go back to Step 1

### Decision Path: POLISH

**Choose this if:**
- Core functionality works
- Users completed main task
- Feedback is mostly about improvements, not fundamental issues
- You hit most success criteria

**What to do:**
1. Implement the "MUST FIX" items from Step 11
2. Implement the "SHOULD FIX" items (time permitting)
3. Do one more round of light testing
4. Proceed to Phase 5 (Deploy)

**Prompt for polishing:**
```
Based on user testing, I need to make these improvements:

CRITICAL:
1. [Must fix item 1]
2. [Must fix item 2]

IMPORTANT:
3. [Should fix item 1]
4. [Should fix item 2]

For each fix, maintain existing functionality. Let me test after each change.
```

### Decision Path: POLISH & RETEST

**Choose this if:**
- Core works but has significant friction
- Users completed task but struggled
- Hit some success criteria but not all
- Fixes might change user experience significantly

**What to do:**
1. Implement "MUST FIX" items
2. Implement "SHOULD FIX" items
3. Test with 2-3 new users
4. Analyze again
5. Then proceed to Phase 5

**Timeline:** Add 2-4 hours for fixes + retesting

### Decision Path: PIVOT

**Choose this if:**
- Users couldn't complete core task
- Missed most success criteria
- Users said they wouldn't use it
- You built the wrong solution

**What to do:**
```
PIVOT CHECKLIST:
□ Document what you learned (what didn't work and why)
□ Revisit Step 1 (problem definition)
□ Consider: Is this the right problem to solve?
□ Option A: Restart with simpler approach
□ Option B: Solve a different problem
□ Option C: Use existing tool instead of building
```

**When to pivot:**
- Testing revealed fundamental misunderstanding of user needs
- The problem is bigger/different than you thought
- Technical approach isn't working
- Users want something completely different

**Pivot prompt:**
```
Based on user testing, I need to reconsider our approach.

WHAT WE BUILT:
[Description]

WHAT WE LEARNED:
[Key insights from testing]

WHAT USERS ACTUALLY NEED:
[What testing revealed]

Can you suggest 3 alternative approaches that better address what users actually need? Keep it simple and feasible for prototyping.
```

### Decision Path: HAND TO ENGINEERING

**Choose this if:**
- Prototype proves value, but technical complexity exceeds vibe coding
- Users love it, but it needs production-quality code
- Security/compliance requirements emerge
- Scale requirements are clear

**What to do:**
1. Document everything you learned
2. Create handoff document (see Phase 5, Step 14)
3. Set up meeting with engineering
4. Position prototype as reference, not production code

### Real Example: Feedback Tool Decision

```
DECISION: POLISH & RETEST

REASONING:
✅ All users completed core task
✅ Users said they would use it
⚠️ Average rating 7.2/10 (target was 7+, barely met)
⚠️ Several friction points that could improve experience

POLISH PLAN:
1. Add category tooltips (2 min fix)
2. Make "View Past Feedback" button prominent (5 min fix)
3. Add response time expectation text (2 min fix)
4. Increase mobile button sizes (5 min fix)

RETEST PLAN:
Test with 2 new users after fixes
Target: 8+ out of 10 ratings
If successful → Deploy
If not → Analyze further
```

### Making the Call

**Tips for deciding:**

💡 **Don't over-polish:** If users complete the task and say they'd use it, don't aim for perfection. Ship it.

💡 **Don't under-react:** If 3+ users had the same critical issue, it needs fixing before deployment.

💡 **Trust patterns, not individuals:** One user's feedback might be an outlier. Look for what 2-3+ users mentioned.

💡 **Time-box polishing:** Give yourself max 2 hours for polish fixes. If it takes longer, reconsider.

### ✅ Checkpoint #12

Before moving to Phase 5:
- [ ] Made clear decision (polish, pivot, or hand off)
- [ ] If polishing: List of specific fixes is ready
- [ ] If pivoting: Documented learnings and new direction
- [ ] If handing off: Documentation prepared
- [ ] Realistic about timeline for next steps
- [ ] Have updated stakeholder on status

🎯 **Reality Check:** Most projects should choose "polish" if they followed the framework. If you're pivoting, reflect on whether early steps were thorough enough.

---

# PHASE 5: SHARE & DECIDE
**Time Investment: 1-2 hours**  
**This is where you decide what happens to your prototype**

<a id="step-13-deploy"></a>
## Step 13: Deploy Your Prototype (30-60 min)

Time to make your prototype accessible to others beyond your test users.

### Pre-Deployment Checklist

Before deploying anything:

```
FUNCTIONALITY:
□ All core features work
□ Tested on mobile and desktop (if needed)
□ No critical bugs
□ Error messages are user-friendly
□ Success states are clear

CONTENT:
□ No test/dummy data visible
□ No placeholder text ("Lorem ipsum", "Coming soon")
□ No profanity or internal jokes
□ Contact info is correct (if any)

SECURITY:
□ No exposed API keys or credentials
□ No sensitive data hard-coded
□ Input validation is working
□ No obvious security holes

PRESENTATION:
□ Looks professional enough for audience
□ Branding is consistent (if applicable)
□ No broken images or links
□ Mobile experience is acceptable (if needed)

EXPECTATIONS:
□ Stakeholders know this is a prototype
□ Documented known issues
□ Clear about what it does/doesn't do
```

### Deployment Options by Target Type

#### For POC (Proof of Concept)

**Don't deploy!** Keep it local.

- Show it via screen share
- Record a quick video demo
- Take screenshots for documentation

**Why:** POCs are disposable. No need to make them publicly accessible.

#### For MVP (User Testing)

**Recommended: Use free, simple hosting**

**Option 1: Claude Artifacts (Simplest)**
- Already hosted when you build
- Get shareable link
- Limitation: Requires Claude access to view

**Option 2: Replit (Great for beginners)**
1. Go to replit.com
2. Create new Repl
3. Copy your code from Claude
4. Click "Run"
5. Share the URL
- Pros: Free, instant, no setup
- Cons: Replit branding, may sleep after inactivity

**Option 3: Vercel (More professional)**
1. Export code from Claude
2. Go to vercel.com
3. Sign up (free tier)
4. Drag and drop your project folder
5. Get deployment URL
- Pros: Fast, professional, custom domain possible
- Cons: Slight learning curve

**Prompt for export:**
```
I need to deploy this prototype. Can you provide:
1. All the code organized in files (HTML, CSS, JS)
2. Any setup instructions needed
3. What hosting platform would you recommend for this specific project?
```

#### For Demo (Stakeholder Presentation)

**Recommended: Professional hosting + custom domain (optional)**

Use Vercel (above) but also:
- Get custom domain if possible (makes it feel real)
- Test extensively before the presentation
- Have backup plan (screen recording) if hosting fails
- Consider: Record a polished video demo as backup

#### For Internal Tool (Team Use)

**Recommended: Stable hosting with authentication**

**Option 1: Keep in Claude Projects**
- If team has Claude access
- Good for tools used sporadically

**Option 2: Deploy with simple auth**
- Use Vercel + password protection
- Or Replit with auth enabled

**Option 3: Hand to IT/Engineering**
- For tools that need to be reliable
- IT can deploy to company infrastructure

### How to Share Your Deployed Prototype

**Create a Share Package:**

```
Subject: [Prototype Name] - Ready for Review

Hi [Recipients],

I've built a working prototype of [brief description].

🔗 LIVE LINK: [URL]

📋 WHAT IT DOES:
[2-3 sentences about core functionality]

👤 WHO IT'S FOR:
[Target users]

✅ WHAT WORKS:
- [Feature 1]
- [Feature 2]
- [Feature 3]

⚠️ KNOWN LIMITATIONS:
- [Limitation 1]
- [Limitation 2]

🎯 WHAT I NEED FROM YOU:
[Try it out and let me know: feedback/approval/next steps]

Best,
[Your name]
```

### Monitoring After Deployment

Even for prototypes, basic monitoring helps:

**For Simple Tracking:**
```
Ask Claude: "Can you add simple analytics to track:
- How many people visit
- Which features they use most
- Where they drop off

Use a free tool that's easy to set up."
```

**For Bug Reports:**
- Set up simple feedback form
- Monitor your email for issues
- Check in with users after a few days

### Deployment Troubleshooting

**"The link doesn't work"**
- Check if hosting is still active
- Verify URL is correct
- Test in incognito window
- Try different browser

**"It works for me but not for others"**
- Browser compatibility issue
- Have them send screenshot
- Test on their device type

**"It's really slow"**
```
The deployed version is loading slowly.
Can you optimize for:
- Smaller file sizes
- Faster load times
- Better performance

Keep functionality the same.
```

### ✅ Checkpoint #13

After deployment:
- [ ] Prototype is accessible via URL
- [ ] Tested the live link yourself
- [ ] At least one other person has accessed it successfully
- [ ] Known limitations are documented
- [ ] Stakeholders have been notified with appropriate context
- [ ] You have a way to get feedback/bug reports
- [ ] Backup plan ready (screenshots/video) if link fails

🎯 **Reality Check:** Deployment should take 30-60 minutes max. If it's taking hours, you're over-complicating it. Keep it simple.

---

<a id="step-14-whats-next"></a>
## Step 14: Plan What's Next (30-60 min)

Your prototype is live. Now decide what happens to it.

### The Decision Tree

Answer this question first:

**"What was the goal of this prototype?"**

```
□ Prove technical feasibility → Probably done, hand off findings
□ Get stakeholder buy-in → Present results, get decision
□ Test with real users → Analyze results, iterate or hand off
□ Solve internal problem → Keep using it, plan maintenance
□ Show what's possible → Mission accomplished, document learnings
```

### Path 1: This Was a POC → Hand to Engineering

**When to choose this:**
- You proved the concept works
- Goal was validation, not production
- Engineering will build the real thing

**What to document:**

```
POC HANDOFF DOCUMENT

PROJECT: [Name]
GOAL: [What we wanted to prove]
OUTCOME: [What we learned]

✅ WHAT WORKED:
- [Technical approach that worked]
- [User feedback that validated concept]
- [Unexpected wins]

❌ WHAT DIDN'T WORK:
- [Technical limitations discovered]
- [User friction points]
- [Things harder than expected]

🔑 KEY LEARNINGS:
1. [Important insight 1]
2. [Important insight 2]
3. [Important insight 3]

📊 USER TESTING RESULTS:
- [Number tested]
- [Success rate]
- [Key quotes]

💡 RECOMMENDATIONS FOR PRODUCTION:
1. [Technical recommendation]
2. [Feature recommendation]
3. [Design recommendation]

🔗 PROTOTYPE LINK:
[URL - as reference only, not production code]

⏭️ SUGGESTED NEXT STEPS:
[What engineering should do next]
```

### Path 2: This is an Internal Tool → Plan Maintenance

**When to choose this:**
- Solves operational problem
- Team will use it regularly
- Good enough as-is

**⚠️ Important Reality Check:**

Vibe-coded tools are NOT production-grade. They will break. Plan for it.

**Maintenance Plan Template:**

```
INTERNAL TOOL MAINTENANCE PLAN

TOOL NAME: [Name]
PURPOSE: [What it does]
USERS: [Who uses it]

🔄 EXPECTED MAINTENANCE:
- Updates needed: [Weekly/Monthly/Quarterly]
- Estimated time per update: [X hours]
- Who maintains it: [Your name + backup]

⚠️ KNOWN LIMITATIONS:
1. [Limitation 1]
2. [Limitation 2]
3. [Limitation 3]

🚨 WHEN TO INVOLVE ENGINEERING:
- If [condition 1]
- If [condition 2]
- If usage grows beyond [X users]

📋 BACKUP PLAN:
If this tool breaks:
1. [Fallback process]
2. [Who to contact]
3. [Data recovery plan if needed]

📚 DOCUMENTATION:
- User guide: [Link]
- Technical notes: [Link]
- Known issues: [Link]
```

**Set Realistic Expectations:**

```
Team announcement:

I've built [tool name] to help with [problem].

✅ It's ready to use for [purpose]

⚠️ Important: This is a prototype-grade tool
- It may have bugs
- It will need occasional maintenance
- If it becomes critical, we should involve engineering

Please report issues to [your email/slack]
```

### Path 3: This Will Become a Real Product → Collaborate with Engineering

**When to choose this:**
- User validation was successful
- This needs to be production-ready
- You want to ship this to customers

**Engineering Collaboration Plan:**

```
ENGINEERING HANDOFF PLAN

PROJECT: [Name]
WHY THIS MATTERS: [Business case from user testing]

✅ PROTOTYPE VALIDATES:
- [User need 1]
- [User need 2]
- [Technical feasibility]

📊 USER TESTING DATA:
- Tested with [X] users
- [Y]% completion rate
- Average rating: [Z]/10
- Key insight: [Main learning]

🎯 PRODUCTION REQUIREMENTS:
MUST HAVE:
- [Requirement 1]
- [Requirement 2]

SHOULD HAVE:
- [Requirement 3]
- [Requirement 4]

🔒 PRODUCTION CONCERNS:
- Security: [What needs review]
- Scale: [Expected load]
- Integration: [What systems to connect]
- Compliance: [Any regulations]

🔗 PROTOTYPE AS REFERENCE:
URL: [Link]
Note: This is reference only, not production code
Use it to understand: UX flow, feature requirements, edge cases

⏱️ TIMELINE:
Prototype took: [X hours]
Production build estimate: [Multiply by 3-10x]

📅 NEXT STEPS:
1. [Engineering reviews prototype]
2. [Technical planning session]
3. [Production design/architecture]
4. [Development begins]

🤝 COLLABORATION MODEL:
- I own: Product decisions, user testing, feedback
- Engineering owns: Code quality, security, architecture
- We collaborate on: Feature prioritization, technical tradeoffs
```

**The Handoff Meeting:**

Schedule 30-60 minute meeting with engineering:

**Agenda:**
1. Demo the prototype (5 min)
2. Share user testing results (10 min)
3. Discuss technical learnings (10 min)
4. Answer engineering questions (20 min)
5. Define next steps (10 min)

**Come prepared with:**
- Live prototype demo
- User testing summary
- List of edge cases you discovered
- Known technical limitations
- Your product priorities

### Path 4: This Didn't Work → Document and Move On

**When to choose this:**
- User testing showed it doesn't solve the problem
- Technical approach isn't feasible
- Problem isn't worth solving after all

**This is success too!** You learned something quickly before investing engineering months.

**Failure Report Template:**

```
PROJECT RETROSPECTIVE: [Name]

❌ OUTCOME: Prototype didn't validate hypothesis

ORIGINAL HYPOTHESIS:
[What we thought would work]

WHAT WE BUILT:
[Brief description]

WHAT WE LEARNED:
[Why it didn't work]

USER TESTING INSIGHTS:
- [Key learning 1]
- [Key learning 2]
- [Key learning 3]

💡 WHAT THIS MEANS:
[Implications for product strategy]

⏭️ ALTERNATIVE APPROACHES:
1. [Could try this instead]
2. [Or this]
3. [Or maybe this isn't the right problem]

⏱️ TIME INVESTMENT:
Total time: [X hours]
Value: Saved engineering [weeks/months] of work

🔗 PROTOTYPE LINK:
[URL - archived for reference]
```

**Share the learnings:**
- Failed experiments are valuable
- Document why it didn't work
- Share with team so others learn
- This is how product discovery works

### Red Flags That Require Engineering

**⚠️ Involve engineering NOW if:**

```
□ Handling payment information
□ Storing sensitive user data (PII, health, financial)
□ Need 100+ concurrent users
□ Integrating with complex existing systems
□ Subject to compliance (HIPAA, SOC2, GDPR, etc.)
□ Requires high availability (downtime = major problem)
□ Security is business-critical
□ Performance is business-critical
```

Don't try to vibe-code these. Seriously.

### Timeline Reality Check

**Prototype to production timeline:**

- Simple tool: Prototype [X hours] → Production [3-5X hours]
- Medium complexity: Prototype [X hours] → Production [5-10X hours]
- Complex features: Prototype [X hours] → Production [10-20X hours]

**Why the multiplier?**
Production code needs:
- Security review
- Error handling for ALL edge cases
- Performance optimization
- Testing (unit, integration, E2E)
- Documentation
- Code review
- Architecture that scales
- Monitoring and logging
- Proper database design
- Deployment infrastructure

### ✅ Checkpoint #14

Before closing this project:
- [ ] Chosen clear next path (hand off/maintain/collaborate/move on)
- [ ] Documentation complete for chosen path
- [ ] Stakeholders informed of decision
- [ ] If continuing: Maintenance plan exists
- [ ] If handing off: Engineering has what they need
- [ ] Learnings documented for future reference
- [ ] Celebrated what you accomplished!

🎯 **Reality Check:** The prototype was the easy part. Production takes 3-10x longer. Make sure the business case justifies that investment.

---

# PART 4: COMPLETE WALKTHROUGH

<a id="walkthrough-feedback-tool"></a>
## Case Study: Building a Customer Feedback Tool

Let me walk you through a real example from start to finish.

### The Challenge

**Background:**
Sarah is a Product Manager at a B2B SaaS company. Customer feedback currently comes through scattered channels: support emails, sales calls, Slack messages. There's no central place to track feedback or see what's been addressed.

**Goal:**
Build a simple prototype to validate whether a centralized feedback tool would solve this problem.

---

### PHASE 1: THINK BEFORE YOU BUILD

#### Step 1: Define the Problem

**Sarah's Problem Definition:**

```
PROBLEM STATEMENT:
Customer feedback is scattered across email, Slack, and sales calls. We have no way to track what feedback we've received, what we've acted on, or which requests are most common. This leads to:
- Lost feedback that never gets reviewed
- Customers feeling unheard (ask about same issues repeatedly)
- Product team can't prioritize based on demand

REAL EXAMPLE:
Last month, 5 customers requested API rate limit increases via different channels. We didn't realize it was a pattern until the 5th request.

TARGET USER:
Role: Existing B2B customers (technical and non-technical)
Context: They use our product daily, encounter issues/ideas, want to share feedback
Tech level: Mixed (some developers, some business users)
Key frustrations: "I told support about this bug 3 months ago, is anyone looking at it?"
Success for them: Submit feedback easily, see status of their past feedback

EXISTING SOLUTIONS:
- Canny: Good but $400/mo, too expensive for MVP test
- Google Forms: Free but no status tracking for users
- Intercom: We have it, but feedback gets lost in support tickets
Our advantage: Custom to our needs, integrated status tracking

SUCCESS CRITERIA:
1. 80% of test users can submit feedback in under 2 minutes
2. Users can see status of their past feedback
3. Internal team (me) can easily see all feedback in one place
4. 3+ beta customers use it within first week

OUT OF SCOPE:
- Admin dashboard (separate project)
- Email notifications (can add later)
- Voting on others' feedback (nice-to-have)
- Integration with Jira (too complex for MVP)

WHY SOFTWARE?
Google Form could handle submission, but can't show users their feedback status. Existing tools are too expensive or not the right fit. This needs to be custom, but simple.
```

#### Step 2: Pressure-Test with AI

Sarah's prompt to Claude:

```
I'm planning to build a customer feedback tool for B2B SaaS customers.

CONTEXT:
Problem: Feedback is scattered, customers can't track their submissions
Target users: B2B customers (mix of technical and non-technical)
Success looks like: Easy submission + status tracking for users

CHALLENGE THIS IDEA:
1. What am I assuming that might be wrong?
2. What are 3 alternative approaches I haven't considered?
3. What will be hardest to build or maintain?
4. What could make this fail with users?
5. What's the absolute simplest version that could work?
6. Is there an existing tool I should use instead?

Be skeptical and direct.
```

Claude's response highlighted:
- **Assumption risk:** "You're assuming customers WANT to track status. They might just want acknowledgment."
- **Alternative:** "Use Typeform + Airtable combo for MVP testing"
- **Hardest part:** "Status tracking requires backend/database - are you ready for that complexity?"
- **Simplest version:** "Start with submission only, add status tracking in v2"

Sarah's decision: Start with submission + basic status tracking. Status is the differentiator vs. Google Forms.

#### Step 3: Choose Target

Sarah chose: **MVP (Test with real users)**

```
TARGET: MVP

PRIMARY GOAL:
Validate that customers want/use feedback submission with status tracking

AUDIENCE:
5-10 beta customers (mix of technical and business users)

QUALITY BAR:
Must work: Submission form, view past feedback with status
Should work: Mobile responsive, clean design
Nice to have: Categories, filtering

SUCCESS METRIC:
- 5+ customers submit feedback in first week
- 3+ customers check status of past feedback
- Average usability rating 7+/10

WHAT HAPPENS NEXT:
If successful: Build proper admin dashboard, hand to engineering
If not successful: Use simpler solution (Google Form + manual tracking)
```

---

### PHASE 2: PLAN YOUR BUILD

#### Step 4: Describe What You Want

```
ONE-SENTENCE SUMMARY:
A form where customers submit feedback and can see the status of all their past submissions.

USER FLOW:
1. Customer lands on feedback page
2. Sees form: Name (optional), Email (required), Feedback (textarea), Category (dropdown)
3. Clicks "Submit Feedback"
4. Sees success message: "Thanks! We'll review this within 48 hours."
5. Clicks "View My Past Feedback"
6. Enters email, sees list of their submissions
7. Each submission shows: Date, Category, Message preview, Status badge

SUCCESS OUTCOME:
Customer can submit feedback in under 90 seconds and check on any past feedback whenever they want.

CONSTRAINTS:
Device: Mobile-first (many customers on-the-go), but works on desktop
Data: Need simple storage (suggest Firebase or similar easy solution)
Design: Clean, modern, friendly (not intimidating)
Performance: Form submits in under 2 seconds

REFERENCE EXAMPLES:
- Form feel: Like Typeform (friendly, not corporate)
- Status display: Like package tracking (clear progress indicators)
- Overall aesthetic: Like Linear (clean, modern, lots of white space)

NOT INCLUDED:
- User accounts/passwords
- Admin dashboard (separate project)
- Email notifications
- File attachments
```

#### Step 5: Break Down Features

```
MUST HAVE:
- [ ] #1 Feedback form (Name optional, Email req, Message req, Category dropdown)
- [ ] #2 Form validation (proper email, non-empty message)
- [ ] #3 Submit with success message
- [ ] #4 View past feedback (by email lookup)
- [ ] #5 Status badges (New/Reviewing/Implemented)

SHOULD HAVE:
- [ ] #6 Mobile responsive design
- [ ] #7 Character counter on message field
- [ ] #8 Empty states ("No feedback yet")

COULD HAVE:
- [ ] #9 Filter by category
- [ ] #10 Search past feedback

WON'T HAVE:
- Admin panel
- Edit/delete submitted feedback
- Real-time updates
- Voting/commenting
```

#### Step 6: First Prompt

```
I want to build a customer feedback form where users can submit feedback and see their past submissions with status tracking.

CONTEXT:
Users: B2B SaaS customers (mix of technical and business users)
Problem: Currently no central place for feedback, customers can't track what happens to their requests
Success: Users can submit in under 90 seconds and check status anytime

TECHNICAL CONSTRAINTS:
- Mobile-first, but works on desktop
- Need simple data storage (suggest easiest approach)
- Form submit should be fast (under 2 seconds)

LET'S START WITH:
Build the feedback submission form.

Specifically:
- Fields: Name (optional text), Email (required, validated), Feedback (required textarea, 500 char max), Category (dropdown: Bug Report, Feature Request, General Feedback, Other)
- Submit button that validates, submits, shows success message
- Success message: "Thanks! We'll review this within 48 hours."
- After submission, clear form and keep success message for 3 seconds

Design: Clean and modern with lots of white space, friendly tone (not corporate)
Colors: Use soft blue (#4A90E2) for accents

Please build this and show me what it looks like. Ask if anything is unclear.
```

---

### PHASE 3: BUILD WITH CLAUDE

#### Step 7-8: The Build (Abbreviated Conversation)

**Exchange 1:**

```
Sarah: [First prompt above]

Claude: [Builds initial form with all fields, validation, and success message]

Sarah: This looks great! But the textarea is too small on mobile - can you make it taller (at least 120px) and the submit button bigger (48px height)?

Claude: [Updates the styling]

Sarah: Perfect. Now let's add the "View My Past Feedback" feature.

What it should do:
- Add a button below the form: "View My Past Feedback"
- When clicked, show a simple input asking for email
- After entering email and clicking "Show My Feedback", display list of all feedback from that email
- Each item shows: Date (formatted nicely), Category (as badge), Message (first 60 characters + "..."), Status (colored badge)
- Status options: "New" (blue), "Reviewing" (yellow), "Implemented" (green), "Won't Fix" (gray)
- If no feedback found, show: "No feedback found for this email. Submit your first piece of feedback above!"

For now, use dummy data (create 3 sample feedback items) so we can see how it looks.

Claude: [Builds the past feedback view with dummy data]
```

**Exchange 2:**

```
Sarah: Good! But I notice the feedback list isn't very readable. Can you:
- Add more space between each feedback item
- Make the date smaller and lighter gray
- Put the status badge on the right side instead of left
- Add a subtle border between items

Claude: [Makes styling improvements]

Sarah: Much better. Now let's talk about data persistence. Currently it's just dummy data. What's the simplest way to actually store submissions and retrieve them by email?

Claude: I can suggest two approaches:

1. **Simplest (Browser LocalStorage):**
   - Stores data in user's browser
   - No backend needed
   - Limitation: Only works on same device/browser
   
2. **Simple Backend (Firebase):**
   - Free tier available
   - Real database storage
   - Works across devices
   - Requires Firebase setup (I can guide you)

For an MVP, I'd recommend Firebase. Would you like me to integrate that?

Sarah: Yes, let's use Firebase. Please guide me through what I need to do, then integrate it.

Claude: [Provides step-by-step Firebase setup instructions, then integrates Firebase code]
```

**Exchange 3:**

```
Sarah: Following your instructions, I set up Firebase. But when I try to submit, I get an error about Firebase not being initialized. Can you help?

Claude: I need to see the error message. Can you copy it here?

Sarah: [Pastes error]

Claude: Ah, you need to add your Firebase config. In the Firebase console, go to Project Settings > Your apps > Firebase SDK snippet. Copy the config object and replace the placeholder in the code.

Sarah: [Does that] - It works! I just submitted test feedback and I can see it when I check my past feedback.

Claude: Great! Let me add error handling so if Firebase is down, users get a friendly message instead of a technical error.

[Adds error handling]
```

#### Step 9: Quality Checkpoint

After 5 features, Sarah does a checkpoint:

```
Sarah: Let's pause and review. Can you:
1. Explain the main parts of what we've built
2. Check for any security issues
3. Identify any problems with the current approach

Claude: [Provides overview]

Main components:
- Feedback form with validation
- Firebase integration for data storage
- Past feedback viewer with email lookup

Security concerns:
- Currently anyone can view any email's feedback (just need to guess email)
- No rate limiting on submissions (could be spammed)

Suggestions:
- For MVP: Add simple rate limiting (max 10 submissions per hour)
- Future: Add user authentication for viewing feedback

Technical issues:
- Status is hard-coded (you'll need manual process to update)
- No admin panel to manage feedback
```

Sarah's response:

```
Good catches. Let's add rate limiting now.
For status updates and admin panel - those are separate projects, out of scope for this MVP.
I'll manually update Firebase data for now during testing.
```

---

### PHASE 4: VALIDATE

#### Step 10: User Testing

Sarah tested with 5 beta customers. Here's one example:

**User: Mike (Technical Founder)**

```
Task: "Submit a feature request about API rate limits"

Observations:
[0:15] Loads page, immediately starts typing
[0:30] Pauses at category dropdown, hovers over options
[0:35] Selects "Feature Request"
[0:50] Submits form
[0:52] Sees success message, smiles
[1:00] Scrolls down, notices "View My Past Feedback" button
[1:05] Clicks it, enters email
[1:10] Sees his submission, nods approvingly

Total time: 1:10

Follow-up:
"How easy was that?" → "Super easy, 9/10"
"What was confusing?" → "Wasn't sure if 'Bug Report' or 'Feature Request' was right for API limits, but picked one"
"Would you use this?" → "Definitely. Way better than emailing support."
"What's missing?" → "Would be nice to get notified when status changes"
```

#### Step 11: Analyze Feedback

```
PATTERNS ACROSS 5 USERS:

✅ WORKED WELL:
- All 5 submitted feedback successfully
- Times ranged 1:05 to 2:20 (all under goal of 2:00)
- All rated ease of use 8-10/10
- 4/5 proactively checked their past feedback
- 5/5 said they'd use this over email

⚠️ FRICTION POINTS:
- Category confusion: 3/5 paused, unsure which to pick
- "View Past Feedback" button: 2/5 didn't notice it initially (had to scroll)
- Character counter: 2/5 mentioned wishing they knew how much they could write

🚩 CRITICAL ISSUES:
- None! All users completed successfully

FEATURE REQUESTS:
- 4/5 wanted email notifications when status changes
- 2/5 wanted to attach screenshots
- 2/5 wanted to see other customers' feedback (community feature)
```

#### Step 12: Polish

Decision: **POLISH (minor fixes) then deploy**

Fixes:
1. Add category tooltips explaining each option
2. Make "View Past Feedback" button larger and different color
3. Add character counter to message field
4. Add text: "We'll email you when the status changes"

Implemented in 20 minutes, retested with 2 users → both gave 10/10 rating.

---

### PHASE 5: SHARE & DECIDE

#### Step 13: Deploy

Sarah deployed to Vercel (free tier):
1. Exported code from Claude
2. Created Vercel account
3. Dragged project folder
4. Got URL: `customer-feedback.vercel.app`
5. Tested live link
6. Shared with 10 beta customers

#### Step 14: Plan Next

Sarah's decision: **This will become a real product → Collaborate with engineering**

```
HANDOFF DOCUMENT:

WHY THIS MATTERS:
- Tested with 5 customers: 100% said they'd use it
- Average rating: 9.2/10
- Solves real problem (centralized feedback tracking)
- 10 customers using it in first week

PROTOTYPE VALIDATES:
- Customers want centralized feedback submission
- Status tracking is valuable (4/5 proactively checked)
- Simple UI works (no one needed help)

PRODUCTION REQUIREMENTS:

MUST HAVE:
- Admin dashboard to view all feedback, update status
- Email notifications when status changes
- Proper authentication (not just email lookup)
- Rate limiting and spam protection

SHOULD HAVE:
- Export to CSV
- Filter/search feedback
- Bulk status updates
- Integration with Slack (notify team of new feedback)

COULD HAVE:
- File attachments
- Voting on feedback
- Customer profiles

PRODUCTION CONCERNS:
- Security: Currently anyone can view any email's feedback
- Scale: Firebase free tier limits (need paid plan or migrate)
- Spam: Need better protection than current rate limit
- Data ownership: Want to self-host data

NEXT STEPS:
1. Engineering reviews prototype (this week)
2. Technical design for production version (next week)
3. Start development (2-week sprint)
4. Beta test with 20 customers (week 4)

COLLABORATION:
- Sarah: Owns product decisions, user testing
- Engineering: Owns architecture, security, code quality
- Together: Feature prioritization, technical tradeoffs
```

---

### OUTCOME

**Timeline:**
- Planning: 1 hour
- Building with Claude: 4 hours
- User testing: 2 hours
- Polish: 30 minutes
- Deploy: 20 minutes
- **Total: ~8 hours**

**Results:**
- Validated customer need
- 100% user completion rate
- High satisfaction (9.2/10 avg)
- Engineering got clear requirements
- Saved weeks of building wrong thing

**Engineering estimate for production:** 2-3 weeks

**Sarah's reflection:**
"I couldn't have coded this myself, and if I'd written a spec for engineering first, we wouldn't have learned what we learned from real users. Vibe coding let me validate the idea fast, then hand engineering a proven concept."

---

# PART 5: RESOURCES

<a id="prompt-library"></a>
## Prompt Library

Copy-paste these templates and customize for your needs.

### Starting a New Project

```
I want to build [type of tool].

CONTEXT:
Users: [specific user type and their characteristics]
Problem: [what specific problem this solves with real example]
Success: [what success looks like with measurable outcome]

TECHNICAL:
- [Device: Mobile/Desktop/Both]
- [Data: where does data come from/go to]
- [Performance: any speed requirements]

LET'S START WITH:
[Feature #1 - specific and testable]

Specifically:
- [Detail about feature]
- [Detail about feature]
- [Detail about feature]

Design: [aesthetic description]

Please build this and ask questions if unclear.
```

### Adding a Feature

```
Now let's add [feature name].

WHAT IT SHOULD DO:
- [Specific behavior 1]
- [Specific behavior 2]
- [Specific behavior 3]

SUCCESS LOOKS LIKE:
[Concrete example of working]

KEEP EXISTING [previous features] WORKING.
```

### Fixing a Bug

```
Found an issue with [feature].

STEPS TO REPRODUCE:
1. [Step 1]
2. [Step 2]
3. [Step 3]

WHAT HAPPENS:
[Actual behavior]

WHAT SHOULD HAPPEN:
[Expected behavior]

Can you fix this?
```

### Improving Design

```
The [feature] works but I want to improve [aspect].

CURRENTLY:
[How it is now]

CHANGE TO:
[How it should be]

REASON:
[Why this matters for users]
```

### Getting Unstuck

```
I'm confused by what you just built.

Please explain:
1. What does this code do?
2. Why did you build it this way?
3. What are the main parts?
4. What would break if I changed [X]?

Use simple language (I'm not a developer).
```

### Asking for Options

```
I need to implement [specific feature].

Please suggest 3 approaches:
1. Simplest (even if limited)
2. Most robust (handles edge cases)
3. Best user experience

For each, explain:
- How it works
- Pros and cons
- Implementation complexity
```

### Quality Checkpoint

```
Please review what we've built:

1. What are the main components?
2. Any potential issues or problems?
3. Is the code organized well or getting messy?
4. Any security concerns?
5. What would be hardest to change later?
```

### Optimization

```
The [feature] is slow.

SPECIFICALLY:
[What action is slow and how slow]

Please optimize for:
- Faster load time
- Better performance
- Smoother experience

Keep all functionality the same.
```

### Refactoring

```
The code is getting messy. Let's clean up.

ISSUES:
- [Issue 1]
- [Issue 2]
- [Issue 3]

Please refactor to address these while keeping all functionality working.

I'll test everything after to ensure nothing broke.
```

### Preparing for Deployment

```
I need to deploy this.

Please provide:
1. All code organized in files
2. Setup instructions
3. Recommended hosting platform for this project
4. Any environment variables or config needed
```

### Explaining Technical Concepts

```
I need you to explain [technical thing] in simple terms.

Assume I don't have a technical background.
Use analogies or real-world examples.
Focus on what I need to know, not how it works internally.
```

---

<a id="common-scenarios"></a>
## Common Scenarios

Quick guides for frequent use cases.

### Scenario 1: Building a Form

**What forms are good for:** Data collection, surveys, lead generation, feedback, contact forms

**Basic prompt:**
```
Create a form for [purpose].

Fields:
- [Field 1]: [Type] - [Required/Optional]
- [Field 2]: [Type] - [Required/Optional]
- [Field 3]: [Type] - [Required/Optional]

After submission:
- [What should happen]

Design: [Mobile-first / Desktop / Both]
Style: [Clean / Modern / Minimal / etc.]
```

**Common improvements:**
- "Add validation for email format"
- "Show error messages below each field"
- "Disable submit button while processing"
- "Add character counter on text areas"
- "Make form multi-step (wizard style)"

### Scenario 2: Building a Dashboard

**What dashboards are good for:** Data visualization, KPIs, project tracking, analytics

**Basic prompt:**
```
Create a dashboard showing [type of data].

SECTIONS:
1. [Section 1]: [What it shows]
2. [Section 2]: [What it shows]
3. [Section 3]: [What it shows]

Data source: [Where data comes from]
Update frequency: [Real-time / Daily / Manual]

Design: [Clean layout with cards / Single page / etc.]
```

**Common improvements:**
- "Add filters by date range"
- "Make charts interactive (hover shows details)"
- "Add export to CSV button"
- "Make it responsive for mobile"
- "Add dark mode toggle"

### Scenario 3: Building a Calculator/Tool

**What calculators are good for:** ROI calculators, pricing estimators, converters, cost calculators

**Basic prompt:**
```
Create a [type] calculator.

INPUTS:
- [Input 1]: [Description]
- [Input 2]: [Description]

CALCULATION:
[Explain the formula or logic]

OUTPUT:
[What result to show and how to format it]

Design: Simple and focused on the calculation
```

**Common improvements:**
- "Add input validation (no negative numbers)"
- "Show calculation breakdown"
- "Add 'Reset' button"
- "Make result copyable"
- "Add comparison with industry average"

### Scenario 4: Building a List/Table

**What lists are good for:** Task tracking, inventory, contacts, order history

**Basic prompt:**
```
Create a [type] list showing [items].

Each item displays:
- [Field 1]
- [Field 2]
- [Field 3]

Features:
- [Add new items]
- [Edit existing items]
- [Delete items]
- [Sort by X]

Design: [Clean table / Card layout / etc.]
```

**Common improvements:**
- "Add search/filter functionality"
- "Add pagination (show 20 at a time)"
- "Make columns sortable"
- "Add bulk actions (select multiple, delete)"
- "Add export to CSV"

### Scenario 5: Building a Simple Game/Quiz

**What these are good for:** Training, assessments, engagement, fun internal tools

**Basic prompt:**
```
Create a [quiz/game] about [topic].

STRUCTURE:
- [Number] questions
- [Multiple choice / True-false / etc.]
- [Scoring system]

FLOW:
1. [Start screen]
2. [Question screen]
3. [Results screen]

Design: Fun and engaging
```

**Common improvements:**
- "Add timer for each question"
- "Show correct answer after each question"
- "Add progress bar"
- "Make shareable (save results with URL)"
- "Add leaderboard"

---

<a id="troubleshooting-guide"></a>
## Troubleshooting Guide

Common problems and how to solve them.

### Problem: Claude Keeps Breaking Previous Features

**Symptoms:**
- Fix one thing, another thing breaks
- Features that worked now don't work
- Lots of back-and-forth without progress

**Solutions:**

**1. Start a new chat with full context**
```
I'm continuing work on [project].

COMPLETED FEATURES:
✅ [Feature 1]
✅ [Feature 2]
✅ [Feature 3]

CURRENT ISSUE:
[Specific problem]

Please [fix/add] this without breaking existing features.
```

**2. Ask Claude to be more careful**
```
When you make changes, please:
1. Only modify the specific feature I mentioned
2. Leave all other features untouched
3. Test that previous features still work
4. Tell me what you changed and why
```

**3. Consider starting over with clearer architecture**

Sometimes it's faster to rebuild cleanly than fix a mess.

---

### Problem: I Don't Understand What Claude Built

**Symptoms:**
- Code looks complex and confusing
- Can't explain what it does
- Afraid to ask for changes
- Don't know where to look when things break

**Solutions:**

**1. Ask for a plain-English explanation**
```
Please explain what you just built:
1. What are the main parts?
2. What does each part do?
3. How do they work together?

Use simple language (I'm not a developer).
Use analogies if helpful.
```

**2. Ask for a diagram**
```
Can you create a simple text diagram showing:
- Main components
- How data flows
- What triggers what

Keep it high-level (I don't need code details).
```

**3. Request code comments**
```
Please add comments to the code explaining:
- What each main section does
- Why you chose this approach
- What I should know if I need to change something
```

---

### Problem: Features Are Taking Too Long to Build

**Symptoms:**
- 2+ hours on a single feature
- Lots of back-and-forth without progress
- Feature getting more complex, not simpler

**Solutions:**

**1. Simplify the feature**
```
This feature is taking too long. Let's simplify.

CURRENT: [Complex version]
SIMPLIFIED: [Just the essential parts]

Build the simplified version first.
We can add complexity later if needed.
```

**2. Break it into smaller pieces**
```
Let's break [feature] into steps:

STEP 1: [Smallest possible first step]
Build just this first. I'll test it before we continue.
```

**3. Question if it's feasible**
```
This seems difficult. Before we continue:
1. Is this feature feasible for a prototype?
2. Are there simpler alternatives?
3. Should this be handled differently?
```

---

### Problem: The UI Looks Broken on Mobile

**Symptoms:**
- Text cut off
- Buttons too small
- Layout squished
- Can't scroll properly

**Solutions:**

```
The UI is broken on mobile devices.

ISSUES:
- [Specific issue 1]
- [Specific issue 2]

Please make it mobile-responsive:
- All text should be readable (min 16px)
- All buttons should be tappable (min 44px height)
- Content should fit screen without horizontal scroll
- Spacing should be comfortable for thumb tapping

I'll test on mobile after you update.
```

---

### Problem: Form Validation Isn't Working

**Symptoms:**
- Can submit empty required fields
- Email validation accepts invalid emails
- No error messages showing

**Solutions:**

```
Form validation needs fixing.

WHAT SHOULD HAPPEN:
- Required fields: Show error if empty
- Email field: Validate proper format
- [Other validations]

ERROR MESSAGES:
- Show below each field
- Use red text
- Be specific ("Email must be valid format")
- Don't allow submission until all valid

Please fix validation and show me error states.
```

---

### Problem: Data Isn't Persisting

**Symptoms:**
- Data disappears on refresh
- Submissions not saving
- Can't retrieve past data

**Solutions:**

**1. Check what storage method is being used**
```
Where is data currently being stored?
- LocalStorage?
- Firebase?
- Other?

Please explain and show me how to verify data is saving.
```

**2. Add proper error handling**
```
When data fails to save, please:
- Show user-friendly error message
- Log the error so we can debug
- Prevent data loss (keep form filled)
```

---

### Problem: It Works for Me but Not for Others

**Symptoms:**
- Prototype works on your computer
- Others get errors or blank screens
- Link doesn't work for testers

**Solutions:**

**1. Test in incognito/private mode**
- Open prototype in private browsing
- Clears all local data
- Shows what new users see

**2. Get specific error details**
```
Ask testers to:
- Take screenshot of error
- Tell you what device/browser
- Describe what they did before error
```

**3. Check browser compatibility**
```
Are there any browser-specific features in the code?
Please make it work in:
- Chrome
- Firefox  
- Safari
- Mobile browsers

Use widely-supported code only.
```

---

### Problem: Performance is Slow

**Symptoms:**
- Long load times
- Laggy interactions
- Frozen screens

**Solutions:**

```
Performance is slow, specifically [describe what's slow].

Please optimize:
- Reduce file sizes
- Load data more efficiently
- Make interactions feel instant
- Add loading indicators where needed

Goal: Everything should respond in under 2 seconds.
```

---

### Problem: Same Bug Keeps Reappearing

**Symptoms:**
- Fix a bug, it comes back
- Different features have same issue
- Fundamental problem not being addressed

**Solutions:**

```
We keep hitting the same issue: [describe pattern].

This suggests a fundamental problem.

Please:
1. Identify the root cause
2. Suggest a better approach
3. Implement a fix that prevents this issue

I'm willing to refactor if needed.
```

---

### Problem: Too Many Features, Getting Overwhelmed

**Symptoms:**
- Project scope growing
- Losing sight of core value
- Everything feels important

**Solutions:**

**1. Go back to Step 1**
- Revisit your problem statement
- What's the ONE thing this must do?
- Cut everything else

**2. Create two versions**
- Version 1: Absolute minimum (1-3 features)
- Version 2: With nice-to-haves

Build V1 first, test it, then decide on V2.

**3. Ask yourself:**
- If I could only have 3 features, which 3?
- What can I add AFTER validation?
- What's out of scope completely?

---

<a id="glossary"></a>
## Glossary

Terms you might encounter while vibe coding.

**Artifact**
Claude's term for generated code/apps that appear in a preview panel. You can interact with artifacts in real-time.

**API (Application Programming Interface)**
A way for different software to talk to each other. Example: Using Google Maps in your app.

**Backend**
The server-side part of an app that handles data, logic, and storage. You typically don't see this part.

**Bug**
An error or flaw that makes something not work as intended.

**CSS (Cascading Style Sheets)**
Code that controls how things look (colors, sizes, spacing).

**Database**
Where data is stored permanently. Examples: Firebase, PostgreSQL.

**Deploy**
Making your prototype available on the internet for others to access.

**Edge Case**
An unusual scenario that might break your app. Example: User enters 1000-character name.

**Frontend**
The user-facing part of an app—what people see and interact with.

**Framework**
Pre-built code that provides structure. Examples: React, Vue, Next.js.

**HTML**
The code that defines content structure (headings, buttons, forms, etc.).

**JavaScript (JS)**
Programming language that makes websites interactive.

**JSON**
A format for organizing data. Looks like: `{"name": "Sarah", "role": "PM"}`

**LocalStorage**
Storage in the user's browser. Data persists but only on that device.

**MVP (Minimum Viable Product)**
Simplest version that delivers core value and can be tested with real users.

**POC (Proof of Concept)**
Quick prototype to prove something is technically possible.

**React**
Popular framework for building user interfaces.

**Refactor**
Rewriting code to be cleaner/better without changing functionality.

**Responsive Design**
Design that adapts to different screen sizes (mobile, tablet, desktop).

**UI (User Interface)**
What users see and interact with.

**UX (User Experience)**
How it feels to use something (easy, confusing, fast, frustrating, etc.).

**Validation**
Checking that user input is correct (e.g., email format, required fields).

**Vercel / Netlify / Replit**
Platforms for hosting web apps (making them accessible via URL).

---

# CONCLUSION

## You're Ready to Build

You now have a complete framework for turning ideas into working prototypes using AI.

**Remember the core principles:**

1. **Think before you build** - The 30 minutes you spend in Phase 1 saves hours in Phase 3
2. **Start small** - Build the simplest version first, add complexity only if needed
3. **Test with real users** - Your opinion doesn't matter as much as your users' experience
4. **Iterate rapidly** - Embrace the back-and-forth, that's where the magic happens
5. **Know your limits** - Vibe coding is powerful for prototypes, but production needs engineering

**What makes vibe coding successful:**

✅ Clear problem definition  
✅ Specific, testable requirements  
✅ Willingness to iterate  
✅ Real user validation  
✅ Honest assessment of quality

**What kills vibe coding projects:**

❌ Vague goals  
❌ Scope creep  
❌ No user testing  
❌ Trying to build production systems  
❌ Giving up after first try

## Your Next Steps

**If this is your first vibe coding project:**
1. Choose something small (2-4 hours max)
2. Follow Phase 1 carefully (don't skip the planning!)
3. Use the Prompt Library liberally
4. Test with at least 3 users
5. Celebrate what you learn, not just what you build

**If you're experienced with vibe coding:**
1. Use this framework to level up your process
2. Focus on the validation phases (where most people skip)
3. Document your learnings for others
4. Share your templates and shortcuts

## Common Questions

**"How long until I'm good at this?"**
Your first project: 8-12 hours total  
Your third project: 4-6 hours total  
Your tenth project: 2-4 hours total

**"What if I get stuck?"**
- Reference the Troubleshooting Guide (Part 5)
- Start a fresh chat with better context
- Simplify the feature you're working on
- Ask Claude to explain what's happening

**"Should I learn to code?"**
Not necessary for vibe coding! But if you're curious, you'll naturally pick up concepts. Focus on product thinking, not syntax.

**"Can this really replace developers?"**
No. Vibe coding is for rapid prototyping and validation. Production systems need proper engineering. Think of this as a superpower for product people, not a replacement for dev teams.

**"What should I build first?"**
Build something that solves a real problem you or your team has. Internal tools are great first projects because:
- You understand the problem deeply
- You have access to users (your team)
- Stakes are lower (not customer-facing)
- You can iterate based on daily use

## Resources & Community

**Keep Learning:**
- Claude.ai documentation
- Share your projects and get feedback
- Build in public (Twitter, LinkedIn)
- Teach others (best way to solidify learning)

**Share Your Success:**
When you ship something, share it! The vibe coding community grows when we see what's possible.

## Final Thoughts

The ability to turn ideas into working prototypes in hours instead of months is a superpower. Use it wisely:

- **Validate before you invest** - Test ideas quickly before committing engineering resources
- **Empower yourself** - Don't wait for eng availability to explore ideas
- **Collaborate better** - Show don't tell when working with developers
- **Learn faster** - See working code immediately, understand patterns in real context
- **Ship more** - 10 validated experiments beat 1 perfect plan

The future of product building isn't about replacing people—it's about empowering more people to build. You're now one of them.

**Now go build something.**

---

*Version 1.0 - October 2025*  
*Questions? Feedback? Improvements? Share them with the community.*

**Credits:**
- Based on experiences of product managers using Claude Code
- Inspired by real projects built in hours, not months
- Refined through teaching dozens of non-technical builders

**License:**
This guide is meant to be shared. Use it, improve it, teach it to others.
