---
description: Learn how to open additional ports on your Windows server.
---

# Opening Ports/Firewall Rules

## Video Tutorial

[Click here to watch our video tutorial on opening firewall ports!](https://www.youtube.com/watch?v=qj\_jZKcR\_9A\&t=2s)

## Getting Started

To open any port within Windows you need to use the Windows Defender Firewall. To get started gather a list of all TCP + UDP ports and whether they're Inbound or Outbound. Once you've gathered your ports you're going to want to:

* Hit your Windows Start Button
* Search for "Windows Defender Firewall with Advanced Security" and click on it.

### Inbound Port Rules

* Right-click on Inbound Rules.

![Rule Type](<../../.gitbook/assets/image (97) (1).png>)

* Click "**New Rule**".
* Click "**Port**" and select Next.
* Depending on what you've gathered for the information you can select TCP or UDP. For this example, we will be opening TCP Port `40125` and `40126`.

![Port Type and Ports](<../../.gitbook/assets/image (14).png>)

* We would select TCP for the Port type. We would click "**Specific local ports**" and enter `40125, 40126`. If you are doing just one port you don't need the comma. After entering the required information hit **Next**.
* You will want to ensure "**Allow the connection**" has been selected and then hit **Next**.
* `Domain`, `Private`, and `Public` should also be selected. Click **Next**.
* Give this rule a Name and Description relative to the application. Click **Finish**.&#x20;



### Inbound Program Rules (EXE)

* Right-click on **Inbound Rules**.

![Rule Type](<../../.gitbook/assets/image (97) (1).png>)

* Click "**New Rule**".
* Click "**Program**" and select **Next**.
* Click the "**Browse...**" button, and navigate to the EXE that you would like to allow inbound connections to, then select **Next**.

![Browse for the program you want to allow inbound connections to](<../../.gitbook/assets/image (129).png>)

* In this example, we are allowing the FileZilla Server.exe.
* You will want to ensure "**Allow the connection**" has been selected and then hit **Next**.
* `Domain`, `Private`, and `Public` should also be selected. Click **Next**.
* Give this rule a Name and Description relative to the application. Click **Finish**.&#x20;

### Outbound Port Rules

{% hint style="warning" %}
By default Windows Server allows most outbound connections. You rarely need to add a firewall rule in the outbound category...
{% endhint %}

* Right-click on **Outbound Rules**.

![Rule Type](<../../.gitbook/assets/image (50).png>)

* Click "**New Rule**".
* Click "**Port**" and select **Next**.
* Depending on what you've gathered for the information you can select TCP or UDP. For this example, we will be opening TCP Port `40125` and `40126`.

![Port Type and Port](<../../.gitbook/assets/image (14).png>)

* We would select TCP for the Port type. We would click "**Specific local ports**" and enter `40125, 40126`. If you are doing just one port you don't need the comma. After entering the required information hit **Next**.
* You will want to ensure "**Allow the connection**" has been selected and then hit **Next**.
* `Domain`, `Private`, and `Public` should also be selected. Click **Next**.
* Give this rule a Name and Description relative to the application. Click **Finish**.&#x20;
