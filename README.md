# github-template-oss

A repository template of GitHub community health files for starting a small
open-source project (solo-friendly, trunk-based development).

## What's included

- Issue templates: Bug Report / Feature Request / Task
- Discussion templates: General / Ideas
- Pull request template (intentionally lightweight — grow it when the project does)
- `CONTRIBUTING.md`, `SECURITY.md`, `CODEOWNERS`
- CI workflow skeleton (`.github/workflows/ci.yml`, language-agnostic)

## After creating a repository from this template

A leftover placeholder is easy to miss and can go unnoticed for a long time.
Work through this checklist right after creating the repository.

### Replace placeholders

- [ ] `.github/CODEOWNERS` — replace `@OWNER` with your GitHub username
- [ ] `.github/ISSUE_TEMPLATE/config.yml` — replace `OWNER/REPO` in the Discussions URL
- [ ] `.github/CONTRIBUTING.md` — replace `OWNER/REPO` in the clone URL and fill in the `TODO` install / test commands
- [ ] `.github/workflows/ci.yml` — uncomment the setup block for your language and replace every `TODO` placeholder step with a real command (**the workflow fails on purpose until you do**)
- [ ] `.github/SECURITY.md` — review the supported versions table

### Repository settings (GitHub web UI)

- [ ] Enable **Discussions** (linked from the issue template chooser and used by the discussion templates)
- [ ] Create a **`task`** label (used by the Task issue template)
- [ ] Set up branch protection / rulesets **only after** `ci.yml` runs real commands — a placeholder or skipped required check passes silently and protects nothing

### Finally

- [ ] Replace this README with your project's own README
