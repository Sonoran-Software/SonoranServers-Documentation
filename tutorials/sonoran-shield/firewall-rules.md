---
description: >-
  Sonoran Shield allows you to easily lock down unused ports, restrict access
  based on IPs, and more!
---

# Firewall Rules

Open and unused ports represent potential security vulnerabilities. Attackers can exploit open ports to gain unauthorized access to a system, take down your server through denial of service attacks (DoS/DDoS) and compromise its security. By blocking unused ports, organizations can reduce their attack surface and minimize the risk of a successful attack. It is a best practice to only allow traffic on necessary ports to limit potential vulnerabilities and maintain the security of the system.

Sensitive ports can be limited to only authorized source IP addresses (your developers for example) to limit attack surface further while allowing access to authorized users.

## Getting Started with Firewall Rules

<figure><img src="../../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>

### 1. Block all Unused Ports

The first rule will block access on all unused ports. After this, we will add rules to open only the ports we need.

* Select `New Rule`
* Add your server's IP address in the `Destination` drop-down
* Select `Network` as the `Source Type`
* Set the `Source IP` to `0.0.0.0/0`
* Leave the `Protocol`, `Source Port`, and `Destination Port` fields blank
* Set the `Action` to `Block`
* Save the new rule

<figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

### 2. Add a port for RDP

Next, we will want to open up a port for remote desktop connections. This will allow us to use Window's RDP to view/manage our server.

* Select `New Rule`
* Add your server's IP address in the `Destination` drop-down
* Select `Network` as the `Source Type`
* Set the `Source IP` to:
  * Allow any IP: `0.0.0.0/0`
  * Or, allow only your specific IP address to connect
* Set `Protocol` to `TCP`
* Set the `Destination Port` to 3389
  * This is the default RDP port for Windows servers
* Leave the `Destination Port` field blank
* Set the `Action` to `Allow`
* Save the new rule

Continue this process to open additional ports for your game server and any other applications.

<figure><img src="../../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>
