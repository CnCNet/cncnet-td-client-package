# CnCNet Tiberian Dawn Client Package

<!-- <p align="center">
  <img src="package/Resources/ThemeDefault/splashScreen.png" width="256" alt="CnCNet Tiberian Dawn Client logo">
</p> -->

The official CnCNet [Command & Conquer: Tiberian Dawn](https://cncnet.org/tiberian-dawn) package for online play.
It provides the game-specific configuration, interface assets, launcher, and prebuilt binaries for the [XNA CnCNet Client](https://github.com/CnCNet/xna-cncnet-client), originally created by [Rampastring](https://github.com/Rampastring).

## Contributors

- [MahBoiDeveloper](https://github.com/MahBoiDeveloper)
- [CCHyper](https://github.com/CCHyper)
- [GrantBartlett](https://github.com/GrantBartlett)

## Special thanks

- [Bittah Commander and DTA team](https://cncnet.org/dawn-of-the-tiberium-age) — client theme basics

## Used projects

- [XNA CnCNet Client](https://github.com/CnCNet/xna-cncnet-client) (GNU GPLv3)
- [XNA CnCNet Client Launcher](https://github.com/CnCNet/xna-cncnet-client-launcher) (GNU GPLv3)
- [CnCNet Tiberian Dawn patches](https://github.com/CnCNet/td-patches) (GNU GPLv3)

## Development

> [!IMPORTANT]
> This repository does not contain the source code of the XNA CnCNet Client. It contains the Tiberian Dawn package and its configuration. Client code changes should be contributed to the [XNA CnCNet Client repository](https://github.com/CnCNet/xna-cncnet-client).

Configuration, theme, map-list, and other package changes should be made under `package` while preserving its directory layout. Released client and launcher binaries are kept up to date by scheduled GitHub Actions workflows that open pull requests when new upstream versions are available.

## Repository structure

- `package` — the exact directory structure delivered as the Tiberian Dawn client package.
  - `INI` — multiplayer map definitions.
  - `Maps/Custom` — location reserved for user-supplied custom maps.
  - `Resources` — client binaries, configuration files, compatibility components, sounds, and UI assets.
  - `Resources/ThemeDefault` — the default Tiberian Dawn theme.
  - `TiberianDawn.exe` — the Windows client launcher.
  - `LauncherUnixMono.sh` and `LauncherUnixWine.sh` — Unix launch scripts.
- `.github/workflows` — automated updates for the XNA CnCNet Client binaries and launcher.

## License

See [`package/LICENSE.md`](package/LICENSE.md) for the package license. Third-party components retain their respective licenses; the corresponding notices are included in `package/Resources`.

## Sponsored by

<a href="https://www.digitalocean.com/?refcode=337544e2ec7b&utm_campaign=Referral_Invite&utm_medium=opensource&utm_source=CnCNet" title="Powered by DigitalOcean">
  <img src="https://opensource.nyc3.cdn.digitaloceanspaces.com/attribution/assets/PoweredByDO/DO_Powered_by_Badge_blue.svg" width="201" alt="Powered by DigitalOcean">
</a>
