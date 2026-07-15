# Week 2 – Prompt Ladder

## Goal

Improve a prompt for writing a portfolio case study by changing only one prompt engineering layer at a time.

---

# Baseline Prompt

> Write a case study for my FlyRank internship.

### Output (excerpt)

"The FlyRank internship helped me learn machine learning and data analysis. I worked with search data and gained valuable experience."

### Notes

- **What changed?**
  - Baseline prompt with no context.

- **What improved?**
  - Nothing. The output was generic.

- **What still failed?**
  - It could describe almost anyone's internship.

- **Next change**
  - Clearly define the goal.

---

# Version 1 — Clear Goal

### Added Layer

Clear Goal

### Prompt

> Write a portfolio case study that explains my FlyRank Machine Learning Internship and demonstrates my software engineering skills.

### Output (excerpt)

"The internship focused on applying machine learning concepts to real search data while building repeatable analysis workflows."

### Notes

- **What changed?**
  - Added a clear goal.

- **What improved?**
  - The response became focused on a portfolio case study instead of a general summary.

- **What still failed?**
  - It still lacked details about my actual work.

- **Next change**
  - Add project context.

---

# Version 2 — Context

### Added Layer

Real Context

### Prompt

> Write a portfolio case study. I am a final-year Computer Engineering student specializing in AI & Data Science. During the FlyRank internship I explored anonymized search data, framed a machine learning problem, performed exploratory data analysis, and built the foundation for a content opportunity scoring workflow.

### Output (excerpt)

"The project focused on understanding search performance data before selecting machine learning techniques."

### Notes

- **What changed?**
  - Added real project context.

- **What improved?**
  - The output reflected my actual work instead of making generic assumptions.

- **What still failed?**
  - The writing was still too broad.

- **Next change**
  - Specify the audience.

---

# Version 3 — Audience

### Added Layer

Audience

### Prompt

> Write this case study for a Software Engineering Hiring Manager evaluating internship candidates.

### Output (excerpt)

"The project demonstrates an evidence-based approach to framing machine learning problems and building repeatable workflows."

### Notes

- **What changed?**
  - Added the audience.

- **What improved?**
  - The output emphasized technical decisions rather than explaining basic concepts.

- **What still failed?**
  - The structure varied from run to run.

- **Next change**
  - Specify an output format.

---

# Version 4 — Output Format

### Added Layer

Output Format

### Prompt

> Write the case study using these sections:
>
> - Problem
> - What I Did
> - Outcome
> - Lessons Learned

### Output (excerpt)

```
Problem

...

What I Did

...

Outcome

...
```

### Notes

- **What changed?**
  - Added a required structure.

- **What improved?**
  - The response became much easier to read and reuse in a portfolio.

- **What still failed?**
  - Some wording sounded like generic AI writing.

- **Next change**
  - Add quality constraints.

---

# Version 5 — Constraints

### Added Layer

Constraints

### Prompt

> Use only information I provide.
> Do not exaggerate achievements.
> Avoid buzzwords.
> Write in a direct, practical tone.
> Do not invent metrics or results.

### Output (excerpt)

"The internship helped me understand how to frame business problems as machine learning tasks using real search data while carefully avoiding unsupported claims."

### Notes

- **What changed?**
  - Added writing constraints.

- **What improved?**
  - The response sounded much more like my own writing and avoided unsupported claims.

- **What still failed?**
  - It could still benefit from examples from my notebooks.

- **Next change**
  - Add notebook excerpts as supporting evidence.

---

# Final Reusable Prompt

You are helping me write a portfolio case study.

Audience:
Software Engineering Hiring Manager.

Goal:
Create a portfolio case study that demonstrates my engineering thinking.

Context:
I am a final-year Computer Engineering student specializing in AI & Data Science. During my FlyRank Machine Learning Internship, I explored anonymized search data, framed machine learning problems, performed exploratory data analysis, and developed a repeatable workflow for content opportunity scoring.

Output format:

- Problem
- What I Did
- Outcome
- Lessons Learned

Constraints:

- Use only information I provide.
- Do not invent achievements.
- Do not invent metrics.
- Avoid buzzwords.
- Use a direct, practical tone.
- Keep the writing suitable for a professional portfolio.
