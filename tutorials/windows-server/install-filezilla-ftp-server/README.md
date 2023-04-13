---
description: Learn how to install FileZilla's FTP server on your VPS or dedicated server!
---

# Install FileZilla FTP Server

FileZilla is a free and open-source FTP Manager Server/Client application. With this program, you can transfer the files you need from your computer to your host or server. And you can easily modify the access to your files.

FileZilla supports simultaneous sending of multiple files in parallel, support for dragging and dropping, and matching files are the features of this program.

{% hint style="info" %}
This guide only applys to FileZilla Server version 1.0 or higher.\
For previous versions see our guide [here](filezilla-v0.9.md).
{% endhint %}

## Video Tutorial

[Watch our video tutorial on installing a FileZilla FTP server.](https://www.youtube.com/watch?v=lspNUtwLfrE)

## Install FileZilla FTP Server

### 1. Download the FTP Server

First, [remote to your server](../remote-desktop-access/), and from the below link, download the server version of this software.

[https://filezilla-project.org/download.php?type=server](https://filezilla-project.org/download.php?type=server)

![](<../../../.gitbook/assets/image (113).png>)

### 2. Install

In the first step, agree to the terms and choose **I Agree** if you agree!

![](<../../../.gitbook/assets/image (5).png>)

Check the components that you wish to be installed and choose **Next**.

![](<../../../.gitbook/assets/image (125).png>)

The next window will ask for the installation directory, you can leave this as the default and click **Next** again. The same will be true for the start menu window that follows, simply click **Next** until you receive the next window as pictured below...

### 3. Configure

Now, in this section, it asks 3 questions.

1. The first one is how the FileZilla server should be started that we recommend putting it on the default option. Leaving the checkmark to start the server after the installation process is complete is also recommended.
2. The second question is to choose a port number for the FileZilla by which it will be used to administrate the server with the FileZilla server interface.

You can choose an amount between **1** to **65535**. You can choose any free port number on your server.

{% hint style="warning" %}
This is not the FTP port used by FTP clients. Do **NOT** set this port as 21 as that will be in use for FTP clients.
{% endhint %}

3\. The third one is to set your administrative password to manage the FileZilla Server. Please choose a memorable password that is secure. We suggest mixing a combination of uppercase letters, lowercase letters, numbers and symbols.

![](<../../../.gitbook/assets/image (154).png>)

On the next step, choose how the interface of the server should be started and click **Install**.

![](<../../../.gitbook/assets/image (4).png>)

### 4. Open FileZilla

Once it was opened, click `Connect to FileZilla FTP Server`.

![](<../../../.gitbook/assets/image (46).png>)

A smaller window will prompt you for your administrative password. Enter you password then click **Ok** to administrate the FTP server.

![](<../../../.gitbook/assets/image (69).png>)

You will get a notice the first time connecting to your FTP server asking to trust the signature of the server. Click **Yes** to proceed.

![](<../../../.gitbook/assets/image (22).png>)

### 5. Create a User

Now you need to create at least one username and define a folder. To do this, click on the `Server` tab > then choose `Configure`.&#x20;

![](<../../../.gitbook/assets/image (75).png>)

This will open the configuration window. Click `Users` on the left sidebar, then click `Add` at the bottom left to add a new user. You will be able to set the username of the user as seen in the top left.

![](<../../../.gitbook/assets/image (33).png>)

Check the Password checkbox and type a secure password of at least **8 characters** and has a combination of uppercase letters, lowercase letters, numbers and symbols. Then click **Apply** at the bottom right of the window.

![](<../../../.gitbook/assets/image (62).png>)

### 6. Assign Shared Folders

To assign one or more folders to this user first you must have the server file path. Open Windows Explorer and navigate to the folder you would like to make accesible from your FTP server. Copy the file path at the top of the Windows Explorer window.

![](<../../../.gitbook/assets/image (65).png>)

Click in the `Virtual path` field and enter a name that will be displayed when connecting to your FTP server. The name should have a "/" before the name. Then paste your server file path in the `Native path` field. If you want to allow files to be written click the `Writeable` checkbox. Save your shared folder settings by clicking `Apply` at the bottom right.

![](<../../../.gitbook/assets/image (3).png>)

### 7. Open FTP port in the firewall

#### A: Open Port 21

Note that you will have to allow the FTP port `21` in the firewall. Please check our [guide on how to open ports here](../opening-ports.md).&#x20;

#### B: Open the Firewall

Additionally, you will need to add a second firewall rule for the FileZilla Server EXE file. This will allow FileZilla to listen on additional ports for transfers once users are connected. Our [firewall guide](../opening-ports.md) goes over both inbound port rules and EXE rules.

### Having Trouble?

Our support team is happy to help! [Reach out to us at any time](https://support.sonoransoftware.com).
