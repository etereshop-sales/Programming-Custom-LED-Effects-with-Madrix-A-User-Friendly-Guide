# Programming Custom LED Effects with Madri A User Friendly Guide
Welcome to the exciting world of LED effect customization! This comprehensive guide is designed to walk you through every step of the process, ensuring that even if you’re new to computers, you’ll be able to follow along and successfully create stunning LED effects.

---

##  Before You Begin 

Welcome to the exciting world of LED customization!

The main tool is **Madrix 3**, compatible with **Windows 10 or earlier**. It no longer supports free recording in later versions without a license.

> ⚠️ MacOS or Windows 11+ users will need to install a virtual machine (VM) to run Madrix 3.  
> ⚠️ If you have a Madrix license, ensure it supports enough **DMX universes** for your product.

---

##  Step 1 – Setting Up a Virtual Machine 

<details>
<summary><strong>VirtualBox (Windows / macOS)</strong></summary>

* Download and install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)  
* Recommended specs:
  * 8GB RAM
  * 32GB free disk space (preferably SSD)

* Steps:
  1. Download our prebuilt Windows 10 `.ova` image
  2. Open VirtualBox → Import Appliance
  3. Load `.ova` file and finish import
  4. Launch the VM

<!-- IMAGE PLACEHOLDER: VirtualBox import screen -->

> ⏳ First boot may be slow due to system updates (especially on HDDs).

</details>

<details>
<summary><strong>Hyper-V (Windows only)</strong></summary>

* Open **Turn Windows Features On or Off**  
* Enable **Hyper-V**, click OK, restart PC

* If Hyper-V is missing (common on Windows Home), run `hyperv.bat` as Administrator.

* Steps:
  1. Download `.vmcz` file
  2. Double-click → Import Virtual Machine
  3. Launch the VM

<!-- IMAGE PLACEHOLDER: Hyper-V import screen -->

> 🗝️ Default VM password: `etereshop`  
> 🎥 [Video Tutorial](https://www.youtube.com/watch?v=iJGeNG-NsPo)

</details>

<details>
<summary><strong>Tips & Troubleshooting</strong></summary>

* Configure RAM & CPU via: `VM → Settings → Memory / Processor`  
* To share drives:  
  - Connect → Show Options → Local Resources → Drives  
  - Choose USB or system drives

* Common issues:
  - Reduce VM RAM if total system memory is ≤ 8GB
  - Avoid running heavy apps in background while VM is active

<!-- IMAGE PLACEHOLDER: Hyper-V settings screen -->

</details>

---

## < Step 2 – Installing the Necessary Software >

<details>
<summary><strong>Drivers & Tools</strong></summary>

* Skip this if you used our preinstalled VM  
* Otherwise, install:

1. **Microsoft Visual C++ 2013 (x64 or x86)**  
2. **WinPcap**  
   - ⚠️ Must uninstall any **Npcap** version first  
3. **Madrix 3**  
   - Request from [sales@etereshop.com](mailto:sales@etereshop.com)  
4. **Effects Recorder**  
   - Just unzip and run

<!-- IMAGE PLACEHOLDER: msinfo32 system check -->

🎥 [Video Tutorial](https://www.youtube.com/watch?v=dO-x0v_YKjU)

</details>

---

## < Step 3 – Importing and Creating LED Effects >

<details>
<summary><strong>Open Your Project File</strong></summary>

* After your order, you receive an `.msz` Madrix file  
* Open via:
  - Double-click `.msz`  
  - OR Madrix → File → Open Setup

📧 Missing your file? Contact [sales@etereshop.com](mailto:sales@etereshop.com)

<!-- IMAGE PLACEHOLDER: Madrix project screen -->

</details>

<details>
<summary><strong>Effect Library & Templates</strong></summary>

* [Download the Library](https://drive.google.com/open?id=1n6zfrZB7e-kuGIrPIW2Oox5tQg4fkwhc)  
* [Watch tutorial](https://www.youtube.com/watch?v=fwkRx998_QM)  

</details>

<details>
<summary><strong>Make Your Own Effects</strong></summary>

* Create visuals using Madrix  
* Add **text** to effects → [Video](https://www.youtube.com/watch?v=D7ihn3LcXHc)  
* Experiment with **3D effects** → [Video](https://www.youtube.com/watch?v=fwkRx998_QM)

> ⚠️ Always close Madrix fully before loading a new project to avoid bugs.

</details>

---

## < Step 4 – Recording Your Effects >

<details>
<summary><strong>Use Effects Recorder</strong></summary>

1. Run `VS_PcapSniffer.exe`  
2. Select correct network adapter  
3. Click **Start Recording**  
4. If Artnet = 0, stop and try a different device

🎥 [Recording Tutorial](https://www.youtube.com/watch?v=ZZECUX7TrQk)

<!-- IMAGE PLACEHOLDER: Recorder UI and Artnet rising -->

> ⚠️ Trial version records only ~1 minute (due to blackout protection)

</details>

---

## < Step 5 – Copying Effects to the Controller’s SD Card >

<details>
<summary><strong>File Transfer Process</strong></summary>

* Power off product and remove SD card  
* Copy `.txt` effects to SD  
  - Format: `S1.txt`, `S5_logo.txt`, etc.  
  - Keep `config.txt` present  
* Reinsert card → Power on

📁 Folder can also contain backups or notes (ignored by controller)

<!-- IMAGE PLACEHOLDER: SD card structure -->

</details>

---

## < Common Problems >

<details>
<summary>* My recorded effect flickers / freezes *</summary>

✅ Reinstall **correct version** of WinPcap  
🔁 See [Step 2](#step-2--installing-the-necessary-software)

</details>

<details>
<summary>* Artnet is not increasing *</summary>

🛠️ Go to `Madrix → Preferences → Device Manager → ArtNet`  
☑️ Enable ArtNet output

</details>

<details>
<summary>* “Too long delay” error *</summary>

📶 Happens with **Wi-Fi** connections  
🔌 Use a **wired** Ethernet cable instead

</details>

<details>
<summary>* SD card files are duplicated *</summary>

⚠️ Always power down device **before** removing the SD card to avoid corruption.

</details>

---

## < Useful Links >

* [Full Knowledge Base](https://etereshop.zohodesk.com/portal/en/kb/articles/programming-of-led-effects-via-madrix)  
* [WinPcap Download](https://www.winpcap.org/install/default.htm)  
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)  
* [Madrix Tutorial Videos](https://www.youtube.com/@etereshop)  
* 📩 [Contact Support](mailto:sales@etereshop.com)

---
