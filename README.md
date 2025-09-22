# Track8
8 Track Hardware Arranger

We’re excited to have you here! 🎉  
Please use this repository for contributions, discussions, and ideas regarding Track8.  

To ensure a friendly and collaborative environment, please follow these guidelines:

- Be respectful and constructive in all discussions.  
- Keep communication clear and on-topic.  
- Avoid offensive, discriminatory, or inappropriate language.  
- Report issues responsibly and with enough context for others to help.  

---

# Submitting Bug Reports & Issues

If you encounter a problem with the Track8, please let us know by opening an issue on GitHub.  
Before submitting, please:

1. **Search existing issues**  
   Check the [Issues page](https://github.com/ThingstoneGmbH/Track8/issues) to see if the bug has already been reported.

2. **Prepare details**  
   Include as much relevant information as possible:
   - A clear description of the problem  
   - Steps to reproduce the issue  
   - Expected vs. actual behavior    
   - Screenshots or logs, if applicable  

3. **Create a new issue**  
   - Go to the [New Issue page](https://github.com/ThingstoneGmbH/Track8/issues/new)  
   - Fill in the details and submit  

---

# Feature Requests & Suggestions

We welcome ideas for improvements!  
Please open an issue labeled **Feature Request** with:
- A description of the new feature  
- Why it would be useful  
- Any examples or references  

---

# Code of Conduct

By participating in this project, you agree to uphold the standards of our [Code of Conduct](CODE_OF_CONDUCT.md).  



# Track8 Application Update

Follow these steps to update the **Track8 Application**.  
(For instructions on how to access the internal SSD, see **page 34** of the main manual.)

---

## Steps to Update

1. **Download the Application**  
   Go to the [Track8 Releases page](https://github.com/ThingstoneGmbH/Track8/releases) and download the latest release.

2. **Unzip the Downloaded File**  
   Extract the contents of the `.zip` file on your computer.

3. **Copy the New File**  
   - Locate the extracted `track8` file.  
   - Copy it to the **TRACK8 Drive** → `bin` folder.  
   - Overwrite the existing file when prompted.

4. **Safely Unmount the TRACK8 Drive**  
   Eject the drive using your operating system’s safe removal procedure.

5. **Disconnect the Cable**  
   Pull the **USB-C to USB-A cable** from the device.

6. **Restart**  
   Track8 will automatically restart with the updated application.

---

## Notes
- Ensure you have write access to the **TRACK8 Drive**.  
- Do not interrupt the process while copying or unmounting the drive.  
- After restart, confirm the update by checking the application version in the Track8 interface.


# Resetting the Base System

If **Track8** is unable to boot, or if a major update requires a reset, follow these steps carefully.

---

## Steps to Reset

1. **Download the Base System**  
   Get the latest `track8-base-system-x_x_x.img.zip` from the [Track8 Releases page](https://github.com/ThingstoneGmbH/Track8/releases).

2. **Download and Install Raspberry Pi Imager**
   - Visit the [Raspberry Pi Software page](https://www.raspberrypi.com/software/)  
   - Download the installer for your operating system  
   - Install and open the Raspberry Pi Imager  

3. **Connect Track8 to Your PC**  
   Plug in the **USB-C to USB-A cable** between Track8 and your computer.

4. **Enter Reset Mode**  
   Hold down the **RST Button** on Track8 using a paper clip.

5. **Choose Base System**  
   - In Raspberry Pi Imager, click **"Use Custom"**  
   - Select the downloaded `track8-base-system-x_x_x.img.zip` file

6. **Choose Storage Device**  
   - Click **"Choose Storage"**  
   - Select `mmcblk0p1`
     
7. **Wait until finished**

8. **Safely Unmount the Drive**  
   Eject the **TRACK8 Drive** safely using your operating system’s removal procedure.

9. **Power Down Track8**  
   Turn off Track8 and wait until the **Power light** is fully off.

19. **Disconnect the Cable**  
   Remove the **USB-A cable** from your PC.

11. **Restart Track8**  
    Power Track8 back on. The system will boot from the restored base system.

---

## Notes
- Do not interrupt the ISO restore process.  
- Make sure to select the correct disk (**bootfs**) in Disk Utility.  
- After restart, Track8 should boot into a fresh base system.

