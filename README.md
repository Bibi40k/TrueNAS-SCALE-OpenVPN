# TrueNAS-SCALE-OpenVPN-server-install
![visitors](https://visitor-badge.glitch.me/badge?page_id=Bibi40k.TrueNAS-SCALE-OpenVPN)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/Bibi40k)

OpenVPN installer for TrueNAS SCALE (Debian).

This script will let you setup your own secure VPN server in just a few seconds.

## Usage

First, get the script and make it executable:

```bash
cd
curl -O https://raw.githubusercontent.com/Bibi40k/TrueNAS-SCALE-OpenVPN/master/install-openvpn-server.sh
chmod +x install-openvpn-server.sh
```

Then run it with sudo privileges:

```bash
sudo ./install-openvpn-server.sh
```

The first time you run it, you'll have to follow the assistant and answer a few questions to setup your VPN server.

When OpenVPN is installed, you can run the script again, and you will get the choice to:

- Add a client
- Revoke a client
- Uninstall OpenVPN

In your home directory, you will have `<client_name>.ovpn` files. These are the client configuration files. Download them from your server and connect using your favorite OpenVPN client.

**PLEASE do not send me emails or private messages asking for help.** The only place to get help is the issues. Other people may be able to help and in the future, other users may also run into the same issue as you.

## Fork & credits

This script is based on the great work of [angristan and its contributors](https://github.com/angristan/openvpn-install) and [Nyr and its contributors](https://github.com/Nyr/openvpn-install).

## Say thanks

You can [say thanks](https://saythanks.io/to/Bibi40k) if you want.

## TrueNAS SCALE useful related commands
```bash
systemctl status openvpn-server@server # view TrueNAS SCALE native OpenVPN server status
cat /etc/openvpn/server/server.conf # view TrueNAS SCALE native OpenVPN server config file

systemctl status openvpn@server # view custom (installed by scrypt) OpenVPN server status
cat /etc/openvpn/server.conf # view custom (installed by scrypt) config file

systemctl list-units --type=service --state=running | grep openvpn # view all running services named "openvpn"
```
