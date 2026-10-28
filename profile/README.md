# OpenDocs

**Publish Markdown from your AI agent: a link your team can read, or a branded PDF or Word file.**

Claude Code, Codex, Cursor and every other coding agent write Markdown all day: specs, runbooks, reports, release notes. OpenDocs gives those files somewhere to go. One command turns a `.md` file into a permanent link, or into a PDF or DOCX in your workspace's colors, font and logo.

OpenDocs is open source under the MIT license, and you can [host it yourself](https://github.com/opendocs-cc/opendocs/blob/main/SELF_HOSTING.md).

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
| [opendocs](https://github.com/opendocs-cc/opendocs) | The web app, API and MCP server: everything behind opendocs.cc, ready to self-host | MIT |
| [doc-converter](https://github.com/opendocs-cc/doc-converter) | Markdown to branded PDF and Word, used for exports | MIT |
| [opendocs-cli](https://github.com/opendocs-cc/opendocs-cli) | The `opendocs` CLI and the agent skill (`SKILL.md`) | MIT |
| [opendocs-extension](https://github.com/opendocs-cc/opendocs-extension) | Browser extension: publish ChatGPT, Claude and Gemini answers | MIT |
| [skills](https://github.com/opendocs-cc/skills) | Agent skills and the Claude Code plugin | MIT |

Everything is open source under the MIT license. To run your own instance, follow the [self-hosting guide](https://github.com/opendocs-cc/opendocs/blob/main/SELF_HOSTING.md): it's written so an AI agent such as Claude Code or Codex can do the setup for you. If you'd rather not, [opendocs.cc](https://opendocs.cc) runs it for you.

## Links

[Website](https://opendocs.cc) · [Docs](https://docs.opendocs.cc) · [Pricing](https://opendocs.cc/pricing) · [Self-hosting](https://github.com/opendocs-cc/opendocs/blob/main/SELF_HOSTING.md) · [X](https://x.com/opendocshq) · [Buy me a coffee](https://ko-fi.com/patrekurm)

Found a bug or have an idea? Open an issue on [opendocs](https://github.com/opendocs-cc/opendocs/issues), or on the repository it's about. Pull requests are welcome. Security reports go privately to hello@opendocs.cc, never to a public issue.
