# Replugged theme template

[Use this template](https://github.com/replugged-org/theme-template/generate)

## Prerequisites

- NodeJS
- pnpm: `npm i -g pnpm`
- [Replugged](https://github.com/replugged-org/replugged#installation)

## Install

1. [Create a copy of this template](https://github.com/replugged-org/theme-template/generate)
2. Clone your new repository and cd into it
3. Install dependencies: `pnpm i`
4. Build the theme: `pnpm run build`
5. Reload Discord to load the theme

The unmodified theme replaces the Discord font with the old Whitney font. Credit to
[@overimagine1](https://github.com/Overimagine1/old-discord-font) for the snippet!

## Development

The code must be rebuilt after every change. You can use `pnpm run watch` to automatically rebuild
the theme when you save a file.

Building using the script above will automatically install the updated version of the theme in
Replugged. You can find the theme folder directories for your OS
[here](https://github.com/replugged-org/replugged#installing-plugins-and-themes).  
If you don't want to install the updated version, append the `--no-install` flag:
`pnpm run build --no-install`.

You can format the code by running `pnpm run lint:fix`. The repository includes VSCode settings to
automatically format on save.

API docs coming soon(tm)

## Distribution

For theme distribution, Replugged uses bundled `.asar` files. Bundled themes can be installed to the
same theme folder as listed above.

This repository includes a GitHub workflow to compile and publish a release with the asar file. To
trigger it, create a tag with the version number preceded by a `v` (e.g. `v1.0.0`) and push it to
GitHub:

```sh
git tag v1.0.0
git push --tags
```

The Replugged updater (coming soon™) will automatically check for updates on the repository
specified in the manifest. Make sure to update it to point to the correct repository!

You can manually compile the asar file with `pnpm run build-and-bundle`.

## Troubleshooting

### Make sure Replugged is installed and running.

Open Discord settings and make sure the Replugged tab is there. If not,
[follow these instructions](https://github.com/replugged-org/replugged#installation) to install
Replugged.

### Make sure the theme is installed.

Check the [theme folder](https://github.com/replugged-org/replugged#installing-plugins-and-themes)
for your OS and make sure the theme is there. If not, make sure you have built the theme and that
the `NO_INSTALL` environment variable is not set.  
You can run `replugged.themes.list().then(console.log)` in the console to see a list of themes in
the theme folder.

[release-badge]: https://img.shields.io/github/v/release/ClearVision/ClearVision-v6?include_prereleases&style=flat-square
[release-link]: https://github.com/ClearVision/ClearVision-v6/releases
[license-badge]: https://img.shields.io/github/license/ClearVision/ClearVision-v6?style=flat-square
[license-link]: https://github.com/ClearVision/ClearVision-v6/blob/master/LICENSE
[discord-badge]: https://discord.com/api/guilds/212324635356692500/widget.png?style=shield
[discord-link]: https://clearvision.gitlab.io/join
[issues-badge]: https://img.shields.io/github/issues/ClearVision/ClearVision-v6?style=flat-square
[issues-link]: https://github.com/ClearVision/ClearVision-v6/issues
[prs-badge]: https://img.shields.io/github/issues-pr/ClearVision/ClearVision-v6?style=flat-square
[prs-link]: https://github.com/ClearVision/ClearVision-v6/pulls

<div align="center">

# ClearVision v6

[![Releases][release-badge]][release-link]
[![License][license-badge]][license-link]
[![Discord Server][discord-badge]][discord-link]
[![Issues][issues-badge]][issues-link]
[![Pull Requests][prs-badge]][prs-link]

![v6 Sapphire](https://github.com/ClearVision/ClearVision-v6/raw/master/screenshots/6-stable.4.7.9.png)

</div>

## Theme Editor

You are now able to customize the theme with a preview before downloading it to your computer.

> [Theme Editor](https://bdeditor.dev/theme/clearvision)

_Thank you to @Gibbu to providing this._