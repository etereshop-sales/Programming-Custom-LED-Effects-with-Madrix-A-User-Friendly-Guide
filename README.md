# Programming Custom LED Effects with Madri A User Friendly Guide
Welcome to the exciting world of LED effect customization! This comprehensive guide is designed to walk you through every step of the process, ensuring that even if you’re new to computers, you’ll be able to follow along and successfully create stunning LED effects.

---

## Before You Begin

Welcome to the exciting world of LED effect customization! This comprehensive guide is designed to walk you through every step of the process, ensuring that even if you’re new to computers, you’ll be able to follow along and successfully create stunning LED effects.
The main way to create and record effects is to use Madrix software. This is commercial software that requires a subscription, but the free version is enough for you to work. But unfortunately, after version 3, Madrix software no longer allows you to record effects without a license, so you will need to install Madrix 3 if you want to use it for free.


**If you have a license, then you will only need a program to record effects. However, make sure that your license gives you enough universes for your product.**

Madrix 3 runs on **Windows 10** (or earlier), and it is not supported on Mac OS or later versions of Windows. But if you don’t have this operating system, then don’t worry - we have prepared instructions for you to install a virtual machine that will already have all the necessary software to get started!

**Recommended PC specifications for running a virtual machine: - 8 GB of RAM - 32 GB of free disk space. If possible, put it on an SSD drive, because HDD performance is low for virtual machines (they will slow down).**

**Conclusion:**

* If you have Mac OS or Windows 11 and above, you will need a virtual machine to run Madrix 3. Proceed to the first step.

* If you have a license to work in Madrix, then you can use any version, but pay attention to the number of universes available in your license. Install effects recorder from step 2 and proceed to step 3.

* If you have an OS that supports Madrix 3, go to step 2.

*If you already have all the necessary software and you just want to create effects, proceed to step 3.

---

##  Step 1 – Setting Up a Virtual Machine 

<details>
<summary><strong>VirtualBox (Windows / macOS)</strong></summary>

**We have a prepared Windows 10 image for you and we recommend using it. If desired, you can build the virtual machine image that you want to use yourself, but do this only if you already know how to work with virtual machines.**

If you are a Windows user, then we have 2 options for you to install a virtual machine: 1) Using a third-party VirtualBox 2) Using the built-in Hyper-V
The difference is that Hyper-V is a virtualization system built into Windows, which works better than VirtualBox in this case. Therefore, we recommend this method, but it may seem more complicated to you. However, if you encounter any problems with it, then you can always return to the VirtualBox option.
If you are a **macOS** user, then only the method using VirtualBox is suitable for you.

**Important: the virtual machine may lag a lot when it is first started. In this case, after logging into the user’s account, let Windows work for a while so that it makes all the necessary changes. This can take from 20-30 minutes to 1-2 hours, depending on the performance of your system. Most often, slowdowns are caused by installing the system on the HDD. If possible, install the virtual machines on an SSD drive.**

**1. Installing VirtualBox**

