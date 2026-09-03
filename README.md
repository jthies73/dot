# dot

Dotfiles, managed from one place and symlinked wherever they're needed.

Currently:

- `.AGENTS.md` covers git worktree usage, branch naming, commit style, and how to edit or recommend skills.
- `.CLAUDE.md` just imports `.AGENTS.md` via `@.AGENTS.md`. Claude Code reads `CLAUDE.md` by default, so this is how it picks up the rules.

More configs (shell, git, editor, etc.) belong here as they come up.

## Use in another repo or in $HOME

Symlink the file where it's expected:

```
ln -s /path/to/dot/.AGENTS.md .AGENTS.md
ln -s /path/to/dot/.CLAUDE.md .CLAUDE.md
```

Edit the file here, and every linked location picks up the change.
