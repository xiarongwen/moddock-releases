# MODDOCK 0.5.0-beta.20261013.1 — public testing build

MODDOCK (游匣) is a desktop application for discovering community mods, downloading permitted files, and managing mods for locally installed PC games. This prerelease is intended for testing and Nexus Mods integration review.

## Downloads

- `Moddock-0.5.0-beta.20261013.1-windows-x64-Setup.exe`: Windows 10/11 x64 installer.
- `SHA256SUMS.txt`: SHA-256 checksum for the installer and reviewer guide.
- `REVIEWER-GUIDE.md`: English navigation and integration test instructions.

The installer is unsigned. Windows installation, game deployment and uninstall have not yet been verified on a physical Windows machine. This is a testing build, not a stable release.

## Included

- A MOD Workshop tab with Nexus Mods, GameBanana and Steam Workshop entry points.
- Browsing and downloading before associating a locally installed game.
- Steam library discovery, Windows Epic detection and a native folder picker for additional Steam libraries.
- Source connection cards, local OS-backed encryption for API keys, and restoration for the same MODDOCK account after restart.
- Download progress and verification, installation previews, backup/restore and game-specific rules.
- Updated game-library cards and navigation.

## Nexus integration status

Application registration is pending. Nexus SSO is implemented but is unavailable until Nexus assigns an application slug. The Personal API Key entry is provided for development testing. Testers must use their own Nexus account and permissions; the build contains no Nexus credentials.

Non-Premium downloads follow the Nexus website's Mod Manager Download / NXM authorization flow where required. MODDOCK does not bypass Nexus download restrictions or create Nexus accounts for users. Nexus API keys are encrypted on the local computer and are not uploaded to MODDOCK's account service. There is no hosted mod-file mirror or bulk-download service.

Steam subscriptions and downloads are handled by Steam. Not every game has a Steam Workshop. GameBanana downloads require a public file link supplied by the source.

Providing this testing build does not imply endorsement by Nexus Mods, GameBanana or Valve.

## Test access

Review credentials are supplied directly to the Nexus support team in the existing application-registration ticket. No password is included in this release page or in the installer. Other testers may use the in-app registration flow.

## Validation

Automated checks passed (113 tests) before packaging. The installer payload was checked against the frozen application snapshot, including the rendered UI assets and runtime dependencies. Its embedded server was extracted and exercised on macOS: the reviewer account signed in successfully and was permitted to configure source connections. These checks do not replace Windows installation or real-game deployment testing.

## 中文说明

这是游匣的公开测试版本，提供 MOD 工坊、自动扫描和选择游戏库、来源授权本机加密保存、下载与安装预览等功能。Nexus 应用注册仍在审核，尚不能使用一键连接；个人 API Key 入口仅供开发测试。Steam 创意工坊的订阅和下载由 Steam 完成。

下载 Windows x64 安装包后运行安装。安装包未签名，Windows 实机安装、部署游戏 MOD 和卸载尚待验证。测试账号由维护者单独提供，不包含在安装包中。
