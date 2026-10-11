# skills

Personal [Agent Skills](https://agentskills.io/home) collection. Install any skill with [`npx skills`](https://github.com/vercel-labs/skills) (no cloning, no package.json needed — GitHub is the registry).

## Install

```bash
# List available skills without installing
npx skills add paperbenni/skills --list

# Install all skills (interactive picker)
npx skills add paperbenni/skills

# Install one skill
npx skills add paperbenni/skills --skill bozos

# Install globally (available in every project)
npx skills add paperbenni/skills --skill bozos -g

# Non-interactive (CI-friendly)
npx skills add paperbenni/skills --skill bozos -g -a opencode -y
```

Update later with:

```bash
npx skills update bozos
```

## Repo layout

Any public GitHub repo with discoverable `SKILL.md` files is installable. This repo uses the standard catalog layout:

```
skills/
  <skill-name>/
    SKILL.md        # required: name + description frontmatter, then instructions
    references/     # optional: extra docs the agent loads on demand
    scripts/        # optional: executable helpers
    assets/         # optional: templates, images, data
```

`name` must match its directory, be lowercase alphanumeric with single hyphens, 1–64 chars. `description` must be 1–1024 chars. Validate with:

```bash
npx skills add ./ --list
```

## Add a new skill

```bash
npx skills init skills/my-skill
# edit skills/my-skill/SKILL.md, then commit and push
```

