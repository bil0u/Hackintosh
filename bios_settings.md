### BIOS Settings

Bios revision `F11c`. Optimized defaults + following settings :

- **Tweaker**
	- **Extreme Memory Profile (X.M.P.)** : `Profile1`
	- **Advanced CPU Settings**
		- **Hyper-Threading Technology** : `Enabled`
		- **VT-d** : `Enabled`
- **Settings**
	- **IO Ports**
		- **Internal Graphics** : `Enabled`
		- **DVMT Pre-Allocated** : `64M`
		- **DVMT total Gfx Mem** : `256M`
		- **WiFi** : `Disabled`
		- **Above 4g Decoding** : `Enabled`
		- **USB Configuration**
			- **XHCI Hand-Off** : `Enabled`
		- **SATA And RST Configuration**
			- **Sata Mode Selection** : `AHCI`
	- **Miscellaneous**
		- **Intel Platform Trust (PTT)** : `Disabled`
		- **Software Guard Extensions (SGX)** : `Disabled`
- **Boot**
	- **Fast Boot** : `Disabled`
	- **Windows 8/10 Features** : `Windows 8/10 WHQL`
	- **CSM Support** : `Disabled`
	- **Secure Boot**
		- **Secure Boot Enable** : `Disabled`


#### Patched :

The following values are manually patched as they do not appear in bios settings for this version

Variable | Code | Value | Tool
--- | --- | --- | ---
**CFG Lock** | `0x5C1` | `0x0` | CFGLock.efi or ModGrubShell.efi

> The following variables are missing for this bios version :
> - **Execute Disable Bit**

