# installTAK for Raspberry Pi 4 (TAK Server 5.3)

This repository provides a customized `installTAK` script specifically adapted for the Raspberry Pi 4 Model B running Raspberry Pi OS (Debian 12 or 13, "Bookworm" or "Trixie").  
It automates the installation and initial setup of TAK Server 5.3, with Pi-optimized tweaks and required dependencies.

> **Credit:** This project adapts the original installer and workflow from [mytecknet.com](https://mytecknet.com/lets-build-a-tak-server/).  
> All rights to the original author. This repository only customizes the script for Pi hardware.

---

## 🚀 Features

- **Automated Installation:** TAK Server 5.3 setup is fully scripted.
- **Pi Hardware Optimized:** Tweaks for Raspberry Pi 4 Model B are included.
- **Dependency Management:** All required packages are preinstalled.
- **Simplified Setup Wizard:** Guided prompts help with first-time configuration.
- **Compatible OS:** Supports Raspberry Pi OS (Debian 12 "Bookworm" or 13 "Trixie").
- **Workflow Match:** Follows the original installTAK wizard logic.

---

## 📦 Requirements

**TAK Server installation files must be manually downloaded from [tak.gov](https://tak.gov) (login required).  
_These files cannot be redistributed via this repository due to licensing restrictions._**

**After downloading from TAK.gov, place the following files in the same directory as the script:**
- `takserver_5.3-RELEASE30_all.deb`
- `takserver-public-gpg.key`
- `deb_policy.pol`

 
**Example directory:**
```
installTAK/
 ├── installTAK
 ├── takserver_5.3-RELEASE30_all.deb
 ├── takserver-public-gpg.key
 └── deb_policy.pol
```
---

## 🧰 Prerequisites

- **Device:** Raspberry Pi 4 Model B
- **OS:** Raspberry Pi OS (Debian GNU/Linux 12 or 13)
- **RAM:** 4GB or higher recommended
- **Connectivity:** Internet access required for package installation

The script will automatically install all required dependencies for TAK Server.

---

## 📥 Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/dev-lester/TAKServer-install-script.git
   ```

2. **Enter the repo directory:**
   ```sh
   cd TAKServer-install-script
   ```

3. **Make the script executable (if necessary):**
   ```sh
   chmod +x installTAK
   ```

4. **Place the three TAK.gov files in the same folder.**

5. **Run the installer:**
   ```sh
   ./installTAK takserver_5.3-RELEASE30_all.deb
   ```

---

## 🧙‍♂️ Installation Wizard

After launching the script, you'll be guided through:

- Admin credential setup
- Enabling encrypted connections
- Certificate management
- Federation options
- Initial server configuration

Just follow the interactive prompts to complete your installation.

---

## ℹ️ Notes

- This script and repository are **NOT** officially supported by TAK.gov.
- Some Raspberry Pi environments may need tweaks for systemd integration.
- If you encounter issues, refer to the [original guide](https://mytecknet.com/lets-build-a-tak-server/) and TAK Server documentation.

---

## 🙏 Credits

Much respect and gratitude to the original author of the installTAK server guide and script:  
[https://mytecknet.com/lets-build-a-tak-server/](https://mytecknet.com/lets-build-a-tak-server/)

This project simply adapts the installer for Raspberry Pi compatibility.

---

## 🛠️ Contributions

PRs and issues are welcome, especially for improving compatibility with Raspberry Pi hardware or newer Pi OS versions.

---

## 📜 License

This project adapts and redistributes an installer script for personal/hobby use.  
**TAK Server binaries are NOT included and must be obtained directly from TAK.gov by authorized users.**

---
