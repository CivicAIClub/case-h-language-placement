# Case H agent guide

## Purpose

This project supports spoken Spanish placement for incoming Pomfret students for Pablo Montoro Alonso in the World Languages Department. A Spanish teacher keeps the final placement decision after reviewing the recorded conversation.

## Project rules and open decisions

- Read `README.md` and `.cursor/rules/case-h-language-placement.mdc` before working here.
- Recorded status: the first meeting was held October 21, 2026, and the project is waiting for the department's materials.
- Use conversation only, with no written test. The planned tool records each conversation and suggests a level. A Spanish teacher reviews every recording and makes the placement decision; decisions stay with the department.
- Keep results in one place other Spanish teachers can open. Plan for about 30 to 40 incoming students each summer, covering Spanish 1 through Advanced Spanish Literature and Culture, including honors courses.
- The stack is not decided. The recording method and whether to use AI are open. Both need school IT approval because students are under 18. Record approved decisions in the README and project rule.
- Any AI must use an account the school owns and approves, never a club member's personal key. The project rule excludes Gemini API because its terms rule out apps used by people under 18.
- This repo is public. Never record or store real students' voices or answers here. Build and test with made-up answers only.
- Add `.env.example` as soon as a credential or ID is needed. Never commit API keys, tokens or `.env` files. Real values belong in a gitignored `.env`; every environment variable needs a placeholder in `.env.example`. If a developer pastes a real credential into a file, stop and tell them.
- Add code at the repo root, with no `projects/` folder. The README has no setup/run commands yet. When setup exists, add a "Setup from a fresh clone" section covering install, environment variables with `.env.example`, run and build.
- Write the Phase 1 definition of done once the department's materials arrive.

## Working with student developers

- Prefer clear code over clever code. If you generate code the developer cannot explain, say so and explain what it does in plain English.
- Paths in this guide are relative to this standalone repository. Each club project has its own repo. Do not edit the archived `Civic-AI-Github-Repository` monorepo.
- For Git, branches, pull requests or merge conflicts, use the Developer Onboarding Guide linked below instead of making up a workflow.
- Check with Cayden before changing `.github/` or `.cursor/rules/`. Keep the README accurate when setup changes.

## Git and pull requests

- Never push directly to `main`. Work on a branch and open a pull request. Merging needs at least one approving review.
- Name branches `feature/<short-description>`, `fix/<short-description>` or `chore/<short-description>`, using lowercase letters and hyphens, with no spaces.
- Make small, frequent commits with plain-English messages.
- Use `.github/pull_request_template.md` for pull requests.
- Never add `Co-authored-by`, `Generated with`, `Made-with`, `Claude-Session` or any other AI attribution line to a commit message or pull request description. When squash merging, delete any such lines GitHub adds to the merge message.

## Beginner quick start

Full guide: https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md

1. First time: check Git with `git --version`, set your Git name and GitHub email, accept the club invite, and sign in with GitHub Desktop or `gh auth login`. Clone only your project's repo, open its folder, and read its README setup steps.
2. Start each work session from the latest main, then make a branch:

```sh
git checkout main
git pull origin main
git checkout -b feature/short-description
# Make and check your changes before continuing.
git status
git add .
git commit -m "Describe your change"
git push --set-upstream origin feature/short-description
```

Use `feature/`, `fix/`, or `chore/` as appropriate, with lowercase names and hyphens. Commit small working pieces; do not edit or push main directly.
3. Open a PR on GitHub, fill in the template, and get someone else's approval and passing checks where CI exists. Push review fixes to the same branch. After it is merged, pull main again before starting another branch.
4. If stuck, ask in the case chat, then Keke, then Luke or Cayden. Ask before doing anything drastic.

## Sources

- `README.md`
- `.cursor/rules/civic-ai-workflow.mdc`
- `.cursor/rules/commit-messages.mdc`
- `.cursor/rules/case-h-language-placement.mdc`
- [Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md)
