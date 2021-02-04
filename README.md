# Atikmdag patcher 1.4.8



#### Atikmdag patcher — cancels driver signature verification for video cards on chipsets to ensure high resolutions and frequencies, removing clock frequency limits, it is also used for correct driver operation after flashing video cards and removes overclocking limits.



# What is the Atikmag patcher for?



#### Atikmdag Patcher 1.4.8 is needed after — when no drivers are installed on the flashed video card or error 43 pops up after the firmware (the device reported an error). If you do not see the video card after the firmware or the drivers are not installed, this patch will help you. After flashing the BIOS, it is required.



# How to use Аtikmdag patcher
- Download and unpack **Atikmdag-Patcher-1.4.8.zip** to any convenient place
- Run the file «Atikmdag-Patcher-1.4.8»
- Wait until the program finds all the limits, select «Yes» to fix and re-sign the driver.



![1](https://sun9-25.userapi.com/impg/rB4C9sqIu8iDILJ10TA_4-J7mnwho7H841cZpQ/gdlOrLgtRAc.jpg?size=335x417&quality=96&proxy=1&sign=54ea8b2be7722c60bb28677b66cfbc98&type=album)<br>
(If something went wrong, try reinstalling your graphics card driver)

# Requirements:

* Windows Vista or later
* 5000-series GPU or newer
* CrossFire requirements:
  * R9 285/290/290X/295X2 and newer cards can handle higher pixel clocks without CrossFire bridges.
  * Older cards require two CrossFire bridges if the pixel clock is greater than 300 MHz. This is only possible with cards that have two connectors. It will not work properly with more than two cards. Dual-GPU cards such as the 7990 will not work properly at higher pixel clocks.
  
# Compatibility:
  * Version 1.4.9 is compatible with Catalyst 11.9 to Adrenalin 20.12.2. It can be used with future versions if it finds the limits you need.
  
# Getting started:
1. Run atikmdag-patcher.exe. (If you only need the BIOS signature patch, rename it to atikmdag-patcher-bios.exe first.)
2. If all limits are found, click "Yes" to patch and sign. If a limit is not found or if multiple matches are found, the patcher needs to be updated.
3. Reboot.

# Known issues:

* Legacy drivers may have issues with HDCP and video acceleration with the patch.

* Workarounds for video playback issues with legacy drivers:
  * Disable hardware acceleration in the Flash Player settings (right-click on any Flash video and click "Settings...").
  * Use the Codec Tweak Tool to disable DXVA hardware acceleration under "Various Tweaks" (in the "Miscellaneous" section).
  
* Older cards require the "LCD standard" vertical blanking/total to reduce the memory clock when idle. Horizontal values can still be reduced if necessary. Newer cards can handle some lower values depending on the resolution and refresh rate.
* Older cards have a design limitation unrelated to the patch that causes video acceleration to scramble the screen if the vertical blanking/total is below standard with the video card's memory overclocked or with multiple monitors connected. Skype is known to trigger this problem. Either don't overclock the video card's memory, or use the "LCD standard" vertical blanking/total in CRU.

# Recent changes:
- 1.4.9: Fixed HDMI-DVI limit for 20.11.2 and HBlank limit for 20.5.1.<br>
- 1.4.8: Updated for 20.5.1.<br>
- 1.4.7: Find new SL-DVI/HDMI limit.<br>
- 1.4.6: Find new HDMI-DVI limit.<br>
- 1.4.5: Updated for 17.4.1. Find new DP-DVI/HDMI limit.<br>
- 1.4.4: Find BIOS signature check.<br>
- 1.4.3: Fixed HBlank limit for 16.12.1.<br>
- 1.4.2: Find 56 horizontal blanking (HBlank) limit.<br>
- 1.4.1: Fixed an issue that prevented the driver from loading correctly with earlier versions of Windows 10. This does not affect the anniversary update.<br>
- 1.4.0: Updated for 16.9.1. Changed the way the driver is located and patched. Replaced 640x480 limit with low-resolution limit. Fixed VGA limit for 32-bit.<br>
- 1.3.6: Find 10-resolution limit for Radeon Settings.<br>
- 1.3.5: Updated for 15.11 Crimson. Find 640x480 limit for Radeon Settings.<br>
- 1.3.4: Try to improve finding DVI/HDMI limit for newer drivers. Removed blue screen workaround for 14.6/14.7.<br>
- 1.3.3: Updated for 15.3. Fixed DVI/HDMI limit for 32-bit.<br>
- 1.3.2: Updated for 15.2. Fixed DVI/HDMI limit for 64-bit.<br>
- 1.3.1: Find 297 MHz HDMI 1.3+ limits. Run 3 times to properly repatch an existing installation.<br>
- 1.3: Removed blue screen workaround for 14.9. Fall back to self-signing if signing fails.<br>
- 1.2.7: Attempt to work around some antivirus false positives. Repatching is not necessary.<br>
- 1.2.6: Fixed AMD APP encoding for 14.6.<br>
- 1.2.5: Updated for 14.6. Fixed TMDS and VGA limits. Implemented workaround for SYSTEM_SERVICE_EXCEPTION blue screens.<br>
- 1.2.4: Updated for 14.4. Fixed SL limit on DL-DVI.<br>
- 1.2.3: Updated for 13.30 and upcoming 14.x releases.<br>
- 1.2.2: Find new HDMI limit for 12.9+.<br>
- 1.2.1: Find 400 MHz VGA limit.<br>
- 1.2: Test mode no longer required.
