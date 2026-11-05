# The platforms

Each platform is its own repo with its own code, versions and documentation. A platform can be released without affecting the others.

| Repo | For | Built with | Links |
| --- | --- | --- | --- |
| [Bastion for Apple](https://github.com/Pissmyran/bastion-apple) | iPhone, iPad, Mac and Apple TV | Swift, SwiftNIO SSH, SwiftUI | [Documentation](https://docs.denied.se/bastion-apple/) · [Releases](https://github.com/Pissmyran/bastion-apple/releases) |
| [Bastion for Linux](https://github.com/Pissmyran/bastion-linux) | the Linux desktop | Rust, GTK 4, libadwaita, VTE, russh | [Documentation](https://docs.denied.se/bastion-linux/) · [Releases](https://github.com/Pissmyran/bastion-linux/releases) |
| [Bastion for Windows](https://github.com/Pissmyran/bastion-windows) | Windows | C#, .NET, WinUI, SSH.NET | [Documentation](https://docs.denied.se/bastion-windows/) · [Releases](https://github.com/Pissmyran/bastion-windows/releases) |
| [Bastion for Android](https://github.com/Pissmyran/bastion-android) | Android | Kotlin, Gradle, Apache MINA SSHD | [Documentation](https://docs.denied.se/bastion-android/) · [Releases](https://github.com/Pissmyran/bastion-android/releases) |

## What is shared

- **The sync format.** Apple, Linux and Windows read and write the same format for the host list; see [Sync format](sync-format.md).
- **The rules.** Every repo follows [GOVERNANCE.md](https://github.com/Pissmyran/.github/blob/main/GOVERNANCE.md) in `Pissmyran/.github`.
- **The review.** Every repo inherits the central CodeRabbit configuration in [Pissmyran/coderabbit](https://github.com/Pissmyran/coderabbit).

## What is not shared

- **Code.** There is no shared code base. The Swift core SSHCore is only used by the Apple apps; the other platforms have their own implementations.
- **Versions.** Each repo has its own tags. `v1.0.0` for Linux says nothing about Windows.
