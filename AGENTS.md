# How to work in this worktree

Written 2026-09-18 because agents working in the Horizon trees stopped at every
step to ask permission, ask which option to take, and wait for the owner to run
dry runs. That is the behaviour to fix.

## ⚠ This repository is PUBLIC

`socialclassfarewell/gapcheck-site` is world-readable — verified 2026-09-18, and
it is the only public repo in this estate. Everything else is private, so the
habits that are safe elsewhere are not safe here.

- Anything committed here is published. Treat every commit as a press release.
- Never commit provider names, participant details, worker names, email
  addresses, outreach records, credentials, API keys, internal hostnames or
  tailnet addresses. Not in code, not in comments, not in test fixtures, not in
  commit messages.
- Pricing, positioning and roadmap claims are owner-gated. Do not publish a
  number or a promise the owner has not signed off.
- If you are unsure whether something is publishable, it is not. That is the one
  case where stopping to ask beats guessing.

## Do not park work on the owner

- Run the dry run, the smoke test and the build **yourself**. Carry on unless it
  fails. Report after, not before.
- Do not stop to ask which option the owner wants. Pick the sensible default,
  say in one line which you picked and why, and keep going. They will redirect
  you if it is wrong, and that costs them far less than being asked.
- Asking is the exception, not the checkpoint. If you are about to ask a
  question you could answer by reading the repo or running a command, run it.
- Batch anything that genuinely needs the owner into one message at the end,
  rather than blocking on each one as you hit it.

## The gates that still stop you

These are not negotiable, and nothing above loosens them:

- Merges to `main` are owner-gated. Feature-branch commits of verified work are
  pre-authorised; merging is not. On a public repo, a merge is a publication.
- Never `git add -A` here. Targeted single-file commits only — a broad add is
  how private material reaches a public repo by accident.
- Never switch branches in a worktree another live session is using.
- Anything touching personal data stays local and is never sent to a cloud
  agent, and never lands in this repo at all.
- Billing, quota and account settings are owner-only. Report; never change them.

## Verify before you claim

Check the artifact, never the exit code. A command can exit 0 having done
nothing, a test can pass vacuously, and an agent can report a test count it
never ran. If you say something is done, name the evidence you checked.

## Reply style

Short. Plain words. No headers, no bold in chat replies. Answer what was asked.
Commands go in their own block, ready to paste.
