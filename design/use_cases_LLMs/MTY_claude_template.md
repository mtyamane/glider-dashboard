# Use Case Template (from User Stories)

This template turns a file of user stories into fully dressed use cases. Each story lists four things: **who** the user is, **what they want to do** with the tool, **what they need and want** from the tool, and **their skill level**.

The use case is built around **what they want to do** (the goal). The other three parts add detail:

| Story element | Where it goes in the use case |
|---|---|
| **What they want to do** (main focus) | Use case name, goal, main success scenario |
| Who the user is | Primary actor, stakeholders |
| Needs and desires | Stakeholder interests, success guarantee, non-functional notes |
| Skill level | Actor profile, alternate flows (e.g., a guided path for novices, shortcuts for experts) |

---

## Step 1: Group the stories by goal

Before writing use cases, sort the stories by what the user wants to do. Stories with the same or very similar goal become **one** use case, even if the users are different.

| Group ID | Shared goal (verb + object) | Story IDs | Users involved | Skill levels covered |
|---|---|---|---|---|
| G-01 | *e.g., Export a report* | US-03, US-11, US-17 | *Analyst, Manager* | *Novice, Expert* |
| G-02 | | | | |
| G-03 | | | | |

**Grouping rules**
- Name each goal as **verb + object** ("Schedule a meeting," not "Scheduling").
- Merge stories when the user would finish the same task and get the same result.
- Split a group when the end result or trigger is clearly different.
- If one user's story holds two goals, put it in both groups.

---

## Step 2: Write one use case per group

Copy the block below once for each group.

```markdown
## UC-[##]: [Verb + Object — the goal]

**Source stories:** [US-##, US-##, ...]
**Group:** [G-##]
**Scope:** [System or tool name]
**Level:** [User goal | Subfunction | Summary]

### Goal
[One sentence: what the user wants to do with the tool and why, drawn from the
"what do they want to do" part of the stories.]

### Primary Actor
[Main user type]

### Actor Profiles
| Actor | Skill level | Relevant needs/desires |
|---|---|---|
| [User type] | [Novice / Intermediate / Expert] | [From story] |
| [User type] | [ ] | [ ] |

### Stakeholders and Interests
- **[Actor]:** [What they need from this use case]
- **[Other stakeholder, e.g., admin, organization]:** [Their interest]

### Trigger
[The event that starts the use case.]

### Preconditions
- [What must be true before the use case starts]

### Main Success Scenario
1. [Actor] [action].
2. System [response].
3. [Actor] [action].
4. System [response].
5. ...
6. [Final step: goal achieved.]

### Alternate Flows
*Includes different paths based on skill level.*

**[Step #]a. [Condition, e.g., User is a novice]**
1. System [offers guidance / step-by-step help].
2. Resume at step [#].

**[Step #]b. [Condition, e.g., User is an expert]**
1. [Actor] [uses shortcut / advanced option].
2. Resume at step [#].

**[Step #]c. [Other variation]**
1. ...

### Exceptions
**[Step #]x. [Error or failure condition]**
1. System [error handling].
2. [Use case ends / resumes at step #].

### Success Guarantee (Postconditions)
- [What is true when the goal is met; must satisfy the needs listed above]

### Minimal Guarantee
- [What is still true if the use case fails, e.g., no data lost]

### Non-Functional Requirements
*From the needs and desires that are about quality rather than function.*
- **Usability:** [ ]
- **Performance:** [ ]
- **Accessibility:** [ ]
- **Other:** [ ]

### Open Questions
- [Conflicts between stories, unclear details, assumptions made]
```

---

## Step 3: Check the mapping

Use this table to confirm every story ended up somewhere.

| Story ID | Use case(s) | Fully covered? | Notes |
|---|---|---|---|
| US-01 | UC-01 | Yes / Partly / No | |
| US-02 | | | |

---

## Worked example

**Source stories**

> **US-03** — *Who:* Small-business owner. *Wants to do:* Send invoices to clients. *Needs:* Fast, looks professional. *Skill:* Novice.
>
> **US-11** — *Who:* Freelance accountant. *Wants to do:* Send invoices for several clients at once. *Needs:* Batch sending, custom templates. *Skill:* Expert.

## UC-01: Send an Invoice

**Source stories:** US-03, US-11
**Group:** G-01
**Scope:** Billing tool
**Level:** User goal

### Goal
The user creates an invoice and sends it to one or more clients so they get paid.

### Primary Actor
Invoice sender

### Actor Profiles
| Actor | Skill level | Relevant needs/desires |
|---|---|---|
| Small-business owner | Novice | Fast, professional look |
| Freelance accountant | Expert | Batch sending, custom templates |

### Stakeholders and Interests
- **Sender:** Invoice is correct, looks professional, and sends quickly.
- **Client:** Gets a clear invoice with correct amounts and payment details.

### Trigger
The sender chooses "New Invoice."

### Preconditions
- The sender is logged in.
- At least one client is saved.

### Main Success Scenario
1. Sender chooses "New Invoice."
2. System shows the invoice form with the default template.
3. Sender picks a client and adds line items.
4. System calculates totals and shows a preview.
5. Sender confirms and selects "Send."
6. System emails the invoice to the client and marks it "Sent."

### Alternate Flows
**2a. Sender is a novice**
1. System shows a short guided walkthrough of the form.
2. Resume at step 3.

**3a. Sender is an expert sending to several clients**
1. Sender selects multiple clients and a saved custom template.
2. System creates one invoice per client.
3. Resume at step 4.

### Exceptions
**6x. Email fails to send**
1. System saves the invoice as "Draft" and shows the error.
2. Use case ends.

### Success Guarantee (Postconditions)
- Each selected client has received an invoice, and each invoice is marked "Sent."

### Minimal Guarantee
- No invoice data is lost; unsent invoices are saved as drafts.

### Non-Functional Requirements
- **Usability:** A novice can send a first invoice in under 3 minutes.
- **Other:** Invoices use a professional layout by default.

### Open Questions
- Should batch sending be limited to a maximum number of clients?
