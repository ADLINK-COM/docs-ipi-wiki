Changs from v1.07.100:
  1. Connect MMC via UART 2 setting baudrate to 57600Hz.
  2. Update srp-r1.08.
  3. Change RCB0 HI setting to enable PCIe device (LAN card).
  4. Support capsule update.

How to update BIOS/SCP FW:
  1. Unzip to a FAT32 USB disk and boot in to UEFI shell with it.
  2. Run fwu.nsh in UEFI Shell to update BIOS.
  3. Reboot to UEFI Shell to run capsule.nsh to update SCP FW 1.08.

Files list:
  efi\boot\bootaa64.efi  : shell for ARM64
  capsule.nsh: script to flash SCP FW.
  ComHpcAlt_scp_1.07.300.img : SCP FW image.
  ComHpcAlt_tianocore_atf_1.07.301.img : BIOS image.
  fwu.nsh    : script to flash BIOS.
  readme.txt : this file.
  XTools.efi : flash tool. 
