# Review – Raw Data Processing

Review is the ONLY place where:
- Raw journaling is written
- Macro / Micro / Nano classification happens

Claude must treat Review as SOURCE DATA.
Nothing here should be rewritten.

---

## Files and Meaning

### Journaling.md
Contains raw user-written sentences.
Claude must store text exactly as provided.

### Healthy.md
Extract sentences that show forward movement.
Do not modify wording.

### Unhealthy.md
Extract sentences that show avoidance, delay, or breakdown.
Do not modify wording.

### Macro.md
Extract sentences related to work, study, or outcomes.

### Micro.md
Extract sentences related to body, mind, or energy.

### Nano.md
Extract sentences related to people or communication.

## Purpose of Review

Review is the data ingestion and classification layer.
It answers:
What happened?
What worked?
What didn’t?
At what level did it occur?
