---
description: Learn how to install FileZilla's FTP server on your VPS or dedicated server!
---

# FileZilla v0.9 Install Guide

FileZilla is a free and open-source FTP Manager Server/Client application. With this program, you can transfer the files you need from your computer to your host or server. And you can easily modify the access to your files.

FileZilla supports simultaneous sending of multiple files in parallel, support for dragging and dropping, and matching files are the features of this program.

## Video Tutorial

[Click here to watch our video tutorial on installing FileZilla!](https://youtu.be/qj\_jZKcR\_9A)

## Install FileZilla FTP Server

### 1. Download the FTP Server

First, [remote to your server](../remote-desktop-access/), and from the below link, download the server version of this software.

[https://filezilla-project.org/download.php?type=server](https://filezilla-project.org/download.php?type=server)

![](<../../../.gitbook/assets/image (85).png>)

### 2. Install

In the first step, agree to the terms and choose **I Agree** if you agree!

![](<../../../.gitbook/assets/image (5).png>)

Check the components that you wish to be installed and choose **Next**.

![](<../../../.gitbook/assets/image (138).png>)

### 3. Configure

Now, in this section, it asks for 3 questions.

1. The first one is how the FileZilla server should be started that we recommend putting it on the default option.&#x20;
2. The second question is to choose a port number for the FileZilla by which it will be used to administrate the server with the FileZilla server interface.

You can choose an amount between **1** to **65535**. You can choose any free port number on your server.

{% hint style="warning" %}
This is not the FTP port used by FTP clients. Do **NOT** set this port as 21 as that will be in use for FTP clients.
{% endhint %}

3\. The third one is to check or uncheck the option “Start server after setup completes”.

![](<../../../.gitbook/assets/image (8).png>)

On the next step, choose how the interface of the server should be started and click **Install**.

![](<../../../.gitbook/assets/image (70).png>)

### 4. Open FileZilla

Once it was opened, a pop screen will be shown. Click Connect to administrate.

![](<../../../.gitbook/assets/image (143).png>)

### 5. Create a User

Now you need to create at least one username and define a folder. To do this, click on the `Users` option > Choose `Edit` > `Users` > `add` to add a new user > Check the `Password` box and choose a secure password with at least **8** characters.

![](<../../../.gitbook/assets/image (38).png>)

### 6. Assign Shared Folders

To assign one or more folders to this user, choose `Shared folders`**,** and click `Add`. Next to the shared folders that you chose, also set the accesses that you wish to assign for this new user and click ok.

![](<../../../.gitbook/assets/image (52).png>)

### 7. Open FTP port in the firewall

#### A: Open Port 21

Note that you will have to allow the FTP port `21` in the firewall. Please check our [guide on how to open ports here](../opening-ports.md).&#x20;

#### B: Open the Firewall

Additionally, you will need to add a second firewall rule for the FileZilla Server EXE file. This will allow FileZilla to listen on additional ports for transfers once users are connected. Our [firewall guide](../opening-ports.md) goes over both inbound port rules and EXE rules.

### Having Trouble?

Our support team is happy to help! [Reach out to us at any time](https://support.sonoransoftware.com).
