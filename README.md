<div align="center">

![logo](./assets/icon.svg)

# WandEnhancer

[![GitLab Mirror](https://img.shields.io/badge/GitLab-mirror-fc6d26?logo=gitlab)](https://gitlab.com/kitbyte/wand-enhancer)


## 💫 What features are improved?

✅ Local environment configuration management <br/>
✅ Automated compatibility adjustments for new client versions <br/>
✅ Advanced layout and theme customization (Client-side only) <br/>
✅ AI Features <br/>
✅ Remote web panel (Remote Connect on mobile) <br/>

## 🌐 Remote Web Panel
WandEnhancer includes a built-in **Remote Web Panel** allowing you to control app features directly from your phone.


### Troubleshooting & Remote Access:
- **Page isn't loading?** First, ensure both your PC and phone are connected to the **same local network**. Some routers and guest Wi-Fi networks enable client isolation/AP isolation, which blocks devices on the same SSID from reaching each other. If it still does not load, check Windows Firewall and allow inbound traffic on TCP port `3223` for your local network. If Windows marked your connection as **Public**, switching it to **Private** can also help.
- **Using mobile data or a different network?** If you want to use the panel over mobile data (LTE/5G) or from an entirely different network, you can use [Tailscale](https://tailscale.com/) or similar VPN tools.
- The panel uses plain HTTP on port `3223` and has no pairing code. Anyone who can reach that port can view the panel and control the active trainer, so use it only on a trusted LAN/VPN and never expose the port directly to the internet.
- The panel protocol does not include your Wand bearer token or installation-path fields.


### Testing a release candidate

- `master` is the stable source. Select a `feature/rc_*` branch in your fork's **Run workflow** branch selector only when the maintainer explicitly asks for candidate testing. Ensure that branch contains the upstream commit you intend to test; syncing `master` does not update a separate RC branch.
- You do **not** need to open a pull request to this repository to build your fork.
- Record the workflow's source commit SHA, not just `2.0.0.0`: the RC tag, RC branch and a local build may contain different fixes.
- For startup failures, attach `launcher.log` and, if relevant, `launcher.prev.log` from the Wand installation root. They include the build commit and applied patches. Remove personal paths or other private information before sharing.
- Include the exact Wand version and stable/beta channel, selected patches, and whether the failure happened on a fresh install, an update, or Restore. Do not attach executables, account tokens or storage dumps.

*Here how you do it:*

https://github.com/user-attachments/assets/7966cabe-0aa6-424d-8c2f-981ad91e0f91




### Requirements

- `Visual Studio 2022` or `Build Tools for Visual Studio 2022` with `MSBuild`
- .NET Framework 4.8 desktop build tools / targeting pack


---
## 🖼️ Screenshots
![1](./assets/screenshots/app1.png)
<div align='center'>

![2](./assets/screenshots/app2.png)
</div>


## 📜 License
This project is licensed under the Apache-2.0 - see the [LICENSE](LICENSE.md) file for details.


## ❤️ Support

If you find this project useful, you can support its development using any of the options below 🙌

[![Patreon](https://img.shields.io/badge/Patreon-donate-f96854.svg?logo=patreon)](https://www.patreon.com/kitbyte/gift)
[![USDT TRC20](https://img.shields.io/badge/USDT--TRC20-donate-26a17b.svg?logo=tether)](https://tronscan.org/#/address/TQdvau8pAy5Tg1Aa588tTcPCFgbcHtuoxc)
[![BTC](https://img.shields.io/badge/BTC-donate-f7931a.svg?logo=bitcoin)](https://www.blockchain.com/explorer/addresses/btc/1EZKDcyU8REm9JW5xwXJqSpn5Xaq5yAWWX)
[![ETH](https://img.shields.io/badge/ETH-donate-3c3c3d.svg?logo=ethereum)](https://etherscan.io/address/0xd904d9d0557f88bbb1c4ab3582b4ca0d8a730e8d)


---

> **Legal Disclaimer:**
> This project is a third-party enhancement tool intended solely for educational, research, and local interoperability purposes. It does not distribute any proprietary code or bypass server-side validations. All modifications are performed locally to customize the user's interface.

---
