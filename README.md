Ω OmegaOS

A sovereign Linux distribution built for Africa.



</div>

OmegaOS is a custom Linux distribution engineered for deployment in resource-constrained environments across sub-Saharan Africa. Built on Ubuntu 24.04 Noble Numbat, it is designed to run on aging hardware, operate completely offline, and serve communities where connectivity and software costs are barriers to computing.


Download

Get the ISO from the Internet Archive:

🔗 https://archive.org/details/omega-final_202606

On the Archive page, click the ISO IMAGE link under the download options on the right side. The file is a standard bootable .iso.


Running OmegaOS in VMware

The recommended way to try OmegaOS is inside a virtual machine using VMware Workstation Player (free) or VMware Workstation Pro. This lets you run OmegaOS on your existing Windows or Linux machine without changing anything on your system.

What you need


VMware Workstation Player — free for personal use
The OmegaOS .iso file downloaded from the link above
At least 2 GB of RAM and 15 GB of free disk space to allocate to the VM



Step 1 — Create a new virtual machine


Open VMware Workstation Player and click Create a New Virtual Machine
Select Installer disc image file (ISO) and browse to the OmegaOS .iso you downloaded
When asked to select a guest OS, choose Linux → Ubuntu 64-bit
Give your VM a name (e.g. OmegaOS) and choose where to save it
Set the disk size to at least 15 GB — select Store virtual disk as a single file
Click Finish



Step 2 — Configure VM resources (recommended)

Before starting the VM, click Edit virtual machine settings and adjust:

SettingRecommended ValueMemory (RAM)2048 MB (2 GB)Processors2 coresDisplayEnable 3D acceleration (optional)

OmegaOS is built to run on low resources, so even 1 GB RAM will work — but 2 GB gives a smoother experience.


Step 3 — Boot and install


Click Play virtual machine — OmegaOS will boot from the ISO
At the boot menu, select Try or Install OmegaOS
Once the desktop loads, double-click the Install OmegaOS icon
Follow the installer prompts:

Select your language and timezone
For disk setup, choose Erase disk and install OmegaOS — this only affects the virtual disk, not your real machine



Complete installation and click Restart Now
When prompted to remove the installation medium, go to VM → Removable Devices → CD/DVD → Disconnect, then press Enter


OmegaOS will boot into your freshly installed system.


First Boot

On your first login you'll be greeted by the OmegaOS Welcome App, which introduces the system and walks you through what's available. After that:


The Hardware Optimizer will auto-detect your virtual CPU and RAM and tune performance accordingly — no manual configuration needed
Open Omega Learn from the desktop or applications menu to start learning Linux and cybersecurity fundamentals, completely offline
If you're on a metered connection, enable Low Bandwidth Mode from the taskbar to throttle background data usage



Features

Included out of the box


Hardware Optimizer — auto-detects RAM and CPU, tunes the system for low-spec and virtual environments so performance is always maximized for your hardware
Omega Learn — built-in offline learning platform covering Linux fundamentals and cybersecurity basics, designed for users with no prior Linux experience and no need for an internet connection
Low Bandwidth Mode — throttles background data to conserve costs on metered or limited connections
LibreOffice Suite — full office suite (Writer, Calc, Impress) that works completely offline. No subscription, no activation, no cracking required.
XFCE Desktop Environment — lightweight, fast, and stable desktop that stays responsive even on minimal resources
XFCE Settings Manager — simple controls for WiFi, Bluetooth, Display, and Sound
OmegaOS Welcome App — custom first-boot experience with Axoryn branding to orient new users
Yaru Dark theme — dark mode by default with a custom OmegaOS wallpaper


Coming soon


AI Terminal Assistant — a lightweight, low-resource AI assistant embedded in the terminal to help users run commands, understand errors, and navigate the system — especially useful for those new to Linux



Troubleshooting

VM is very slow or laggy
Increase RAM allocation to at least 2 GB in VMware settings. Also ensure VMware Tools is installed — after booting, go to VM → Install VMware Tools and follow the prompts inside the guest.

Black screen after booting the ISO
In VMware settings, go to Display and disable 3D acceleration, then try again. This is a common issue with some graphics configurations.

No internet inside the VM
VMware defaults to NAT networking which should work automatically. If not, go to VM → Settings → Network Adapter and switch to NAT, then restart the VM.

LibreOffice won't open a file
LibreOffice supports .docx, .xlsx, .pptx, .pdf, .odt and more. If a file opens blank, try: File → Reload.

Omega Learn won't launch
Open a terminal and run:

bashomega-learn

If it returns an error, run sudo apt install omega-learn to reinstall it.


About

OmegaOS is built and maintained by Axoryn Robotics — a student-led technology initiative from Zimbabwe focused on building sovereign infrastructure for African communities.


"Built for Africa. By Africa."




Links


📦 Download ISO — Internet Archive
💻 Source Code — GitHub
🌍 Built on Ubuntu 24.04 Noble Numbat



<div align="center">
Made with ❤️ in Zimbabwe 🇿🇼
</div>
