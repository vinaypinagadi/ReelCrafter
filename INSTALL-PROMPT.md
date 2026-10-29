# Prompt to give Claude

Replace `OWNER/REPOSITORY` with the GitHub repository path, then paste this into Claude Code or Claude with access to the repository:

> Please inspect `https://github.com/OWNER/REPOSITORY` and install its `instagram-content-agent` as a Claude Skill. Read the README and the Skill files first. If you are in Claude Code, install the Skill at the scope I choose: project (`.claude/skills/instagram-content-agent/`) or personal (`~/.claude/skills/instagram-content-agent/`). Copy the complete Skill folder, including its `prompts/` file, then verify the `SKILL.md` frontmatter and report the path installed. Do not run unrelated scripts, create a scheduled task, connect Instagram, or publish anything. If you are in claude.ai chat rather than Claude Code, tell me to upload `dist/instagram-content-agent-skill.zip` from this repo through Customize → Skills; do not claim it was installed just from the link. Ask before overwriting an existing skill or changing its scope.

If Claude cannot access the GitHub repository, download the repo ZIP or the separate Skill ZIP and upload it to Claude instead.
