# Week 2 – Prompt Engineering Iteration Log

## Target Task

Write a portfolio case study for my FlyRank Machine Learning Internship.

---

# Version 0 – Naive Prompt

## Prompt

Write a case study for my FlyRank internship.

## Output (Excerpt)

"The FlyRank internship helped me learn machine learning and data analysis. I worked with search data and gained valuable experience."

## Reflection

- **Technique:** None (Baseline)
- **Observed Difference:** The response was very generic and could apply to almost any internship.
- **What Still Failed:** It lacked technical depth and did not reflect my actual work.
- **Next Technique:** Role Assignment.

---

# Version 1 – Role Assignment

## Technique

Role Assignment

## Prompt

You are a Software Engineering Hiring Manager reviewing internship portfolios. Write a case study for my FlyRank Machine Learning Internship.

## Output (Excerpt)

"The internship demonstrates practical experience with machine learning workflows and search data analysis."

## Reflection

- **Observed Difference:** The response focused more on engineering skills than a general summary.
- **What Still Failed:** It still assumed details instead of using my real experience.
- **Next Technique:** Context and Motivation.

---

# Version 2 – Context and Motivation

## Technique

Context and Motivation

## Prompt

You are a Software Engineering Hiring Manager reviewing internship portfolios.

I am a final-year Computer Engineering student specializing in AI & Data Science.

During the FlyRank internship I framed a machine learning problem, explored anonymized search data, and built the foundation for a content opportunity scoring workflow.

Write a portfolio case study.

## Output (Excerpt)

"The project focused on framing business problems as machine learning tasks before selecting models."

## Reflection

- **Observed Difference:** The response became much closer to my actual experience.
- **What Still Failed:** The structure was inconsistent.
- **Next Technique:** Few-shot Examples.

---

# Version 3 – Few-shot Examples

## Technique

Few-shot Examples

## Prompt

Write using this style:

Problem
What I Did
Outcome

Now write my FlyRank case study using the same format.

## Output (Excerpt)

Problem

...

What I Did

...

Outcome

...

## Reflection

- **Observed Difference:** The output became much easier to read and matched the format I wanted.
- **What Still Failed:** Some wording still sounded like generic AI writing.
- **Next Technique:** Output Structure.

---

# Version 4 – Output Structure

## Technique

Output Structure

## Prompt

Produce exactly these headings:

- Problem
- What I Did
- Technical Decisions
- Outcome
- Lessons Learned

## Output (Excerpt)

Problem

...

Technical Decisions

...

Lessons Learned

...

## Reflection

- **Observed Difference:** The response became more organized and suitable for a portfolio.
- **What Still Failed:** Some claims were broader than my actual experience.
- **Next Technique:** Step Decomposition.

---

# Version 5 – Step Decomposition

## Technique

Step Decomposition

## Prompt

First identify the project problem.

Then identify my technical decisions.

Then summarize the outcome.

Finally write the case study using only information I provide.

Do not invent achievements.

## Output (Excerpt)

"The internship demonstrates how machine learning can support decision-making using anonymized search data while avoiding unsupported conclusions."

## Reflection

- **Observed Difference:** The response became more accurate and reflected my real work.
- **What Still Failed:** It still required manual editing to fully match my writing style.

---

# Cross-Model Comparison

## Claude

Strengths

- Better reasoning
- More natural interview questions
- Better at uncovering technical decisions

Weaknesses

- Sometimes assumes missing details if not constrained.

---

## ChatGPT

Strengths

- Better organization
- Clearer formatting
- Easier to produce reusable documentation

Weaknesses

- More likely to sound polished but generic without sufficient context.

---

# Final Reusable Prompt

You are helping write a software engineering portfolio case study.

Audience:
Software Engineering Hiring Manager.

Goal:
Demonstrate practical engineering thinking rather than listing technologies.

Context:
[Insert project details.]

Follow this process:

1. Identify the problem.
2. Explain the technical decisions.
3. Describe the implementation.
4. Summarize the outcome.
5. Highlight lessons learned.

Output Format

- Problem
- What I Did
- Technical Decisions
- Outcome
- Lessons Learned

Constraints

- Use only the information provided.
- Do not invent metrics.
- Avoid buzzwords.
- Write in a direct and practical tone.
