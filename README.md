<base target="_blank">

<div dir="ltr">



[**![Lang_farsi](https://user-images.githubusercontent.com/125398461/234186932-52f1fa82-52c6-417f-8b37-08fe9250a55f.png) &nbsp;فارسی**](README_fa.md)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</div>
<br>
<div align=center markdown="1">
 

![Hiddify Logo](https://user-images.githubusercontent.com/125398461/227777845-a4d0f86b-faa2-4f2b-a410-4aa5f68bfe19.png)

</div>

# Hiddify Relay builder
This script provides you with the following methods to create a tunnel between a relay server and your main server.

`1. IP Tables`

`2. GOST`

`3. Xray-Dokodemo`

`4. HA-Proxy`

`5. Socat`

## ⚙️ Installation
In order to create tunnels on your relay server, you just need to run the following command.

```
bash -c "$(curl -L https://raw.githubusercontent.com/hiddify/hiddify-relay/main/install.sh)"
```
<div align=center>

 <img src="https://github.com/hiddify/hiddify-relay/assets/125398461/50bc6374-56b4-4eba-866e-c006e123435f" alt="Relay-builder Menu" width=30% />
</div>

### 🛠️ IP-Tables Tunnel
According to the 1st picture above, choose number `1` and enter the `IPTables menu` to manage `IPTables tunnel`:

<div align=center>

 ![IP-Tables Tunnel Menu](https://github.com/hiddify/hiddify-relay/assets/125398461/ddd9cf12-3d5c-4aab-9b36-278395c3cbfb)
 
</div>

`1. Install iptables rules`

After selecting the number `1` in the `IPTables Menu`, it asks you to enter the IP address of the main server and press `Enter` button to activate the tunnel on ports `443` and `80`.

`2. Check ports in use`
This option shows you the ports used in the IPTables tunnel.

`3. Uninstall iptables rules`
This option clears all rules created for the tunnel and all other rules.

> [!NOTE]
> Be careful that if you have created special rules next to the tunnel manually, they will be deleted with this command.

`4. Back to Main Menu`
In order to go back to the main menu press `4` .

### 🛠️ GOST Tunnel
According to the 1st picture above, choose number `2` and enter the `GOST menu` to manage `GOST tunnel`:

<div align=center>
 
![GOST Tunnel](https://github.com/hiddify/hiddify-relay/assets/125398461/afb47714-f566-4a24-a5c6-32b5c971927e)

</div>

`1. Install GOST`

After choosing number `1`, wait until the tunnel is installed. After the installation is complete, in the first step, you must enter the desired port for the tunnel and then press Enter. In the next step, enter the domain or subdomain of your main server, then press `Enter`. Wait until the tunnel should be started. After starting, the message `Gost install and enabled` will be displayed in green.

`2. Check GOST Port and Status`

After selecting option `2`, the ports used in the tunnel and the status of the tunnel will be displayed to you.

`3. Add Another Port and Domain`
- You can use this option if you want to tunnel from the relay server to several outside servers.
- After selecting the number `3`, you must enter the new port, press the `Enter` button, then enter the domain of the main server and press the `Enter` button.
- You can enter option number `2` to ensure that the previous steps are correctly done and to check the used ports and to see if the tunnel is activated.

`4. Uninstall GOST`

This option will remove the GOST tunnel from your relay server.

`5. Back to Main Menu`

In order to go back to the main menu press `5` .


### 🛠️ Dokodemo-door Tunnel
According to the 1st picture above, choose number `3` and enter the `Dekodemo-door Menu` to manage `Dokodemo-door tunnel`:

<div align=center>
 
![Dokodemo Tunnel](https://github.com/hiddify/hiddify-relay/assets/125398461/e8b92d4d-e60e-4526-9280-04d1aac6aa29)

</div>

`1. Install Xray and add inbound`
- After selecting number `1` in the Dokodemo-door tunnel menu, wait for the Xray kernel to be installed on the relay server.
- After installation, enter the `IP address` or the `domain` of the main server in the `address section`.
- in the next section enter the desired port of the tunnel (recommended: 443,80), then press the `Enter` button.
- The message `Inbound added and tunnel started` will be displayed.

`2. Check Xray Service Status`
After selecting option `2`, the ports used in the tunnel and the status of the tunnel will be displayed to you.

`3. Add another inbound`
- You can use option `3` in the Dokodemo-door tunnel menu to create another inbound connection and connect your relay server to several external servers.
- After selecting option `3`, in the `new address section`, enter the `IP address` or the `domain` of your new server, then press `Enter`.
- Next step, enter the new port in the `new port field` and press `Enter` button. You will see inbound added.
- You can enter option number `2` to ensure that the previous steps are correctly done and to check the used ports and to see if the tunnel is activated.


`4. Uninstall Xray and tunnel`
Choose this option to remove Dokodemo-door tunnel and Xray core from your relay server
`5. Back to Main Menu`
In order to go back to the main menu press `5`.

### 🛠️ HA-Proxy Tunnel
According to the 1st picture above, choose number `4` and enter the `HA-Proxy Menu` to manage `HA-Proxy tunnel`:

<div align=center>

 ![HA-Proxy Tunnel](https://github.com/hiddify/hiddify-relay/assets/125398461/4bc0ad31-64b0-4b80-99be-01bf472ec5d4)

</div>

`1. Install HA-Proxy`
- After selecting option `1`, wait for the installation of the HA-Proxy package.
- After installation, in the `Relay port section`, enter the desired port in your relay server (recommended port 443)
- Then enter the IP address of your main server in the Enter Main-Server IP field.
- Then, in the Enter Main-Server Port section, enter the port freed on your main and external server (e.g. by default, Hiddify Manager uses port 443, and it is recommended to use this port).
- After the correct operation, the message `HA-Proxy installed and active successfully!` will be displayed on the screen.

`2. Check HA-Proxy Ports and Status`
After selecting option `2`, the ports used in the tunnel and the status of the tunnel will be displayed to you.

`3. Uninstall HA-Proxy`
Use this option to remove HA-Proxy tunnel from the relay server.

`4. Back to Main Menu`
In order to go back to the main menu press `4`.


<div align=center>

<br>

[![Email](https://img.shields.io/badge/Email-contribute@hiddify.com-005FF9?style=flat-square&logo=mail.ru)](mailto:contribute@hiddify.com)
[![Telegram Channel](https://img.shields.io/endpoint?label=Channel&style=flat-square&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2Fhiddify&color=blue)](https://telegram.dog/hiddify)
[![Telegram Group](https://img.shields.io/endpoint?color=neon&label=Support%20Group&style=flat-square&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2Fhiddify_board)](https://telegram.dog/hiddify_board)
[![Youtube](https://img.shields.io/youtube/channel/views/UCxrmeMvVryNfB4XL35lXQNg?label=Youtube&style=flat-square&logo=youtube)](https://www.youtube.com/@hiddify)
[![Twitter](https://img.shields.io/twitter/follow/hiddify_com?color=%231DA1F2&logo=twitter&logoColor=1DA1F2&style=flat-square)](https://twitter.com/intent/follow?screen_name=hiddify_com)

</div>

<p align=center>
 We appreciate all people who are participating in this project. Some people here and many many more outside of Github. It means a lot to us. ♥
 </p>
 
<p align=center> 
<a href="https://github.com/hiddify/hiddify-relay/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=hiddify/hiddify-relay" />
</a>
</p>
<p align=center>
 Made with <a rel="" target="_blank" href="https://contrib.rocks">Contrib.Rocks</a> 
</p>
