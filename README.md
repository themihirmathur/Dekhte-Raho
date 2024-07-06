# Dekhte Raho 👁️ | User Session Monitor 🖥️

`Dekhte Raho` is a robust Windows service designed to enhance security and manage resource allocation efficiently by terminating specified processes when a user's Windows session is disconnected. This tool is particularly useful in shared environments, such as corporate offices or public terminals, where managing system resources and maintaining security is crucial.

![Screenshot 2024-07-06 at 5 10 17 PM](https://github.com/themihirmathur/Dekhte-Raho/assets/92594107/b6fb354c-a52b-4d2a-bdc5-d8e9332f4b38)

## Features

- **Automated Process Termination**: Automatically kills specified processes when the user's session is disconnected.
- **Configurable Grace Period**: Allows configuration of a grace period after the session lock before terminating processes.
- **Resource Management**: Frees up system resources by terminating unused processes.
- **Security Enhancement**: Enhances security by ensuring no sensitive processes remain running in a user's absence.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Installation Instructions

### Prerequisites
- Administrator privileges on the Windows machine.

### Steps

1. **Download the Installation Archive**
   - Download the `SessionMonitor.zip` file and save it to a local folder.

2. **Unblock the Installation Archive**
   - Right-click on `SessionMonitor.zip` and select `Properties`.
   - Check the box next to `Unblock` and click `OK`.

3. **Extract the Installation Archive**
   - Extract the contents of `SessionMonitor.zip` to your desired folder.

4. **Install the Service**
   - Open the Command Prompt with Administrator privileges.
   - Navigate to the folder containing the extracted files.
   - Run the command `Install` to install the Dekhte Raho service.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Configuration

After installation, you can configure the service to specify which processes to monitor and the grace period before termination. The configuration file is located in the installation directory.

1. **Edit the Configuration File**
   - Open `config.json` in a text editor.
   - Specify the processes to monitor in the `processes` array.
   - Set the `gracePeriod` in seconds.

Example `config.json`:
```json
{
  "processes": ["notepad.exe", "calc.exe"],
  "gracePeriod": 300
}
```

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Usage

Once installed and configured, the Dekhte Raho service will run in the background. When a user locks their session, the service will wait for the specified grace period. If the session remains locked beyond this period, the specified processes will be terminated. If the user unlocks the session before the grace period ends, no action is taken.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Uninstallation

To uninstall the Dekhte Raho service, follow these steps:

1. **Open Command Prompt as Administrator**
2. **Navigate to the Installation Folder**
3. **Run the Uninstall Command**
   ```sh
   Uninstall
   ```

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Support

For any issues, feedback, or feature requests, please contact support at support@dekhteraho.com.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Contributing

We welcome contributions from the community. To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

---

Dekhte Raho is a powerful tool for managing processes in a Windows environment, ensuring security, and optimizing resource use. Install it today to keep your system secure and efficient!

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>
