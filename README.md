# Cisco Packet Tracer Installation Guide for Ubuntu

## Overview

Cisco Packet Tracer is a powerful network simulation tool developed by Cisco for learning networking concepts, creating network topologies, and practicing Cisco certifications.

Before downloading Packet Tracer, create a free account on Cisco Networking Academy (NetAcad). This account gives you access to Packet Tracer downloads, tutorials, and networking courses.

---

## Step 1: Update Your Ubuntu System

Open Terminal and run:

```bash
sudo apt update
sudo apt upgrade -y
```

---

## Step 2: Download Cisco Packet Tracer

Download the latest Packet Tracer `.deb` package from Cisco Networking Academy.

After downloading, save the file in your **Downloads** folder.

---

## Step 3: Install the .deb Package
Use the dpkg command to install Cisco Packet Tracer:

# modify the file name with you file name
sudo dpkg -i CiscoPacketTracer822_amd64_signed.deb
Agree Software License Agreement
<img width="1210" height="787" alt="image" src="https://github.com/user-attachments/assets/b3671d43-5968-4d79-9278-3a1ee656c64b" />

Accept EULA
<img width="1210" height="787" alt="image" src="https://github.com/user-attachments/assets/7e00cda3-68a7-459e-8e80-4de9d6905920" />

if installed with no errors then Congratulations! skip to step 6

---

## Step 4: Resolve Missing Dependencies
If there are missing dependencies, you need to install them manually. For example, if you encounter an error related to libgl1-mesa-glx and libxcb-xinerama0-dev, you can install the missing package using:
<img width="1173" height="631" alt="image" src="https://github.com/user-attachments/assets/e90cef5a-f347-4de4-80ef-8dfc6c3d192d" />

sudo apt-get install libgl1-mesa-glx libxcb-xinerama0-dev

If the packages are installed sucessfully then try to install Cisco Packet Tracer again.

# modify the file name with you file name
sudo dpkg -i CiscoPacketTracer822_amd64_signed.deb

if the packages are not being installed then use the following links to download manually
Example Image

 <img width="1239" height="331" alt="image" src="https://github.com/user-attachments/assets/8f56f6a8-ab59-41f0-8961-ebfc1ade81a2" />

 Download Missing Ubuntu Packages
 https://ubuntu.pkgs.org/

 Select you distribution and then search for the package that is missing in the search
Click on the below image to watch tutorial to download packages manually or Download Video


https://www.youtube.com/watch?v=rc2scAhX6mc

Download the packages with amd64 on your device and Use the dpkg command to install the missing packages

# Replace the package name with your package name
sudo dpkg -i libxcb-xinerama0-dev_1.15-1ubuntu2_amd64.deb
# Replace the package name with your package name
sudo dpkg -i libgl1-mesa-glx_22.3.6-1+deb12u1_amd64.deb

5. Fix Remaining Dependencies
After manually installing all required packages, run the following command to automatically fix any remaining issues:

sudo apt-get install -f
This command will resolve any remaining unmet dependencies and finalize the installation of Cisco Packet Tracer.

6. Verify Installation
Once all dependencies are resolved, verify the installation by launching Cisco Packet Tracer from the terminal:

packettracer
Login in your account to start using Cisco Packet Tracer
Also Toggle On "keep me logged in" button to stay logged in for 3 months

<img width="3445" height="1515" alt="image" src="https://github.com/user-attachments/assets/d15a70a7-c7e9-42ee-9950-6c03146e9e19" />

After clicking on Cisco Skills For All and login to your account

If everything is installed correctly, Cisco Packet Tracer should launch successfully.

<img width="1200" height="675" alt="image" src="https://github.com/user-attachments/assets/aa5bee4e-8726-4f48-9d2e-f14f1dcbd40d" />

support

If you found this helpful, consider giving it a ⭐ and following me on GitHub for more cool things!

)__________________________________________________________________________________________________________________))))))

<b>this is step 3 <b/>

```

During installation:

* Accept the Software License Agreement.
* Accept the End User License Agreement (EULA).
* Continue the installation process.

If the installation completes successfully, proceed to Step 6.

---

## Step 5: Fix Missing Dependencies

If Ubuntu reports missing dependencies, install them using:

```bash
sudo apt-get install libgl1-mesa-glx libxcb-xinerama0-dev
```

Then try installing Packet Tracer again:

```bash
sudo dpkg -i CiscoPacketTracer822_amd64_signed.deb
```

### Manual Dependency Installation

If required packages are unavailable from the repository, download the appropriate **amd64** package files and install them manually:

```bash
sudo dpkg -i libxcb-xinerama0-dev_*.deb
sudo dpkg -i libgl1-mesa-glx_*.deb
```

After installing the packages, run:

```bash
sudo apt-get install -f
```

This command automatically resolves any remaining dependency issues.

---

## Step 6: Verify Installation

Launch Cisco Packet Tracer:

```bash
packettracer
```

If the installation was successful, Cisco Packet Tracer will open.

---

## Login to Packet Tracer

1. Open Cisco Packet Tracer.
2. Select **Cisco Skills For All**.
3. Sign in using your Cisco Networking Academy account.
4. Enable **Keep Me Logged In** for easier access.

You can now start creating and testing network topologies.

---

## Troubleshooting

### Packet Tracer Does Not Launch

Try:

```bash
sudo apt-get install -f
```

Then restart the application.

### Missing Library Errors

Install missing libraries using:

```bash
sudo apt install <package-name>
```

Replace `<package-name>` with the package reported in the error message.

---

## Support

If this guide helped you, consider giving this repository a ⭐.

Feel free to explore my GitHub profile for more Linux, Networking, and Computer Science resources.
