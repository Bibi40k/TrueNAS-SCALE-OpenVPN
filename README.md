# TrueNAS-SCALE-OpenVPN-server-install

![Test](https://github.com/Bibi40k/TrueNAS-SCALE-OpenVPN/workflows/Test/badge.svg)
![Lint](https://github.com/Bibi40k/TrueNAS-SCALE-OpenVPN/workflows/Lint/badge.svg)
![visitors](https://visitor-badge.glitch.me/badge?page_id=Bibi40k.TrueNAS-SCALE-OpenVPN)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/Bibi40k)

OpenVPN installer for TrueNAS SCALE (Debian).

This script will let you setup your own secure VPN server in just a few seconds.

## Usage

First, get the script and make it executable:

```bash
curl -O https://raw.githubusercontent.com/Bibi40k/TrueNAS-SCALE-OpenVPN/master/install-openvpn-server.sh
chmod +x install-openvpn-server.sh
```

Then run it:

```sh
./install-openvpn-server.sh
```

You need to run the script as root.

The first time you run it, you'll have to follow the assistant and answer a few questions to setup your VPN server.

When OpenVPN is installed, you can run the script again, and you will get the choice to:

- Add a client
- Remove a client
- Uninstall OpenVPN

In your home directory, you will have `.ovpn` files. These are the client configuration files. Download them from your server and connect using your favorite OpenVPN client.

If you have any question, head to the [FAQ](#faq) first. Please read everything before opening an issue.

**PLEASE do not send me emails or private messages asking for help.** The only place to get help is the issues. Other people may be able to help and in the future, other users may also run into the same issue as you. My time is not available for free just for you, you're not special.

## Fork

This script is based on the great work of [angristan and its contributors](https://github.com/angristan/openvpn-install).

## Say thanks

You can [say thanks](https://saythanks.io/to/Bibi40k) if you want!

## Credits

Many thanks to the [contributors](https://github.com/Angristan/OpenVPN-install/graphs/contributors) and Nyr's original work.
