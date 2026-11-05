# Bastion

**Documentation:** [docs.denied.se/bastion](https://docs.denied.se/bastion/)

Bastion is an SSH client for several platforms. Each platform has its own repo with its own code, versions and documentation. This repo is the hub: it gathers the links, describes what is shared and takes issues that concern every platform.

## The platforms

| Repo | For | Built with | Documentation |
| --- | --- | --- | --- |
| [Bastion for Apple](https://github.com/Myrpisset/bastion-apple) | iPhone, iPad, Mac and Apple TV | Swift, SwiftNIO SSH, SwiftUI | [Documentation](https://docs.denied.se/bastion-apple/) |
| [Bastion for Linux](https://github.com/Myrpisset/bastion-linux) | the Linux desktop | Rust, GTK 4, libadwaita, VTE, russh | [Documentation](https://docs.denied.se/bastion-linux/) |
| [Bastion for Windows](https://github.com/Myrpisset/bastion-windows) | Windows | C#, .NET, WinUI, SSH.NET | [Documentation](https://docs.denied.se/bastion-windows/) |
| [Bastion for Android](https://github.com/Myrpisset/bastion-android) | Android | Kotlin, Gradle, Apache MINA SSHD | [Documentation](https://docs.denied.se/bastion-android/) |

## Shared

- **The sync format** for the host list is shared by the platforms that sync. The source is the Swift models in [Bastion for Apple](https://github.com/Myrpisset/bastion-apple); the other repos test against copies of the fixtures from there.
- **The projects** of the organization are listed at [github.com/orgs/Myrpisset/projects](https://github.com/orgs/Myrpisset/projects).
- **The rules** for working in every repo are in [GOVERNANCE.md](https://github.com/Myrpisset/.github/blob/main/GOVERNANCE.md).

## Reporting

- **Bugs or requests for one platform:** open an issue in that platform's repo.
- **Anything that concerns every platform** (the sync format, shared documentation): open an issue here.
- **Security problems:** follow [SECURITY.md](SECURITY.md).

## History

Until October 2026 every platform lived in this repo. The old code remains in the Git history and in the releases up to v0.1.3.
