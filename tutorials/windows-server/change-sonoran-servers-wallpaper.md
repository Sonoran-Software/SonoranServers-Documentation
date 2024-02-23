---
description: >-
  Learn how to remove the default wallpaper set on Sonoran Servers and set your
  own
---

# Change Sonoran Servers Wallpaper

Our Windows OS image uses a setting to set the default wallpaper on our servers and subsequently this blocks the ability to change it without removing the setting first. Please follow the steps below to remove this restriction and set a new wallpaper...

1. Download this batch script to your server, then rename the file to remove ".txt" from the name. The resulting name will be `removewallpaper.bat`

{% file src="../../.gitbook/assets/removewallpaper.bat.txt" %}
Sonoran Servers Remove Wallpaper batch script
{% endfile %}

2. If you don't see the .txt on the end of the file name, you may need to enable viewing file name extensions. Open File Explorer and click View -> and check the File name extensions option as pictured.

<figure><img src="../../.gitbook/assets/image (160).png" alt=""><figcaption><p>Enabling file name extension view setting in Windows</p></figcaption></figure>

2. Run the batch script as an administrator by right-clicking and selecting "run as administrator", then click "yes" to any prompts.
3. Once the script has run it will instruct you to log out and log in.
4. Once logging back in, you may set a new wallpaper by right-clicking a photo and choosing "set as wallpaper" or by right-clicking the desktop and clicking the "Personalization" option to open the wallpaper settings menu.
