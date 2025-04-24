About

The Atheros QCA9377 Wi-Fi chip is cheap and popular, but it was mostly made with Windows in mind.

The open-source driver (ath10k) works fine, but the firmware files aren’t fully documented. Some are reverse-engineered or shared by the community.

On Ubuntu 20.04, the default firmware is often outdated or buggy, which can cause Wi-Fi issues.
Fix

This is an updated firmware I found in the official Linux firmware repo — for some reason, Ubuntu doesn’t update it automatically.

To install it:

    Drop the file in:
    /lib/firmware/ath10k/QCA9377/hw1.0/

    Rename it to match the current firmware (usually firmware-5.bin)

    Reboot your machine

That’s it — your Wi-Fi should work better now.
