# ZBT-Z8102AX-M2
My OpenWrt SNAPSHOT / LuCI Main :: user friendly :: build for the Z8102AX-M2 (Z8102AX v01) router.

<p align="center">
<img src="https://github.com/4IceG/Personal_data/blob/master/developzbt.png?raw=true" />
</p>

![GitHub release (latest by date)](https://img.shields.io/github/v/release/4IceG/ZBT-Z8102AX-M2?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/4IceG/ZBT-Z8102AX-M2?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/4IceG/ZBT-Z8102AX-M2?style=flat-square)
![GitHub All Releases](https://img.shields.io/github/downloads/4IceG/ZBT-Z8102AX-M2/total)



### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> OpenWrt installation procedure / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Procedura instalacji OpenWrt

<details>
   <summary>Pokaż | Show me</summary>

- The purchased router has software provided by Zbtlink. | Zakupiony router posiada oprogramowanie dostarczone przez Zbtlink.

![](https://github.com/4IceG/ZBT-Z8102AX-M2/blob/main/ZBT%20to%20OpenWrt/zbt_firmware.jpg?raw=true)

- Installing new firmware. | Instalacja nowego firmware.
  
1. Fixed computer IP: 192.168.1.100, Subnet mask: 255.255.255.0
1. Turn off power and keep press the Reset button for a few seconds to connect to the power supply. Wait 20 seconds after connecting the power supply.
1. Enter the browser page and enter: 192.168.1.1
1. Submit the updated firmware [Z8102AX-nand-mt7981-DDR4-23.0804_121617.bin](https://github.com/4IceG/ZBT-Z8102AX-M2/blob/main/ZBT%20to%20OpenWrt/Z8102AX-nand-mt7981-DDR4-23.0804_121617.bin).
1. Wait for update to complete.
1. Enter the browser page and enter: 192.168.1.1
1. Submit the updated OpenWrt firmware.

  
</details>

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> What You Should Know / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Co powinieneś wiedzieć

+ #### Installation of additional packages / Instalacja dodatkowych pakietów
> Snapshots are built daily, and that sets time limits to installing new packages with opkg. Due to kernel version checksums, you can only install “kmod” kernel modules and other kernel version dependent modules from the exactly same snapshot build. So, a few hours after flashing the firmware you may not be able to install new modules with opkg any more (as the next snapshot has been built into the download repo and has different checksums).   
> Obrazy snapshots budowane są codziennie, a to ustawia limity czasowe na instalację nowych pakietów za pomocą opkg. Z powodu sum kontrolnych wersji jądra, możesz zainstalować tylko moduły "kmod" i inne moduły zależne od wersji jądra z dokładnie tego samego snapshotu. Tak więc, kilka godzin po flashowaniu firmware możesz nie być w stanie zainstalować nowych modułów za pomocą opkg (ponieważ następny snapshot został wbudowany w repo i ma inne sumy kontrolne).

+ #### User's own configuration / Konfiguracja przez użytkownika
> The user must configure on his own:
- wan connection/interface for the modem(s) (e.g. QMI/MBIM).
- set the LEDs (according to preferences)
- set up Wi-Fi/passwords
> Użytkownik musi skonfigurować we własnym zakresie:
- połączenie/interfejs wan dla modemu/modemów (np. QMI/MBIM)
- ustawić diody LED (wedle upodobań)
- skonfigurować Wi-Fi/hasła.

+ #### LuCI theme / Motyw LuCI
> Main theme: Bootstrap.   
> Główny motyw: Bootstrap.

+ #### My modifications / Moje modyfikacje
> I changed the miniDLNA, lan ports, wi-fi, signal levels icons.   
> Zmieniłem ikony dla miniDLNA, portów lan, wi-fi, poziomów sygnału.

+ #### Languages added to image / Języki dodane do obrazu
> Language packs: English and Polish. (I can add other languages, but this will require translating my packages / add-ons).   
> Pakiety językowe: angielski i polski. (Mogę dodać inne języki, ale będzie to wymagało przetłumaczenia moich pakietów/dodatków).

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> Screenshot / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Zrzut ekranu

![](https://github.com/4IceG/ZBT-Z8102AX-M2/blob/main/ZBT%20to%20OpenWrt/zbtlink.png?raw=true)

### Packages available in the image:
<details>
   <summary>Pokaż | Show me</summary>
   
``` bash
aria2 - 1.36.0-2
ariang - 1.3.2-1
base-files - 1542-r24056-86dadeba48
block-mount - 2023-02-28-bfe882d5-1
busybox - 1.36.1-1
ca-bundle - 20230311-1
ca-certificates - 20230311-1
cgi-io - 2022-08-10-901b0f04-21
chat - 2.4.9.git-2021-01-04-5
comgt - 0.32-35
comgt-ncm - 0.32-35
dnsmasq - 2.89-6
dropbear - 2022.82-5
e2fsprogs - 1.47.0-2
eip197-mini-firmware - 20230804-1
ekoonepl-luci - 20230728
ekooneplstat - 20150706
ekooneplusb-luci - 20230728
f2fsck - 1.16.0-1
firewall4 - 2023-09-01-598d9fbb-1
fstools - 2023-02-28-bfe882d5-1
fwtool - 2019-11-12-8f7fe925-1
gawk - 5.2.1-2
getrandom - 2022-08-13-4c7b720b-2
glib2 - 2.74.0-5
hd-idle - 1.05-2
hostapd-common - 2023-09-08-e5ccbfc6-4
ip-tiny - 6.4.0-1
iptables-nft - 1.8.8-1
iw - 5.19-1
iwinfo - 2023-07-01-ca79f641-1
jansson4 - 2.14-3
jshn - 2023-05-23-75a3b870-1
jsonfilter - 2018-02-04-c7e938d6-1
kernel - 6.1.55-1-88aef2feb319d48055493fffc548fc70
kmod-asn1-decoder - 6.1.55-1
kmod-cfg80211 - 6.1.55+6.5-1
kmod-crypto-acompress - 6.1.55-1
kmod-crypto-aead - 6.1.55-1
kmod-crypto-authenc - 6.1.55-1
kmod-crypto-ccm - 6.1.55-1
kmod-crypto-cmac - 6.1.55-1
kmod-crypto-crc32 - 6.1.55-1
kmod-crypto-crc32c - 6.1.55-1
kmod-crypto-ctr - 6.1.55-1
kmod-crypto-des - 6.1.55-1
kmod-crypto-ecb - 6.1.55-1
kmod-crypto-gcm - 6.1.55-1
kmod-crypto-gf128 - 6.1.55-1
kmod-crypto-ghash - 6.1.55-1
kmod-crypto-hash - 6.1.55-1
kmod-crypto-hmac - 6.1.55-1
kmod-crypto-hw-safexcel - 6.1.55-1
kmod-crypto-kpp - 6.1.55-1
kmod-crypto-lib-chacha20 - 6.1.55-1
kmod-crypto-lib-chacha20poly1305 - 6.1.55-1
kmod-crypto-lib-curve25519 - 6.1.55-1
kmod-crypto-lib-poly1305 - 6.1.55-1
kmod-crypto-manager - 6.1.55-1
kmod-crypto-md4 - 6.1.55-1
kmod-crypto-md5 - 6.1.55-1
kmod-crypto-null - 6.1.55-1
kmod-crypto-rng - 6.1.55-1
kmod-crypto-seqiv - 6.1.55-1
kmod-crypto-sha1 - 6.1.55-1
kmod-crypto-sha256 - 6.1.55-1
kmod-crypto-sha512 - 6.1.55-1
kmod-fs-exfat - 6.1.55-1
kmod-fs-ext4 - 6.1.55-1
kmod-fs-f2fs - 6.1.55-1
kmod-fs-ksmbd - 6.1.55-1
kmod-fs-ntfs3 - 6.1.55-1
kmod-fs-smbfs-common - 6.1.55-1
kmod-fs-vfat - 6.1.55-1
kmod-gpio-button-hotplug - 6.1.55-3
kmod-hwmon-core - 6.1.55-1
kmod-ipt-core - 6.1.55-1
kmod-leds-gpio - 6.1.55-1
kmod-lib-crc-ccitt - 6.1.55-1
kmod-lib-crc16 - 6.1.55-1
kmod-lib-crc32c - 6.1.55-1
kmod-lib-lzo - 6.1.55-1
kmod-mac80211 - 6.1.55+6.5-1
kmod-mii - 6.1.55-1
kmod-mt76-connac - 6.1.55+2023-09-18-2afc7285-1
kmod-mt76-core - 6.1.55+2023-09-18-2afc7285-1
kmod-mt7915e - 6.1.55+2023-09-18-2afc7285-1
kmod-mt7981-firmware - 6.1.55+2023-09-18-2afc7285-1
kmod-nat46 - 6.1.55+2022-09-19-4c5beee2-1
kmod-nf-conntrack - 6.1.55-1
kmod-nf-conntrack6 - 6.1.55-1
kmod-nf-flow - 6.1.55-1
kmod-nf-ipt - 6.1.55-1
kmod-nf-log - 6.1.55-1
kmod-nf-log6 - 6.1.55-1
kmod-nf-nat - 6.1.55-1
kmod-nf-reject - 6.1.55-1
kmod-nf-reject6 - 6.1.55-1
kmod-nfnetlink - 6.1.55-1
kmod-nft-bridge - 6.1.55-1
kmod-nft-compat - 6.1.55-1
kmod-nft-core - 6.1.55-1
kmod-nft-fib - 6.1.55-1
kmod-nft-nat - 6.1.55-1
kmod-nft-netdev - 6.1.55-1
kmod-nft-offload - 6.1.55-1
kmod-nls-base - 6.1.55-1
kmod-nls-cp437 - 6.1.55-1
kmod-nls-iso8859-1 - 6.1.55-1
kmod-nls-utf8 - 6.1.55-1
kmod-oid-registry - 6.1.55-1
kmod-ppp - 6.1.55-1
kmod-pppoe - 6.1.55-1
kmod-pppox - 6.1.55-1
kmod-scsi-core - 6.1.55-1
kmod-slhc - 6.1.55-1
kmod-thermal - 6.1.55-1
kmod-tun - 6.1.55-1
kmod-udptunnel4 - 6.1.55-1
kmod-udptunnel6 - 6.1.55-1
kmod-usb-acm - 6.1.55-1
kmod-usb-core - 6.1.55-1
kmod-usb-ehci - 6.1.55-1
kmod-usb-net - 6.1.55-1
kmod-usb-net-cdc-ether - 6.1.55-1
kmod-usb-net-cdc-mbim - 6.1.55-1
kmod-usb-net-cdc-ncm - 6.1.55-1
kmod-usb-net-huawei-cdc-ncm - 6.1.55-1
kmod-usb-net-qmi-wwan - 6.1.55-1
kmod-usb-net-rndis - 6.1.55-1
kmod-usb-ohci - 6.1.55-1
kmod-usb-ohci-pci - 6.1.55-1
kmod-usb-printer - 6.1.55-1
kmod-usb-serial - 6.1.55-1
kmod-usb-serial-option - 6.1.55-1
kmod-usb-serial-qualcomm - 6.1.55-1
kmod-usb-serial-sierrawireless - 6.1.55-1
kmod-usb-serial-wwan - 6.1.55-1
kmod-usb-storage - 6.1.55-1
kmod-usb-storage-extras - 6.1.55-1
kmod-usb-storage-uas - 6.1.55-1
kmod-usb-uhci - 6.1.55-1
kmod-usb-wdm - 6.1.55-1
kmod-usb-xhci-hcd - 6.1.55-1
kmod-usb-xhci-mtk - 6.1.55-1
kmod-usb2 - 6.1.55-1
kmod-usb2-pci - 6.1.55-1
kmod-usb3 - 6.1.55-1
kmod-wireguard - 6.1.55-1
ksmbd-server - 3.4.8-1
libatomic1 - 12.3.0-4
libattr - 2.5.1-1
libblkid1 - 2.39-2
libblobmsg-json20230523 - 2023-05-23-75a3b870-1
libbz2-1.0 - 1.0.8-1
libc - 1.2.4-4
libcap-ng - 0.8.3-2
libcomerr0 - 1.47.0-2
libexif - 0.6.24-1
libext2fs2 - 1.47.0-2
libf2fs6 - 1.16.0-1
libffi - 3.4.2-2
libffmpeg-audio-dec - 5.1.3-2
libflac - 1.3.4-1
libgcc1 - 12.3.0-4
libid3tag - 0.15.1b-4
libiptext-nft0 - 1.8.8-1
libiptext0 - 1.8.8-1
libiptext6-0 - 1.8.8-1
libiwinfo-data - 2023-07-01-ca79f641-1
libiwinfo20230701 - 2023-07-01-ca79f641-1
libjpeg-turbo - 2.1.4-2
libjson-c5 - 0.16-3
libjson-script20230523 - 2023-05-23-75a3b870-1
liblua5.1.5 - 5.1.5-10
liblucihttp-lua - 2023-03-15-9b5b683f-1
liblucihttp-ucode - 2023-03-15-9b5b683f-1
liblucihttp0 - 2023-03-15-9b5b683f-1
liblz4-1 - 1.9.4-1
liblzo2 - 2.10-4
libmbedtls12 - 2.28.4-1
libmbim - 1.28.4-1
libmnl0 - 1.0.5-1
libmount1 - 2.39-2
libncurses6 - 6.4-2
libnftnl11 - 1.2.6-1
libnl-core200 - 3.7.0-1
libnl-genl200 - 3.7.0-1
libnl-tiny1 - 2023-07-27-bc92a280-1
libogg0 - 1.3.5-1
libopenssl-conf - 3.0.11-1
libopenssl3 - 3.0.11-1
libpcre2 - 10.42-1
libpthread - 1.2.4-4
libqmi - 1.32.4-1
libqrtr-glib - 1.2.2-3
libreadline8 - 8.2-1
librt - 1.2.4-4
libsmartcols1 - 2.39-2
libsqlite3-0 - 3410200-1
libss2 - 1.47.0-2
libstdcpp6 - 12.3.0-4
libubox20230523 - 2023-05-23-75a3b870-1
libubus-lua - 2023-06-05-f787c97b-1
libubus20230605 - 2023-06-05-f787c97b-1
libuci20130104 - 2023-08-10-5781664d-1
libuclient20201210 - 2023-04-13-007d9454-1
libucode20220812 - 2023-06-06-c7d84aae-1
libusb-1.0-0 - 1.0.26-3
libustream-openssl20201210 - 2023-02-25-498f6e26-1
libuuid1 - 2.39-2
libvorbis - 1.3.7-2
libxtables12 - 1.8.8-1
logd - 2022-08-13-4c7b720b-2
lsblk - 2.39-2
lua - 5.1.5-10
luci - git-23.252.26061-de65ace
luci-app-3ginfo-lite - 1.0.56-20230930
luci-app-aria2 - git-23.267.29818-4c03f5f
luci-app-atcommands - 1.0.4-20230701
luci-app-commands - git-23.267.29502-3e7fe9f
luci-app-cpu-status-mini - 0.1-5
luci-app-drive-status-mini - 0.4-20230701
luci-app-ekooneplstat - 20220729
luci-app-firewall - git-23.267.29502-3e7fe9f
luci-app-hd-idle - git-23.267.29502-3e7fe9f
luci-app-internet-detector - 0.4
luci-app-ksmbd - git-23.267.29502-3e7fe9f
luci-app-lite-watchdog - 1.0.11-20230815
luci-app-minidlna - git-23.267.29502-3e7fe9f
luci-app-modemband - 1.0.21-20230914
luci-app-modemdefine - 1.0.4-20230711
luci-app-nft-qos - git-23.267.29502-3e7fe9f
luci-app-openvpn - git-23.267.29502-3e7fe9f
luci-app-opkg - git-23.267.29502-3e7fe9f
luci-app-p910nd - git-23.267.29502-3e7fe9f
luci-app-sms-tool-js - 2.0.15-20230930
luci-app-wrtbwmon - 2.0.10
luci-app-zbt-sensors-status - 1.0
luci-base - git-23.266.27574-7744ad0
luci-compat - git-23.252.26061-de65ace
luci-i18n-3ginfo-lite-pl - unknown
luci-i18n-aria2-pl - git-23.270.68722-cbe0748
luci-i18n-atcommands-pl - unknown
luci-i18n-base-pl - git-23.270.68722-cbe0748
luci-i18n-commands-pl - git-23.263.30531-f59a194
luci-i18n-cpu-status-mini-pl - unknown
luci-i18n-drive-status-mini-pl - unknown
luci-i18n-firewall-pl - git-23.270.68722-cbe0748
luci-i18n-hd-idle-pl - git-23.263.30531-f59a194
luci-i18n-internet-detector-pl - unknown
luci-i18n-ksmbd-pl - git-23.270.68722-cbe0748
luci-i18n-lite-watchdog-pl - unknown
luci-i18n-minidlna-pl - git-23.270.68722-cbe0748
luci-i18n-modemband-pl - unknown
luci-i18n-modemdefine-pl - unknown
luci-i18n-nft-qos-pl - git-23.270.68722-cbe0748
luci-i18n-openvpn-pl - git-23.263.30531-f59a194
luci-i18n-opkg-pl - git-23.263.30531-f59a194
luci-i18n-p910nd-pl - git-23.263.30531-f59a194
luci-i18n-sms-tool-js-pl - unknown
luci-i18n-wrtbwmon-pl - unknown
luci-i18n-zbt-sensors-status-pl - unknown
luci-lib-base - git-23.252.26061-de65ace
luci-lib-ip - git-23.252.26061-de65ace
luci-lib-jsonc - git-23.252.26061-de65ace
luci-lib-nixio - git-23.252.26061-de65ace
luci-lib-px5g - git-23.252.26061-de65ace
luci-light - git-23.252.26061-de65ace
luci-lua-runtime - git-23.252.26061-de65ace
luci-mod-admin-full - git-23.252.26061-de65ace
luci-mod-network - git-23.264.73274-598b1eb
luci-mod-status - git-23.261.42034-318ef4c
luci-mod-system - git-23.252.26061-de65ace
luci-proto-3g - git-23.252.26061-de65ace
luci-proto-ipv6 - git-23.252.26061-de65ace
luci-proto-mbim - git-23.252.26061-de65ace
luci-proto-ncm - git-23.252.26061-de65ace
luci-proto-ppp - git-23.252.26061-de65ace
luci-proto-qmi - git-23.252.26061-de65ace
luci-proto-wireguard - git-23.267.54995-527453f
luci-ssl-openssl - git-23.252.26061-de65ace
luci-theme-bootstrap - git-23.252.26061-de65ace
mbim-utils - 1.28.4-1
mhz - 2023-06-17-11aac239-2
minidlna - 1.3.3-1
mkf2fs - 1.16.0-1
modemband - 20230914
mt7981-wo-firmware - 20230804-1
mtd - 26
netifd - 2023-09-19-7a58b995-2
nft-qos - 1.0.6-4
nftables-json - 1.0.8-1
odhcp6c - 2023-05-12-bcd28363-20
odhcpd-ipv6only - 2023-06-24-52112643-1
openssl-util - 3.0.11-1
openvpn-easy-rsa - 3.1.3-1
openvpn-openssl - 2.6.6-1
openwrt-keyring - 2022-03-25-62471e69-2
opkg - 2022-02-24-d038e5b6-2
p910nd - 0.97-9
ppp - 2.4.9.git-2021-01-04-5
ppp-mod-pppoe - 2.4.9.git-2021-01-04-5
procd - 2023-06-25-2db83655-3
procd-seccomp - 2023-06-25-2db83655-3
procd-ujail - 2023-06-25-2db83655-3
qfirehose - 1.4.15-1
qlog - 1
qmi-utils - 1.32.4-1
rpcd - 2023-07-01-c07ab2f9-1
rpcd-mod-file - 2023-07-01-c07ab2f9-1
rpcd-mod-iwinfo - 2023-07-01-c07ab2f9-1
rpcd-mod-luci - 20230123-1
rpcd-mod-rrdns - 20170710
rpcd-mod-ucode - 2023-07-01-c07ab2f9-1
sms-tool - 2022-03-21-f07699ab-1
sysinfo - 20210313
terminfo - 6.4-2
ubi-utils - 2.1.5-1
uboot-envtools - 2023.07.02-2
ubox - 2022-08-13-4c7b720b-2
ubus - 2023-06-05-f787c97b-1
ubusd - 2023-06-05-f787c97b-1
uci - 2023-08-10-5781664d-1
uclient-fetch - 2023-04-13-007d9454-1
ucode - 2023-06-06-c7d84aae-1
ucode-mod-fs - 2023-06-06-c7d84aae-1
ucode-mod-html - 1
ucode-mod-lua - 1
ucode-mod-math - 2023-06-06-c7d84aae-1
ucode-mod-nl80211 - 2023-06-06-c7d84aae-1
ucode-mod-rtnl - 2023-06-06-c7d84aae-1
ucode-mod-ubus - 2023-06-06-c7d84aae-1
ucode-mod-uci - 2023-06-06-c7d84aae-1
ucode-mod-uloop - 2023-06-06-c7d84aae-1
uhttpd - 2023-06-25-34a8a74d-1
uhttpd-mod-ubus - 2023-06-25-34a8a74d-1
umbim - 2022-08-13-146bc77c-24
uqmi - 2022-05-04-56cb2d40-5
urandom-seed - 3
urngd - 2023-07-25-7aefb47b-1
usb-modeswitch - 2022-02-24-3c8595a4-1
usign - 2020-05-23-f1f65026-1
webconsole - 1.000-1
wget-ssl - 1.21.3-3
wireguard-tools - 1.0.20210914-2
wireless-regdb - 2023.09.01-1
wpad-basic-mbedtls - 2023-09-08-e5ccbfc6-4
wrtbwmon - 1.2.1-3
wsdd2 - 2022-04-25-e37443ac-3
wwan - 2019-04-29-6
xtables-nft - 1.8.8-1
zlib - 1.2.13-1
```
</details>

### Useful AT commands (also available in the built image)
<details>
   <summary>Pokaż | Show me</summary>
   
``` bash
4x4/2x2 MIMO ON/OFF ➜ AT+QCFG="lte4x4mimo/disable",0;AT+QCFG="lte4x4mimo/disable",0
4x4/2x2 MIMO OFF/ON ➜ AT+QCFG="lte4x4mimo/disable",1;AT+QCFG="lte4x4mimo/disable",1
Disable Cell Lock ➜ AT+QNWLOCK="COMMON/4G",0;AT+QNWLOCK="COMMON/4G",0
Query ➜ AT+QNWLOCK="COMMON/4G";AT+QNWLOCK="COMMON/4G"
CellLock ➜ AT+QNWLOCK="COMMON/4G",NUM OF CELLS,FREQ,PCI;AT+QNWLOCK="COMMON/4G",1,
Check the signal info on each antenna port ➜ AT+QRSRP;AT+QRSRP
Query and Report Signal Strength ➜ AT+QCSQ;AT+QCSQ
Get the temperature of MT ➜ AT+QTEMP;AT+QTEMP
Check the firmware version ➜ AT+GMR;AT+GMR
Band Preferred ➜ AT+QNWPREFCFG="lte_band"?;AT+QNWPREFCFG="lte_band"?
Carrier Agregation Info ➜ AT+QCAINFO;AT+QCAINFO
Query the serving cell information ➜ AT+QENG="servingcell";AT+QENG="servingcell"
Query the information of neighbour cells ➜ AT+QENG="neighbourcell";AT+QENG="neighbourcell"
Query network information ➜ AT+QNWINFO;AT+QNWINFO
Band 1/3/7/8/20/38 ➜ AT+QNWPREFCFG="lte_band",1:3:7:8:20:38;AT+QNWPREFCFG="lte_band",1:3:7:8:20:38
SIM Preferred Message Storage ➜ AT+CPMS="SM","SM","SM";AT+CPMS="SM","SM","SM"
Modem memory preferred Message Storage ➜ AT+CPMS="ME","ME","ME";AT+CPMS="ME","ME","ME"
Save SMS Settings ➜ AT+CSAS;AT+CSAS
Reboot the modem ➜ AT+CFUN=1,1;AT+CFUN=1,1
Reset the modem ➜ AT+CFUN=1;AT+CFUN=1
Reset modem to factory default ➜ AT+QPRTPARA=3;AT+QPRTPARA=3
Save NVM items through reset/reboot ➜ AT+QPRTPARA=1;AT+QPRTPARA=1
QMI/PPP/Default ➜ AT+QCFG="usbnet",0;AT+QCFG="usbnet",0
ECM ➜ AT+QCFG="usbnet",1;AT+QCFG="usbnet",1
MBIM ➜ AT+QCFG="usbnet",2;AT+QCFG="usbnet",2
Set RAT to 4G-LTE only ➜ AT+QNWPREFCFG="mode_pref",LTE;AT+QNWPREFCFG="mode_pref",LTE
Set RAT to LTE & 5G NR ➜ AT+QNWPREFCFG= "mode_pref",LTE:NR5G;AT+QNWPREFCFG= "mode_pref",LTE:NR5G
WCDMA only ➜ AT+QCFG="nwscanmode",2,1;AT+QCFG="nwscanmode",2,1
GSM only ➜ AT+QCFG="nwscanmode",1,1;AT+QCFG="nwscanmode",1,1
Scan all modes ➜ AT+QNWPREFCFG="mode_pref",AUTO;AT+QNWPREFCFG="mode_pref",AUTO
```

</details>
