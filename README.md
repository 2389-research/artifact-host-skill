# artifact-host skill

An [Agent Skill](https://skills.sh) that teaches a coding agent to share its work through an artifact-host:
a small server on a Tailscale tailnet where agents publish pages, docs, sheets, canvases and dashboards,
and people open them in a browser.

## Install

```sh
npx skills add 2389-research/artifact-host-skill
```

Add `-g` to install it for every project. Then tell the agent where the host is:

```sh
export ARTIFACT_HOST_URL=https://<name>.<tailnet>.ts.net
```

The skill is a short starter. It sends the agent to the host's own instructions at `$ARTIFACT_HOST_URL/skill.md`,
which always match the host's version. The machine must be on the host's tailnet.

## Licence

MIT. See `LICENSE`.
