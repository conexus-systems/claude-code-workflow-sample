# Claude Code workflow: free sample

Three small files from a longer spec-driven workflow for Claude Code. They work on their own.

## What is here
- `CLAUDE.md`: a project guide template. Fill in the three commands. The "check everything" command defines what "done" means.
- `.claude/skills/verify-before-done/SKILL.md`: before declaring a task finished, Claude runs your check command and reports what passed, failed and was not checked.
- `.claude/agents/reviewer.md`: a read-only subagent that reviews a diff and ranks findings by severity, each with a concrete failing input.

## Use it
1. Copy the three files into your repo, keeping the paths above.
2. Edit `CLAUDE.md`: replace every `<...>`.
3. In Claude Code, finish a task, then ask: "Use the reviewer agent on my diff."

## Not included
This is not a promise of faster delivery or fewer bugs. Agents make mistakes, so check their output. Not affiliated with Anthropic.

## The rest
The full pack adds five more subagents (spec-writer, test-first-implementer, security-reviewer, refactorer, release-notes), four more skills (spec-to-tasks, small-commits, pr-description, postmortem), a `SPEC.md` template, and a hook plus permission rules that keep Claude from reading secret files. US$ 12: https://tiagoantoniazi.gumroad.com/l/tleixv

## License
MIT. See `LICENSE`.
