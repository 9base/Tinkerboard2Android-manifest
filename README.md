> [!NOTE]
> **9base status: Preserved** · **Lifecycle: archived reference copy.**
>
> This is a historical fork of [TinkerBoard2-Android/manifest](https://github.com/TinkerBoard2-Android/manifest).
> 9base retains it for provenance and reference and does not actively maintain it.
> Upstream source and inherited authorship remain attributed to their original contributors.

# Tinkerboard2Android-manifest — 9base preservation notes

## Role and branch index

This repository preserves vendor Repo manifests for Tinker Board 2/2S Android
10 and Android 11 source releases. The default `main` branch contains the
upstream checkout instructions retained below; release XML lives on:

- [android10-rk3399](https://github.com/9base/Tinkerboard2Android-manifest/tree/android10-rk3399),
  including [default.xml](https://github.com/9base/Tinkerboard2Android-manifest/blob/android10-rk3399/default.xml);
- [android11-rk3399](https://github.com/9base/Tinkerboard2Android-manifest/tree/android11-rk3399),
  including [tinker_board_2-android11-2.0.1.xml](https://github.com/9base/Tinkerboard2Android-manifest/blob/android11-rk3399/tinker_board_2-android11-2.0.1.xml).

These manifests select vendor `TinkerBoard2-Android` repositories and Android
Open Source Project sources. They are related to the sibling Linux archives
by hardware family, not evidence that an Android checkout fetches the 9base
Linux kernel, U-Boot or rkbin forks.

All three exposed branches were identical to their same-named upstream
branches in the 8 October 2026 audit. No account-linked Zaryob-authored commits
were returned; an account filter does not resolve every possible unlinked
historical author. No complete Android build or current 9base integration was
established by this documentation work.

## Tinker Board 2 platform family

| Layer | Preserved 9base repository |
| --- | --- |
| Linux checkout manifests | [Tinkerboard2-manifest](https://github.com/9base/Tinkerboard2-manifest) |
| Linux kernel | [Tinkerboard2-kernel](https://github.com/9base/Tinkerboard2-kernel) |
| U-Boot bootloader | [Tinkerboard2-uboot](https://github.com/9base/Tinkerboard2-uboot) |
| Buildroot build system | [Tinkerboard2-buildroot](https://github.com/9base/Tinkerboard2-buildroot) |
| Debian/rootfs scripts | [Tinkerboard2-debian](https://github.com/9base/Tinkerboard2-debian) |
| Rockchip firmware and loaders | [Tinkerboard2-rkbin](https://github.com/9base/Tinkerboard2-rkbin) |
| Poky/OpenEmbedded/BitBake | [yocto-poky](https://github.com/9base/yocto-poky) |
| Android checkout manifests | [Tinkerboard2Android-manifest](https://github.com/9base/Tinkerboard2Android-manifest) |

The [Linux release manifest](https://github.com/9base/Tinkerboard2-manifest/blob/linux4.19-rk3399-debian10/default.xml) explicitly names the kernel, U-Boot,
Buildroot, Debian, rkbin and yocto-poky components. Its remote still points to
`TinkerBoard2`, not these 9base forks; it does not automatically select 9base's
historical Debian fix. This family is only a retained subset of the vendor's
larger source graph, not a self-contained complete BSP checkout.

The Android manifests concern the same board family but target a separate
`TinkerBoard2-Android` source graph; they do not establish use of these 9base
Linux components.

## Historical note

These preservation notes were reconstructed on **8 October 2026** from the
repository tree, exposed branches, commit history and upstream comparisons.
They are new archival documentation, not evidence that this explanation existed
at the historical fork date. The original reason for retention or any deployment
is not established by the inspected record. No contemporary build, support or
upstream synchronization commitment is implied.

---

## Original upstream README (preserved)

# manifest

This repo is used to download manifests for Tinker Board 2/2S Android source releases.

Please refer to the following URL to install Repo. 

    https://source.android.com/setup/develop#installing-repo

Please refer to the following URL to understand how to download the AOSP soure.

    https://source.android.com/setup/build/downloading

Then, you can issue the following commands to donwload the Android source releases for Tinker Board 2/2S.

    $ repo init -u https://github.com/TinkerBoard2-Android/manifest.git -b REVISION -m NAME.xml
    $ repo sync

Here REVISON is the manifest branch or revision (use HEAD for default) and NAME.xml is the initial manifest file.
