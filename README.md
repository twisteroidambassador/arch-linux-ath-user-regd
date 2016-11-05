# `linux-ath-user-regd`

This repository contain the `PKGBUILD` and associated files for `linux-ath-user-regd`, an Arch Linux kernel with patched Atheros drivers that ignore regulatory domain settings in the wireless cards' EEPROM.

The purpose of the patches is to remove the "NO-IR" restriction on the 5GHz band on many consumer Atheros wireless cards, so they can be used in master mode on 5GHz. Regulatory settings in software (set by `hostapd`, `iw reg set`, etc.) are still honored.

The patches are adapted from those provided by OpenWRT here: https://dev.openwrt.org/browser/trunk/package/kernel/mac80211/patches
