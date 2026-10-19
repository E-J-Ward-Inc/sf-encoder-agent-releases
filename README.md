# Ward Encoder Agent releases

Installers for the Ward Encoder Agent, the Windows program that lets SimplyFuel card encoding pages talk to card encoders and card printers attached to the PC. This repository holds releases only; the source is maintained privately by E. J. Ward, Inc.

## Install

1. Download `WardEncoderAgent-<version>.msi` from the latest release on the [Releases](../../releases) page.
2. Check the download: `certutil -hashfile WardEncoderAgent-<version>.msi SHA256` must match the `.sha256` file on the release.
3. Run the MSI. It installs for all users, starts the agent at sign-in, and upgrades an installed agent in place.

Silent install for Group Policy, Intune or other management tools:

```
msiexec /i WardEncoderAgent-<version>.msi /qn
```

Requires Windows 11. Releases marked "Pre-release" are unsigned test builds and are not offered by the agent's update check.

## Support

Contact E. J. Ward support.
