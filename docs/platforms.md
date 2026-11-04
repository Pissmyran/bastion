# The platforms

Each platform is its own repo with its own code, versions and documentation. A platform can be released without affecting the others.

| Repo | For | Built with | Links |
| --- | --- | --- | --- |
| [Bastion for Apple](https://github.com/Myrpisset/bastion-apple) | iPhone, iPad, Mac and Apple TV | Swift, SwiftNIO SSH, SwiftUI | [Documentation](https://myrpisset.github.io/bastion-apple/) · [Releases](https://github.com/Myrpisset/bastion-apple/releases) |
| [Bastion for Linux](https://github.com/Myrpisset/bastion-linux) | the Linux desktop | Rust, GTK 4, libadwaita, VTE, russh | [Documentation](https://myrpisset.github.io/bastion-linux/) · [Releases](https://github.com/Myrpisset/bastion-linux/releases) |
| [Bastion for Windows](https://github.com/Myrpisset/bastion-windows) | Windows | C#, .NET, WinUI, SSH.NET | [Documentation](https://myrpisset.github.io/bastion-windows/) · [Releases](https://github.com/Myrpisset/bastion-windows/releases) |
| [Bastion for Android](https://github.com/Myrpisset/bastion-android) | Android | Kotlin, Gradle, Apache MINA SSHD | [Documentation](https://myrpisset.github.io/bastion-android/) · [Releases](https://github.com/Myrpisset/bastion-android/releases) |

## What is shared

- **The sync format.** Apple, Linux and Windows read and write the same format for the host list; see [Sync format](sync-format.md).
- **The rules.** Every repo follows [GOVERNANCE.md](https://github.com/Myrpisset/.github/blob/main/GOVERNANCE.md) in `Myrpisset/.github`.
- **The review.** Every repo inherits the central CodeRabbit configuration in [Myrpisset/coderabbit](https://github.com/Myrpisset/coderabbit).

## What is not shared

- **Code.** There is no shared code base. The Swift core SSHCore is only used by the Apple apps; the other platforms have their own implementations.
- **Versions.** Each repo has its own tags. `v1.0.0` for Linux says nothing about Windows.
