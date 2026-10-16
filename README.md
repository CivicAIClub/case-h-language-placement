# Case H: Language Placement

## What this is

Pablo Montoro Alonso in the World Languages Department at Pomfret School is the client for this case. He wants a more solid placement test for incoming students, and he imagines an on-screen character students could interact with. The first meeting is being scheduled, so there is no code yet. Status: first meeting being scheduled.

| | |
|---|---|
| **Client** | Pablo Montoro Alonso, World Languages Department, Pomfret School |
| **Developers** | _Not yet assigned_ |
| **Club lead** | Cayden Auyang |
| **Status** | 🔵 First meeting being scheduled |

## The problem

Pablo Montoro Alonso wants a more solid placement test for incoming World Languages students, and he imagines an on-screen character students could interact with.

How placement works today, and what the test needs to measure: _To be written in the first meeting._

## Goal

_To be written in the first meeting._ Likely direction (not a commitment): a test that adapts to each student first. The character comes later, if the school approves the AI part.

## Stack

_Not decided._ Decide in the first meeting and record the decision here and in `.cursor/rules/case-h-language-placement.mdc`.

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

_To be written in the first meeting._

## Contributors

- **Cayden Auyang:** club lead; set up this repository
- Developers: not yet assigned
