# AGENTS.md – bastion

The hub for the SSH client Bastion: the hub site, shared documentation and issues that concern every platform. The repository holds no code. The code lives in [bastion-apple](https://github.com/Myrpisset/bastion-apple), [bastion-linux](https://github.com/Myrpisset/bastion-linux), [bastion-windows](https://github.com/Myrpisset/bastion-windows) and [bastion-android](https://github.com/Myrpisset/bastion-android).

Read the shared rules at the start of every session: [GOVERNANCE.md](https://raw.githubusercontent.com/Myrpisset/.github/main/GOVERNANCE.md) and [BASTION.md](https://raw.githubusercontent.com/Myrpisset/.github/main/BASTION.md).

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
- **`site_url`** in `zensical.toml` is a custom domain, while the repository's homepage is `myrpisset.github.io/bastion`. Do not change `site_url` without the owner's decision.
- **Extra care:** links to the platform repositories and the release gate.
