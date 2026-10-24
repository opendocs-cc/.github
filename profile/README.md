# OpenDocs

**Publish Markdown from your AI agent: a link your team can read, or a branded PDF or Word file.**

Claude Code, Codex, Cursor and every other coding agent write Markdown all day: specs, runbooks, reports, release notes. OpenDocs gives those files somewhere to go. One command turns a `.md` file into a permanent link, or into a PDF or DOCX in your workspace's colors, font and logo.

## Get started

Paste this into your agent:

```text
I'd like you to set up OpenDocs: Markdown publishing for agents (shareable links, plus PDF and DOCX export).

Install as a skill if I have npm: npx skills add https://opendocs.cc --skill opendocs -g -y

If not, do this instead: curl -fsSL https://opendocs.cc/install.sh | bash

The npx installer may end with "PromptScript does not support global skill installation". That's a known installer bug that only affects PromptScript; the skill is still installed.

Then sign me up (it's free): ask for my email, run opendocs login --email <my email>, and I'll paste the 6-digit code it sends me.

After that, read the agent quickstart at https://docs.opendocs.cc/getting-started/agent-quickstart.md and ask me what I'd like to publish
```

Or use the CLI yourself:

```bash
npm install -g @opendocs.cc/cli
opendocs login --email you@example.com    # sign up free: emails you a 6-digit code
opendocs publish notes.md                  # prints the link
opendocs export notes -f pdf               # branded PDF
```

Free for up to 50 documents, no credit card.

## What you get

- **Links that last.** Publishing the same file again updates the same URL, and every version is kept.
- **Private by default.** Documents are visible to your workspace until you make one public.
- **Projects.** Group documents by client, product or team; your agent files each one in the right place.
- **On-brand exports.** PDF and Word files in your colors, font and logo, from nine tested presets or your own (Pro).
- **Built for agents.** `--json` output, stable error codes, and a skill file that teaches the agent the whole workflow.

## In this organization

| Repository | What it is | License |
| --- | --- | --- |
| [opendocs-cli](https://github.com/opendocs-cc/opendocs-cli) | The `opendocs` CLI and the agent skill (`SKILL.md`) | MIT |

The hosted service (web app, API and document converter) is closed source.

## Links

[Website](https://opendocs.cc) · [Docs](https://docs.opendocs.cc) · [Pricing](https://opendocs.cc/pricing) · [X](https://x.com/opendocshq)

Found a bug? Open an issue on [opendocs-cli](https://github.com/opendocs-cc/opendocs-cli/issues). Security reports go to hello@opendocs.cc.
