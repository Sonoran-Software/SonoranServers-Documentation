# Troubleshooting Remote Desktop Protocol

## Add Firewall Rules for All Networks

Our install image is setup with Remote Desktop over the internet allowed but for some reason Windows tends to change the network type on reboot. You can resolve this by adding a firewall rule to allow Remote Desktop on Domain, Private and Public network types. Connect via [NoVNC](../../general/novnc-remote-access.md) from your Sonoran Servers customer portal and follow the steps below to add the rules. For instructions on NoVNC, visit our guide [here](../../general/novnc-remote-access.md).

1\. Press the “**Windows**” key and start typing **"Firewall with Advanced Security"**, then click the pictured result to open the Firewall Rule Control Panel.

![Click Firewall with Advanced Security](<../../../.gitbook/assets/image (92).png>)

2\. Click Incoming Rules in the top left of the window.

![Click Inbound Rules](<../../../.gitbook/assets/image (24).png>)

3\. On the right hand collumn, click "**New Rule...**".

![Click New Rule...](<../../../.gitbook/assets/image (123).png>)

4\. Click the bubble to change the new rule to a "**Predefined:**" type and select "**Remote Desktop**" from the drop down before clicking next.

![Select predefined](<../../../.gitbook/assets/image (72).png>)

5\. Select all the rules and click "**Next**".

![Select all rules from list](<../../../.gitbook/assets/image (147).png>)

6\. Keep clicking "**Next**" until the Wizard closes and successfully adds the new rules.

![New Firewall Rules](<../../../.gitbook/assets/image (29).png>)

7\. Try Remote Desktop Connection again.

## Restart Remote Desktop Services

Windows Remote Desktop Protocol sometimes runs into issues and most of the time is resolved with a service restart. You can connect via [NoVNC](../../general/novnc-remote-access.md) from your Sonoran Servers customer portal and restart the service within Windows. Follow the steps below once logged in to Windows over [NoVNC](../../general/novnc-remote-access.md). For instructions on NoVNC, visit our guide [here](../../general/novnc-remote-access.md).

1\. Press the “**Windows**” key and start typing **"Services"**, then click the pictured result to open the Services Control Panel.

![Click "Services"](<../../../.gitbook/assets/image (49).png>)

2\. Rick click on “**Remote** **Desktop** **Service**” and click on **“Restart”.**

![Services Control Panel: Restart "Remote Desktop Services"](<../../../.gitbook/assets/image (139).png>)

3\. Click **"yes"** on the prompt that pops up.

![Click "Yes"](<../../../.gitbook/assets/image (140).png>)

4\. **Check** to see if the issue persists.
