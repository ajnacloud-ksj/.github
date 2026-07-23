# How we work — the whole process on one page

```
ticket → triage → PR against ticket → merge (dev auto-deploys) → promote (prod releases)
```

## 1. Everything starts as a ticket
**New issue → pick a type** (Feature / Bug / Tech debt / Chore). The form asks the right
questions and applies the type label itself.

## 2. Triage — 10 min a week, per team
Open your board's **Triage view**: give each new ticket a milestone (`vNext`) and an assignee.
Empty view = done.

## 3. Work = a PR against the ticket
- Title: `feat(scope): summary` (Conventional Commits) — **CI rejects otherwise**
- One type label: `feature` / `bug` / `tech-debt` / `docs` / `chore` — **CI rejects otherwise**
- `Closes #123` in the description — closes the ticket on merge and rolls up the epic

## 4. Merge — everything after is automatic
Merge to `develop`: dev deploys, the ticket closes, the board card moves to Done.
Nobody updates boards or writes notes by hand, ever.

## 5. Release — the monthly train; you only merge
On the 1st of each month the release train automatically opens a `develop → main` promotion PR
for every app with changes — version computed, changelog in the body. **Merging that PR (merge
commit, never squash) is the release**: prod deploys, the tag is read from the PR title,
categorised notes generate from PR labels, the milestone closes itself. Emergency/off-cycle:
Actions → Cut release in ajna-app-infra, any day.

---
Why it's built this way, and the automation behind it:
[`ajna-app-infra/docs/project-management-design.md`](https://github.com/ajnacloud-ksj/ajna-app-infra/blob/main/docs/project-management-design.md)
