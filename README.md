# Instagram Content Agent for Claude

A Claude-compatible Skill for drafting content for the **Code With The Flow** tech-education brand. It packages the recurring content workflow as reusable instructions; it is not a standalone autonomous agent.

## What it does

The Skill creates one post draft using a weekday pillar, rotates among carousels, reels, and single-image explainers, and supplies three companion Story frames. It includes hooks, caption, challenge/engagement prompt, 15 tiered hashtags, alt text, and accuracy checks. It asks for approval of the exact draft and **does not publish or schedule Instagram content**.

## Install

### Claude Code

This repository includes the Skill at `.claude/skills/instagram-content-agent/`. Claude Code loads project Skills from that path when the repository is opened. To use it in another project, copy that Skill folder into the other repository's `.claude/skills/` directory. For personal use across projects on the same machine, copy it to `~/.claude/skills/instagram-content-agent/`.

Use [`INSTALL-PROMPT.md`](INSTALL-PROMPT.md) as the prompt when asking Claude to install from this repository. Review the Skill files before accepting any changes.

### claude.ai

Download `dist/instagram-content-agent-skill.zip`, then use **Customize → Skills** to add and enable the Skill. A GitHub link alone is not the upload package; a public repository is a source that Claude or a person can inspect, while the ZIP is the packaged Skill.

## Optional daily 10:00 AM drafts

A Skill does not run on a timer. To request a daily draft at **10:00 AM Asia/Kolkata**, create a separate Claude scheduled task on a Claude surface/account that supports scheduled tasks, then use [`prompts/claude-scheduled-task.md`](prompts/claude-scheduled-task.md) as its prompt. Review Claude's current plan and scheduled-task availability before enabling it. Keep the task draft-only; do not give it an Instagram write connector if you want manual approval before every post.

## Instagram and safety

The Skill does not include account credentials or an Instagram connection. Posting requires a separately configured, authorized Instagram tool and explicit approval of each final caption and media item. Never put passwords, tokens, or private account data in this repository.

## Files

- `.claude/skills/instagram-content-agent/SKILL.md` — Skill instructions.
- `.claude/skills/instagram-content-agent/prompts/claude-scheduled-task.md` — suggested prompt for the optional scheduled draft task.
- `prompts/claude-scheduled-task.md` — same prompt as a convenient repository-level copy.
- `dist/instagram-content-agent-skill.zip` — upload package for Claude's Skills interface.
- `INSTALL-PROMPT.md` — paste-ready prompt for asking Claude to install from the repository.

## License

No open-source license is included. Choose and add a license before granting public reuse rights.
