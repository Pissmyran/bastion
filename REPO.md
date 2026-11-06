# REPO.md

The hub for the SSH client Bastion: the hub site, shared documentation and issues that concern every platform. The repository holds no code. The code lives in [bastion-apple](https://github.com/Pissmyran/bastion-apple), [bastion-linux](https://github.com/Pissmyran/bastion-linux), [bastion-windows](https://github.com/Pissmyran/bastion-windows) and [bastion-android](https://github.com/Pissmyran/bastion-android). It is the only thing the agent may change.

## Read first

1. [docs/platforms.md](docs/platforms.md): how the repositories fit together.
2. [docs/sync-format.md](docs/sync-format.md): when sync is involved. The format itself changes in `bastion-apple`.

## Commands

```bash
pip install --upgrade zensical && zensical build --strict
```

## Rules

- **No code here.** Code, tests and platform documentation change in the platform repositories.
- **Links** to the platform repositories and their sites are in `README.md`, `docs/` and `.github/ISSUE_TEMPLATE/config.yml`. If a repository is renamed, update all three.
- **The site is published on GitHub Pages only when a release is created.** A site change that should go out needs `feat:` or `fix:` in the title. The release gate is `.github/release-required-checks` (`Analyze (actions)`).
- **`site_url`** in `zensical.toml` is `https://docs.denied.se/bastion/`. Public documentation for every repository is published at `docs.denied.se/<repo>`, and links between the repositories' documentation use that form. Do not change `site_url` without the owner's decision.
- **Extra care:** links to the platform repositories and the release gate.
