📘 Context-OS: Claude-Based Journaling & Memory System

This repository defines a structured journaling operating system that stores daily journals, segments them into thinking layers, recognizes patterns, remembers repetition, enables controlled habit change, and allows natural-language querying across time.

The system uses:

Claude as the reasoning and segmentation engine

GitHub as the permanent, versioned memory

Claude does not rewrite or summarize journals. It preserves original sentences and organizes them deterministically.

🎯 System Goals

Store daily natural-language journals

Preserve original wording as the source of truth

Segment journals into clear thinking layers

Track patterns over time

Enable search and question answering across all journals

Maintain traceability by date and file

🔁 System Flow
Review → Recognise → Remember → Rewire → Review

This flow is cyclical, not linear.

📂 Repository Structure
journal/
├── README.md
├── Review/
│   ├── Journaling.md
│   ├── Healthy.md
│   ├── Unhealthy.md
│   ├── Macro.md
│   ├── Micro.md
│   └── Nano.md
├── Recognise/
│   ├── Existing painway.md
│   ├── Existing pathway.md
│   ├── Possible painway.md
│   ├── Possible pathway.md
│   ├── Macro,Micro,Nano.md
│   └── High leverage outcome.md
├── Remember/
│   └── Remember.md
└── Rewire/
    └── Rewire.md
1️⃣ REVIEW — Raw Journaling & First Classification
Purpose

The Review folder stores exact journal content and performs first-level classification only.
No advice. No fixing. No rewriting.

Rules (Strict)

Journals are stored exactly as written

Sentence-level extraction only

One sentence may appear in multiple files

Macro/Micro/Nano exist only in Review

Files

Journaling.md
Primary storage for all daily journals, indexed by date. Append-only.

Healthy.md
Extracted sentences indicating effort, stability, learning, or progress.

Unhealthy.md
Extracted sentences indicating delay, stress, avoidance, or breakdown.

Macro.md
Sentences related to work, study, projects, goals, outcomes.

Micro.md
Sentences related to body, mind, health, energy, emotions, habits.

Nano.md
Sentences related to people, communication, and interactions.

2️⃣ RECOGNISE — Awareness Without Fixing
Purpose

The Recognise folder transforms classified data into clear awareness without action.

Rules

Grounded in Review content

No rewriting of journals

No motivation or solutions here

Files

Existing painway.md
Current problems already present.

Existing pathway.md
Behaviors or processes currently working (even partially).

Possible painway.md
Logical continuation of pain if nothing changes.

Possible pathway.md
Small, realistic positive direction available from the current state.

Macro,Micro,Nano.md
Maps where painways and pathways occur across life layers.

High leverage outcome.md
Single focus area that would reduce multiple painways.

3️⃣ REMEMBER — Long-Term Pattern Memory
Purpose

The Remember folder stores repetition across time, not daily events.

Rules

Added only when repetition is detected

Includes frequency

No solutions or advice

Remember.md
Conservative, stable memory of recurring patterns.

4️⃣ REWIRE — Controlled Habit Change (Optional)
Purpose

The Rewire folder designs small, controlled behavior changes after understanding is complete.

Rules

Activated only when requested or clearly needed

One change at a time

Actions must be minimal and concrete

Rewire.md
Contains coach reasoning, client constraints, and small action steps.

🔍 Query & Retrieval

The system supports questions like:

“When did I feel stressed?”

“When did I work on a specific task?”

“How often did this repeat?”

Retrieval Rules

Search Review → Recognise → Remember

Match by meaning

Return date, exact sentence, and source file

Never rewrite historical content

If no match exists, respond: “Not found in stored journals.”

🤖 Claude Responsibilities

Claude must:

Preserve original journal sentences

Follow folder definitions strictly

Maintain date indexing

Commit updates safely to GitHub

Claude must not:

Summarize or improve language

Invent content

Mix folder responsibilities

🗃️ GitHub as Memory

GitHub acts as:

Permanent storage

Version history

Audit trail

External brain

Each daily journal and its processing results in a single, clear commit.

🏁 Final Principle

Journaling is treated as data, not content.
Understanding comes before change.
Memory grows over time, without losing truth.
