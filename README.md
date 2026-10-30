# Case H: Language Placement

## What this is

Pablo Montoro Alonso in the World Languages Department at Pomfret School is the client for this case. The project will support spoken Spanish placement for incoming students.

| | |
|---|---|
| **Client** | Pablo Montoro Alonso, World Languages Department, Pomfret School |
| **Developers** | Angie Huang, Martin Ma, Ryker Reissner, Keke Li (lead developer), Luke Ryan (vice president) |
| **Club lead** | Cayden Auyang |
| **Status** | First meeting held October 21, 2026. Waiting on the department's materials. |

## The problem

Incoming students take an at-home placement test. Some use translators or AI. Mr. Montoro Alonso wants placement to happen as a spoken conversation.

## Goal

Support spoken Spanish placement while keeping the final placement decision with a Spanish teacher.

## First-meeting decisions

- Placement will use conversation only, with no written test.
- The planned tool will record each conversation and suggest a level.
- A Spanish teacher will review every recording and make the placement decision.
- Results will be kept in one place that other Spanish teachers can open.
- About 30 to 40 incoming students will use the process each year, over the summer.
- Placement covers Spanish 1 through Advanced Spanish Literature and Culture, including honors courses.

## Stack

_Not decided._ The recording method and whether AI is used are still open. Both require approval from the school's IT office because the students are under 18. Record approved decisions here and in `.cursor/rules/case-h-language-placement.mdc`.

## Student data and AI

This repository is public, and the students taking this test are under 18.

- Any AI must run through an account the school owns and approves, never a club member's personal key.
- The Gemini API's own terms rule out apps used by people under 18, so it isn't an option.
- Never record or store real students' voices or answers in this repo. Build and test with made-up answers only.
- Placement decisions stay with the World Languages Department.

## Repository layout

```
case-h-language-placement/
├── README.md              ← this file; keep it the source of truth for setup
├── .cursor/rules/         ← committed Cursor rules (workflow + project context)
├── .github/               ← pull request template, CODEOWNERS
└── .gitignore
```

Add code at the repo root (no `projects/` folder). When you add a real setup, write a "Setup from a fresh clone" section here: install, env vars (with a `.env.example`), run, build.

## Working on this repo

- Branch from `main` as `feature/<short-description>`, `fix/<short-description>`, or `chore/<short-description>` (lowercase, hyphens).
- Every change goes through a pull request with at least one approval. `main` cannot be pushed to directly.
- Never commit secrets. Put real values in a gitignored `.env`; list variable names with placeholders in `.env.example`.
- Cursor rules for this project are committed in `.cursor/rules/`. You do not need to paste anything into your IDE settings.
- The full Git walkthrough for beginners is the club's **[Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md)**.

## Definition of done (Phase 1)

To be written once the department's materials arrive.

## Contributors

- **Cayden Auyang:** club lead; set up this repository
- **Angie Huang:** developer
- **Martin Ma:** developer
- **Ryker Reissner:** developer
- **Keke Li:** lead developer
- **Luke Ryan:** vice president
