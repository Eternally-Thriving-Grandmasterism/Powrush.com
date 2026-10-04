# Powrush

Static website for Powrush, the game from Autonomicity Games Inc. The company site is [acitygames.com](https://acitygames.com).

The pages live in [`site/`](site/). `README.md` stays at the repository root and is not part of the published site.

## Preview

From the repository root:

```bash
python3 -m http.server 8080 --directory site
```

Open [http://127.0.0.1:8080/](http://127.0.0.1:8080/).

Links are relative, so the same files work on a GitHub Pages project URL and on the apex domain.

## What is on the site

Home, World, Systems, and Play. The pages are plain HTML, CSS, and one small theme script, with no trackers, no third-party embeds, and no external fonts.

Play is coming later. Online play is not available. There is no sign-up.

Contact: [info@Rathor.ai](mailto:info@Rathor.ai)

## Publishing

`.github/workflows/pages.yml` uploads only `site/`. The workflow has a `workflow_dispatch` trigger. The push trigger gets added when GitHub Pages is switched on.

`site/CNAME` contains `powrush.com`. The repository owner turns GitHub Pages on in the repository settings and chooses GitHub Actions as the source. This repository does not change that setting.
