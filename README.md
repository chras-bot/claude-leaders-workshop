# Claude Leaders Workshop

Moving Faster Together, New York.

This is a shared workspace for the Claude leaders user group in New York. Each person adds one small folder. The folder holds a short rules file and a few checks for one task their team repeats. Near the end of the session, Clayton uses Claude to read the open pull requests and shows a summary to the room.

The exercise has two parts.

## Part 1: pick the work and write the rules

Use any Claude: the app, the website, your phone, or Cowork. No GitHub needed. Paste this:

```
Interview me, one question at a time, about 3 tasks my team repeats.
Help me pick the one to hand to Claude first.
Then write rules for it in 15 lines or fewer: the goal, the inputs,
numbered rules, the output format, and when to stop and ask.
Leave out names, clients, and links.
```

Keep the rules Claude writes. You use them in part 2.

## Part 2: check it and share it

Open Claude Code or Cowork and paste this line, then paste your rules from part 1:

```
Clone github.com/praecipio-community/claude-leaders-workshop, then follow its CLAUDE.md.
```

No Claude Code or Cowork? Paste this in any Claude instead, then paste your rules:

```
Read https://raw.githubusercontent.com/praecipio-community/claude-leaders-workshop/main/CLAUDE.md and follow it. I will share through github.com in my browser.
```

Claude adds 3 checks and 1 trap, removes anything private, and shows you both files. When you say yes, it commits on a branch and opens a pull request.

Claude asks you for a short alias for your folder. Do not use your name, your employer, a client, or your GitHub username. Your GitHub username still shows on the pull request, so use a personal account, not a work one.

Rather not post? Tell Claude to stop before it pushes. Your files stay on your laptop.

If your Claude cannot push, it walks you through github.com instead. No GitHub account? Tell Claude. It walks you through a free one in about 3 minutes. No laptop? Pair with a neighbor.

## After the session

The two files are yours. Paste rules.md into your team's CLAUDE.md or project instructions. Run the checks against the next three outputs. Add a check each time the agent gets something wrong.

## About the CLAUDE.md files

This repository contains CLAUDE.md files. They are instructions for AI agents. When you open this folder with Claude, it reads them and follows them. Agents that are not Claude read `AGENTS.md`, which points to the same rules. Read them first. They are short.

- [CLAUDE.md](CLAUDE.md): the exercise, why to sanitize, and how to share the work.
- [submissions/CLAUDE.md](submissions/CLAUDE.md): folder rules and the check before commit.

## What not to share

This repository is public. Everything you commit can be read by anyone.

- No names of people, clients, or employers.
- No emails, phone numbers, URLs, or social handles.
- No internal system names, ticket keys, or project codes.
- No money figures tied to a company.
- No passwords, API keys, tokens, or files from work.

Use roles and generic terms instead. Write "the service desk lead" and "the ticketing tool," not a person or a product instance. Claude checks for these before it commits. You make the final call.

## What is here

| Path | What it is |
|------|------------|
| `CLAUDE.md` | Instructions for the agent |
| `AGENTS.md` | Points agents that are not Claude to the same instructions |
| `CONTRIBUTING.md` | The same rules, written for people |
| `templates/` | Fill-in templates for the two files |
| `examples/` | Three worked examples: a Jira admin hygiene report, mapping two Jira estates, and a monthly operating review |
| `submissions/<alias>/` | Where your files go, under a short alias you pick |
| `.github/pull_request_template.md` | The pull request checklist |
| `.github/CODEOWNERS` | Requests a review from Clayton Chancey, the workshop host, on every pull request |

## License

MIT. See [LICENSE](LICENSE).
