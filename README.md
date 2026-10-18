# imagegen-skills

Skills that make an agent generate design images worth building from: website comps, mobile app screens and brand kits, plus a pipeline that generates a site's design images first and then builds the site to match them.

By the author of [taste-skill](https://github.com/Leonxlnx/taste-skill). These skills used to live there and moved here in October 2026 so each repo does one job: taste-skill builds and checks real frontends, imagegen-skills makes the pictures.

## Skills

| Skill | Install name | What it does |
| --- | --- | --- |
| **[imagegen-frontend-web](skills/imagegen-frontend-web/SKILL.md)** | `imagegen-frontend-web` | Website comps: one image per section of a landing page, with varied composition and readable type. |
| **[imagegen-frontend-mobile](skills/imagegen-frontend-mobile/SKILL.md)** | `imagegen-frontend-mobile` | App screens and flows for iOS, Android and cross-platform, consistent across a set. |
| **[brandkit](skills/brandkit/SKILL.md)** | `brandkit` | Brand-guideline boards: logo directions, symbol systems, palettes, type and applications. |
| **[image-to-code](skills/image-to-code/SKILL.md)** | `image-to-code` | The whole pipeline: generate the design images, study them, then build the website to match. |

The first three produce images only. Use them with ChatGPT Images, Codex image mode or any agent that can generate images, then hand the frames to your coding agent. `image-to-code` needs an agent that can both generate images and write code.

## Install

```bash
npx skills add https://github.com/Leonxlnx/imagegen-skills --skill "imagegen-frontend-web"
```

Swap in any install name from the table, or leave out `--skill` to install all four.

<details>
<summary>Claude Code plugin</summary>

```
/plugin marketplace add Leonxlnx/imagegen-skills
/plugin install imagegen-skills@imagegen-skills
```

</details>

<details>
<summary>Codex plugin</summary>

```bash
codex plugin marketplace add Leonxlnx/imagegen-skills
codex plugin add imagegen-skills@imagegen-skills
```

Start a new Codex session afterwards so the skills are loaded.

</details>

Installed these from taste-skill before? Install them from here; the install names did not change.

## License

MIT. See [LICENSE](LICENSE).
