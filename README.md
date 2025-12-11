# RPCS3 M4 Mac Build with RPCN v1.5

A custom RPCS3 build for Apple Silicon Macs (M1/M2/M3/M4) with RPCN v1.5 online support.

## Why This Build?

Recent RPCS3 builds have stability issues on M4 Macs, but build **0.0.37-18115** works great. However, on December 8, 2025, the RPCN server was updated to v1.5, breaking online connectivity for older builds.

This custom build combines:
- ✅ **Base:** RPCS3 0.0.37-18115 (last stable M4 Mac build)
- ✅ **Patch:** RPCN v1.5.0 protocol update for online play

## Download

📥 **[Download Latest Release](../../releases/latest)**

## Installation

1. Download the zip file from Releases
2. Unzip and drag `rpcs3.app` to your **Applications** folder
3. **First launch:** Right-click the app and select "Open" (to bypass Gatekeeper)

### If you get a code signing error:

Open Terminal and run:
```bash
xattr -cr /Applications/rpcs3.app
codesign --force --deep --sign - /Applications/rpcs3.app
```

## Notes

- This build is specifically for **Apple Silicon Macs** (arm64)
- Your existing RPCS3 config, games, and saves will work
- Config location: `~/Library/Application Support/rpcs3/`

## Source

Built from the official RPCS3 source with:
- Base commit: [6b238d8](https://github.com/RPCS3/rpcs3/commit/6b238d847fd7576773d1d5653a90dbc1acadd313) (build 37-18115)
- RPCN v1.5 patch: [PR #17825](https://github.com/RPCS3/rpcs3/pull/17825)

## Disclaimer

This is an unofficial custom build. For issues specific to this build, please open an issue here. Do NOT report issues to the official RPCS3 project.

---

*Built with ❤️ for the PS3 emulation community*

