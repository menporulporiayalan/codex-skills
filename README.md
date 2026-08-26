# Dayzy skill

Use Dayzy cards and boards from Codex or Claude Code.

## Before you start

You need access to this private GitHub repository and a Dayzy API token. Keep the token out of Git and chat.

```sh
export DAYZY_TOKEN='your-token'
```

This lasts for the current terminal session. Store it in your preferred secrets manager or shell configuration if needed.

## Codex

In Codex, ask:

```text
$skill-installer Install the Dayzy skill from GitHub repository menporulporiayalan/codex-skills at path dayzy.
```

Restart Codex if the skill does not appear. Invoke it explicitly with `$dayzy`, or ask a Dayzy-related question.

## Claude Code

Clone the private repository, then copy the skill into Claude Code's personal skills directory:

```sh
gh repo clone menporulporiayalan/codex-skills /tmp/codex-skills
mkdir -p ~/.claude/skills
cp -R /tmp/codex-skills/dayzy ~/.claude/skills/dayzy
```

Restart Claude Code if `~/.claude/skills` did not already exist. Invoke the skill with `/dayzy`, or ask Claude a Dayzy-related question.