Download [VirtualBox](https://www.virtualbox.org/wiki/Downloads) from the official website and install it on your PC. 

![unnamed](images/1.png)

**2. Creating a virtual machine**

> The user’s password is “etereshop”

Steps:
1. Download the Windows.ova file (this is an archived virtual machine image)
2. Launch VirtualBox, click Import
3. Select the downloaded file Windows.ova
4. Select the appropriate settings and wait for the import to complete
   
We also have a video tutorial on installing and configuring this virtual machine.
[![Watch the tutorial on YouTube](https://img.youtube.com/vi/iJGeNG-NsPo/hqdefault.jpg)](https://youtu.be/iJGeNG-NsPo)

</details>

<details>
<summary><strong> An alternative way for Windows users: Hyper-V</strong></summary>

** Enabling the Hyper-V component**
   
Hyper-V is a built-in component of Windows, i.e. you do not need to install any software to run a virtual machine, but you may need the Internet so that Windows can get the necessary files. To enable this component, you need to do the following: 
1. Search for Turn Windows features on or off
2. Check the Hyper-V component
3. Click OK, wait for the changes to be made and restart the computer

![unnamed](images/2.png)

If you **do not see the Hyper-V** component in the list (most likely you are a Windows Home distribution user), then you can install it using a special file: hyperv.bat To do this, follow these steps: 1. Download the file 2. Run it as an administrator: select the file, right-click, select run as an administrator. 3. Wait for the installation to finish. 4. At the end, you will be prompted to restart your computer, you can type “y” or “n” **without quotes** and press enter. However, a reboot is necessary in any case to make changes.

After this step, the **Hyper-V** Manager application will appear on your system - with it you will be able to manage your virtual machines.

**Creating a virtual machine**

1. Download the [Madrix.vmcz](https://drive.google.com/file/d/1Oc9T0QdLcCz-ylFizRLqyfM9VQiR-m5G/view?pli=1) file (this is an archived virtual machine image)
2. Double-click on the downloaded file
3. Click “Import Virtual Machine”
4. Wait for the import to finish (It may take some time.)
5. You can run your virtual machine

![unnamed](images/3.png)

</details>

<details>
<summary><strong>How to set up and launch</strong></summary>

**How to set up**

First, you can change the installation paths of virtual machines if you have several disks and you do not want to install a virtual machine on the system disk (this is the default path). To do this, do the following:

1. Open Hyper-V Manager
2. Right-click on the name of your computer:

![unnamed](images/4.png)

3. Select a location for storing virtual machine disks (you don’t need to change the other paths)

![unnamed](images/5.png)

> Warning! Check the presence of this check mark in the Hyper-V Manager settings 

![unnamed](images/6.png)

After importing the virtual machine, it will appear in the central window of the **Hyper-V** Manager program. To open this list, left-click on the name of your computer in the list on the left. The settings of the virtual machine are opened by right-clicking on it and clicking on the Settings item.

![unnamed](images/7.png)

> You can change the settings of a virtual machine only when it is turned off

On the **Memory ta**b, you can configure the amount of RAM available for the virtual machine:

![unnamed](images/8.png)

On the **Processor tab**, you can configure the number of available processor cores for a virtual machine

![unnamed](images/9.png)

Check that the **Enable checkpoints** checkbox is disabled:

![unnamed](images/10.png)

**How to launch**

Virtual machines start working in the background at startup. You can connect and disconnect to them, they will still continue to work. You can see the status of the virtual machine at the bottom of the application when you click on it:

![unnamed](images/11.png)

After the launch:

![unnamed](images/12.png)

Therefore, you can start a virtual machine by clicking on it and selecting **Start**. Then you can right-click and select **Connect** - you will connect to the VM. If you close the window, you can connect to the machine again by clicking **Connect**. To stop a virtual machine, you can click Shutdown in the Start menu of the virtual Windows or by clicking on the virtual machine and selecting **Stop**.

When connecting to a VM, you will see the enhanced mode settings window. With this mode, the virtual machine can interact with your PC. Click **Show Options**:

![unnamed](images/13.png)

Select the **Local Resources tab**, expand the **Drives list**, and select which of your disks you want to connect to the VM. You can also select a USB flash drive if it is currently connected to a PC. Or you can choose the Drives that i plug in later option. The selected disks will appear in the explorer in the virtual machine. This way you can download the recorded effects directly to your computer/USB.

![unnamed](images/14.png)

![unnamed](images/15.png)

> Before clicking the Connect button, you can return to the Display tab and select Save my settings for future connections to this virtual machine

![unnamed](images/17.png)

Now you can click the **Connect** button and start working in your virtual machine!

**Possible problems**
 1. If you have a small amount of RAM (8 GB or less), reduce the value of RAM available to the virtual machine (set 3072 or 2048). Just keep in mind that this will lead to a decrease in the performance of the virtual machine.
 2. If you encounter an error at startup about a lack of RAM, close background applications and/or reduce the available amount of RAM for the virtual machine.
 3. Virtual machines are resource-demanding, so it is not recommended to run them together with other “heavy” programs (browsers, various editors, etc.). 

If you have installed our virtual machine, then congratulations - you can already start creating effects! Proceed to the third step
   
</details>

---

##  Step 2 – Installing the Necessary Software 

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

##  Step 3 – Importing and Creating LED Effects 

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

##  Step 4 – Recording Your Effects 

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

##  Step 5 – Copying Effects to the Controller’s SD Card 

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

##  Common Problems 

<details>
<summary> My recorded effect flickers / freezes </summary>

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

##  Useful Links 

* [Full Knowledge Base](https://etereshop.zohodesk.com/portal/en/kb/articles/programming-of-led-effects-via-madrix)  
* [WinPcap Download](https://www.winpcap.org/install/default.htm)  
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)  
* [Madrix Tutorial Videos](https://www.youtube.com/@etereshop)  
* 📩 [Contact Support](mailto:sales@etereshop.com)

---
