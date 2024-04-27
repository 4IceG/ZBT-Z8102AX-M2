# ZBT-Z8102AX-M2 V1
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
aria2 - 1.36.0-r2
ariang - 1.3.6-r1
base-files - 1590~a8dde7e5bd
block-mount - 2024.01.22~08cd7083-r1
busybox - 1.36.1-r1
ca-bundle - 20240203-r1
ca-certificates - 20240203-r1
cgi-io - 2022.08.10~901b0f04-r21
chat - 2.4.9_git20210104-r5
comgt - 0.32-r35
comgt-ncm - 0.32-r35
dnsmasq - 2.90-r2
dropbear - 2022.83-r1
e2fsprogs - 1.47.0-r2
eip197-mini-firmware - 20240220-r1
ekoonepl-luci - 20231219
ekooneplstat - 20150706
ekooneplusb-luci - 20231219
ethtool-full - 6.6-r1
f2fsck - 1.16.0-r2
firewall4 - 2023.11.03~698a5335-r1
fitblk - 1
fstools - 2024.01.22~08cd7083-r1
fwtool - 2019.11.12~8f7fe925-r1
gawk - 5.3.0-r1
getrandom - 2024.03.02~d4139030-r1
glib2 - 2.74.7-r3
gzip - 1.13-r1
hd-idle - 1.05-r2
hostapd-common - 2024.03.09~695277a5-r1
ip-tiny - 6.7.0-r1
iptables-nft - 1.8.8-r2
iw - 5.19-r1
iwinfo - 2024.03.23~79a96150-r1
jansson4 - 2.14-r3
jshn - 2024.03.29~eb9bcb64-r1
jsonfilter - 2024.01.23~594cfa86-r1
kernel - 6.6.28~27a3618cd17297e1502abeaadb1f6c01-r1
kmod-asn1-decoder - 6.6.28-r1
kmod-cfg80211 - 6.6.28.6.6.15-r1
kmod-crypto-aead - 6.6.28-r1
kmod-crypto-authenc - 6.6.28-r1
kmod-crypto-ccm - 6.6.28-r1
kmod-crypto-cmac - 6.6.28-r1
kmod-crypto-crc32 - 6.6.28-r1
kmod-crypto-crc32c - 6.6.28-r1
kmod-crypto-ctr - 6.6.28-r1
kmod-crypto-des - 6.6.28-r1
kmod-crypto-ecb - 6.6.28-r1
kmod-crypto-gcm - 6.6.28-r1
kmod-crypto-geniv - 6.6.28-r1
kmod-crypto-gf128 - 6.6.28-r1
kmod-crypto-ghash - 6.6.28-r1
kmod-crypto-hash - 6.6.28-r1
kmod-crypto-hmac - 6.6.28-r1
kmod-crypto-hw-safexcel - 6.6.28-r1
kmod-crypto-kpp - 6.6.28-r1
kmod-crypto-lib-chacha20 - 6.6.28-r1
kmod-crypto-lib-chacha20poly1305 - 6.6.28-r1
kmod-crypto-lib-curve25519 - 6.6.28-r1
kmod-crypto-lib-poly1305 - 6.6.28-r1
kmod-crypto-manager - 6.6.28-r1
kmod-crypto-md4 - 6.6.28-r1
kmod-crypto-md5 - 6.6.28-r1
kmod-crypto-null - 6.6.28-r1
kmod-crypto-rng - 6.6.28-r1
kmod-crypto-seqiv - 6.6.28-r1
kmod-crypto-sha1 - 6.6.28-r1
kmod-crypto-sha256 - 6.6.28-r1
kmod-crypto-sha3 - 6.6.28-r1
kmod-crypto-sha512 - 6.6.28-r1
kmod-fs-exfat - 6.6.28-r1
kmod-fs-ext4 - 6.6.28-r1
kmod-fs-f2fs - 6.6.28-r1
kmod-fs-ksmbd - 6.6.28-r1
kmod-fs-netfs - 6.6.28-r1
kmod-fs-ntfs3 - 6.6.28-r1
kmod-fs-smbfs-common - 6.6.28-r1
kmod-fs-vfat - 6.6.28-r1
kmod-gpio-button-hotplug - 6.6.28-r3
kmod-hwmon-core - 6.6.28-r1
kmod-ipt-core - 6.6.28-r1
kmod-leds-gpio - 6.6.28-r1
kmod-lib-crc-ccitt - 6.6.28-r1
kmod-lib-crc16 - 6.6.28-r1
kmod-lib-crc32c - 6.6.28-r1
kmod-libphy - 6.6.28-r1
kmod-mac80211 - 6.6.28.6.6.15-r1
kmod-mii - 6.6.28-r1
kmod-mt76-connac - 6.6.28.2024.04.03~1e336a85-r1
kmod-mt76-core - 6.6.28.2024.04.03~1e336a85-r1
kmod-mt7915e - 6.6.28.2024.04.03~1e336a85-r1
kmod-mt7981-firmware - 6.6.28.2024.04.03~1e336a85-r1
kmod-nat46 - 6.6.28.2022.09.19~4c5beee2-r1
kmod-nf-conntrack - 6.6.28-r1
kmod-nf-conntrack6 - 6.6.28-r1
kmod-nf-flow - 6.6.28-r1
kmod-nf-ipt - 6.6.28-r1
kmod-nf-log - 6.6.28-r1
kmod-nf-log6 - 6.6.28-r1
kmod-nf-nat - 6.6.28-r1
kmod-nf-reject - 6.6.28-r1
kmod-nf-reject6 - 6.6.28-r1
kmod-nfnetlink - 6.6.28-r1
kmod-nft-bridge - 6.6.28-r1
kmod-nft-compat - 6.6.28-r1
kmod-nft-core - 6.6.28-r1
kmod-nft-fib - 6.6.28-r1
kmod-nft-nat - 6.6.28-r1
kmod-nft-netdev - 6.6.28-r1
kmod-nft-offload - 6.6.28-r1
kmod-nls-base - 6.6.28-r1
kmod-nls-cp437 - 6.6.28-r1
kmod-nls-iso8859-1 - 6.6.28-r1
kmod-nls-ucs2-utils - 6.6.28-r1
kmod-nls-utf8 - 6.6.28-r1
kmod-oid-registry - 6.6.28-r1
kmod-phy-aquantia - 6.6.28-r1
kmod-ppp - 6.6.28-r1
kmod-pppoe - 6.6.28-r1
kmod-pppox - 6.6.28-r1
kmod-scsi-core - 6.6.28-r1
kmod-slhc - 6.6.28-r1
kmod-tcp-bbr - 6.6.28-r1
kmod-thermal - 6.6.28-r1
kmod-tun - 6.6.28-r1
kmod-udptunnel4 - 6.6.28-r1
kmod-udptunnel6 - 6.6.28-r1
kmod-usb-acm - 6.6.28-r1
kmod-usb-core - 6.6.28-r1
kmod-usb-ehci - 6.6.28-r1
kmod-usb-net - 6.6.28-r1
kmod-usb-net-cdc-ether - 6.6.28-r1
kmod-usb-net-cdc-mbim - 6.6.28-r1
kmod-usb-net-cdc-ncm - 6.6.28-r1
kmod-usb-net-huawei-cdc-ncm - 6.6.28-r1
kmod-usb-net-qmi-wwan - 6.6.28-r1
kmod-usb-net-rndis - 6.6.28-r1
kmod-usb-ohci - 6.6.28-r1
kmod-usb-ohci-pci - 6.6.28-r1
kmod-usb-printer - 6.6.28-r1
kmod-usb-serial - 6.6.28-r1
kmod-usb-serial-option - 6.6.28-r1
kmod-usb-serial-qualcomm - 6.6.28-r1
kmod-usb-serial-sierrawireless - 6.6.28-r1
kmod-usb-serial-wwan - 6.6.28-r1
kmod-usb-storage - 6.6.28-r1
kmod-usb-storage-extras - 6.6.28-r1
kmod-usb-storage-uas - 6.6.28-r1
kmod-usb-uhci - 6.6.28-r1
kmod-usb-wdm - 6.6.28-r1
kmod-usb-xhci-hcd - 6.6.28-r1
kmod-usb-xhci-mtk - 6.6.28-r1
kmod-usb2 - 6.6.28-r1
kmod-usb2-pci - 6.6.28-r1
kmod-usb3 - 6.6.28-r1
kmod-wireguard - 6.6.28-r1
ksmbd-server - 3.5.2-r1
libatomic1 - 13.2.0-r4
libattr - 2.5.2-r1
libblkid1 - 2.39.3-r1
libblobmsg-json20240329 - 2024.03.29~eb9bcb64-r1
libbz2-1.0 - 1.0.8-r1
libc - 1.2.5-r4
libcap-ng - 0.8.4-r1
libcomerr0 - 1.47.0-r2
libe2p2 - 1.47.0-r2
libexif - 0.6.24-r1
libext2fs2 - 1.47.0-r2
libf2fs6 - 1.16.0-r2
libffi - 3.4.6-r1
libffmpeg-audio-dec - 5.1.3-r5
libflac - 1.4.3-r1
libgcc1 - 13.2.0-r4
libid3tag - 0.16.3-r1
libiptext-nft0 - 1.8.8-r2
libiptext0 - 1.8.8-r2
libiptext6-0 - 1.8.8-r2
libiwinfo-data - 2024.03.23~79a96150-r1
libiwinfo20230701 - 2024.03.23~79a96150-r1
libjpeg-turbo - 3.0.2-r1
libjson-c5 - 0.17-r1
libjson-script20240329 - 2024.03.29~eb9bcb64-r1
liblua5.1.5 - 5.1.5-r11
liblucihttp-lua - 2023.03.15~9b5b683f-r1
liblucihttp-ucode - 2023.03.15~9b5b683f-r1
liblucihttp0 - 2023.03.15~9b5b683f-r1
liblz4-1 - 1.9.4-r1
liblzo2 - 2.10-r4
libmbedtls13 - 2.28.8-r1
libmbim - 1.30.0-r2
libmnl0 - 1.0.5-r1
libmount1 - 2.39.3-r1
libncurses6 - 6.4-r2
libnftnl11 - 1.2.6-r1
libnl-core200 - 3.9.0-r1
libnl-genl200 - 3.9.0-r1
libnl-tiny1 - 2023.12.05~965c4bf4-r1
libogg0 - 1.3.5-r1
libopenssl-conf - 3.0.13-r1
libopenssl3 - 3.0.13-r1
libpcre2 - 10.42-r1
libpthread - 1.2.5-r4
libqmi - 1.34.0-r2
libqrtr-glib - 1.2.2-r3
libreadline8 - 8.2-r1
librt - 1.2.5-r4
libsmartcols1 - 2.39.3-r1
libsqlite3-0 - 3410200-r1
libss2 - 1.47.0-r2
libstdcpp6 - 13.2.0-r4
libubox20240329 - 2024.03.29~eb9bcb64-r1
libubus-lua - 2023.11.28~f84eb599-r1
libubus20231128 - 2023.11.28~f84eb599-r1
libuci20130104 - 2023.08.10~5781664d-r1
libuclient20201210 - 2024.04.19~e8780fa7-r1
libucode20230711 - 2024.04.07~5507654a-r1
libudebug - 2023.12.06~6d3f51f9
libusb-1.0-0 - 1.0.26-r3
libustream-openssl20201210 - 2024.04.19~524a76e5-r1
libuuid1 - 2.39.3-r1
libvorbis - 1.3.7-r2
libxtables12 - 1.8.8-r2
logd - 2024.03.02~d4139030-r1
lsblk - 2.39.3-r1
lua - 5.1.5-r11
luci - 24.049.84207~c8cddc3
luci-app-3ginfo-lite - 1.0.69-20240427-1
luci-app-aria2 - 24.049.84207~c8cddc3
luci-app-atcommands - 1.0.8-20240102-1
luci-app-commands - 24.049.84207~c8cddc3
luci-app-cpu-status-mini - 0.1-5-1
luci-app-drive-status-mini - 0.5-20240205-1
luci-app-easyconfig-transfer - 1.0.7-20240427-1
luci-app-ekooneplstat - 20231220
luci-app-filebrowser - 1.1.0-1
luci-app-firewall - 24.102.51352~cc44632
luci-app-hd-idle - 24.049.84207~c8cddc3
luci-app-internet-detector - 0.4-1
luci-app-ksmbd - 24.049.84207~c8cddc3
luci-app-lite-watchdog - 1.0.15-20240102-1
luci-app-minidlna - 24.102.51352~862c675
luci-app-modemband - 1.0.25-20240330-1
luci-app-modemdefine - 1.0.6-20240330-1
luci-app-nft-qos - 24.075.52231~d94efb5
luci-app-openvpn - 24.108.02989~f630156
luci-app-opkg - 24.076.42328~4d23adc
luci-app-p910nd - 24.102.51352~5c6fbba
luci-app-sms-tool-js - 2.0.21-20240421-1
luci-app-zbt-sensors-status - 1.0-1
luci-base - 24.102.51352~4cffc9f
luci-compat - 24.079.46325~f896ca1
luci-i18n-3ginfo-lite-pl - 0
luci-i18n-aria2-pl - 24.115.26817~307bba4
luci-i18n-atcommands-pl - 0
luci-i18n-base-pl - 24.116.39921~cd26146
luci-i18n-commands-pl - 24.106.57326~da794c7
luci-i18n-cpu-status-mini-pl - 0
luci-i18n-drive-status-mini-pl - 0
luci-i18n-easyconfig-transfer-pl - 0
luci-i18n-firewall-pl - 24.112.71589~c6e201a
luci-i18n-hd-idle-pl - 24.110.61618~49a0a91
luci-i18n-internet-detector-pl - 0
luci-i18n-ksmbd-pl - 24.110.61618~49a0a91
luci-i18n-lite-watchdog-pl - 0
luci-i18n-minidlna-pl - 24.110.61618~49a0a91
luci-i18n-modemband-pl - 0
luci-i18n-modemdefine-pl - 0
luci-i18n-nft-qos-pl - 24.110.61618~49a0a91
luci-i18n-openvpn-pl - 24.115.75043~25af314
luci-i18n-opkg-pl - 24.110.61618~49a0a91
luci-i18n-p910nd-pl - 24.110.61618~49a0a91
luci-i18n-sms-tool-js-pl - 0
luci-i18n-zbt-sensors-status-pl - 0
luci-lib-base - 24.079.46064~3e3005c
luci-lib-ip - 24.049.84207~c8cddc3
luci-lib-jsonc - 24.079.46156~c1e3fa9
luci-lib-nixio - 24.049.84207~c8cddc3
luci-lib-px5g - 24.049.84207~c8cddc3
luci-light - 24.049.84207~c8cddc3
luci-lua-runtime - 24.079.46338~374af8b
luci-mod-admin-full - 24.049.84207~c8cddc3
luci-mod-network - 24.111.82636~ea7452d
luci-mod-status - 24.115.26262~a4a7f0b
luci-mod-system - 24.102.51352~2967807
luci-proto-3g - 24.079.44556~466110d
luci-proto-ipv6 - 24.076.80664~c88e247
luci-proto-mbim - 24.079.44556~8c5865e
luci-proto-ncm - 24.079.44556~cd411a8
luci-proto-ppp - 24.107.56915~995d3a1
luci-proto-qmi - 24.079.44556~9cdb26b
luci-proto-wireguard - 24.116.61717~1ba94f2
luci-ssl-openssl - 24.079.45685~320744f
luci-theme-bootstrap - 24.087.66588~bd2b2ec
mbim-utils - 1.30.0-r2
mhz - 2023.06.17~11aac239-r2
minidlna - 1.3.3-r1
mkf2fs - 1.16.0-r2
modemband - 20240330
mt7981-wo-firmware - 20240220-r1
mtd - 26
netifd - 2024.01.04~f01345ec-r1
nft-qos - 1.0.6-r4
nftables-json - 1.0.9-r1
odhcp6c - 2023.05.12~bcd28363-r20
odhcpd-ipv6only - 2023.10.24~d8118f6e-r1
openssl-util - 3.0.13-r1
openvpn-easy-rsa - 3.1.3-r1
openvpn-openssl - 2.6.10-r1
openwrt-keyring - 2022.03.25~62471e69-r2
opkg - 2022.02.24~d038e5b6-r2
p910nd - 0.97-r14
ppp - 2.4.9_git20210104-r5
ppp-mod-pppoe - 2.4.9_git20210104-r5
procd - 2024.03.30~946552a7-r1
procd-seccomp - 2024.03.30~946552a7-r1
procd-ujail - 2024.03.30~946552a7-r1
qfirehose - 1.4.17-r1
qlog - 1
qmi-utils - 1.34.0-r2
rpcd - 2024.02.22~8ef4c258-r1
rpcd-mod-file - 2024.02.22~8ef4c258-r1
rpcd-mod-iwinfo - 2024.02.22~8ef4c258-r1
rpcd-mod-luci - 20240305-r1
rpcd-mod-rrdns - 20170710
rpcd-mod-ucode - 2024.02.22~8ef4c258-r1
sms-tool - 2023.09.21~1b6ca032-r1
sysinfo - 20210313
terminfo - 6.4-r2
ubi-utils - 2.1.6-r1
uboot-envtools - 2024.01-r2
ubox - 2024.03.02~d4139030-r1
ubus - 2023.11.28~f84eb599-r1
ubusd - 2023.11.28~f84eb599-r1
uci - 2023.08.10~5781664d-r1
uclient-fetch - 2024.04.19~e8780fa7-r1
ucode - 2024.04.07~5507654a-r1
ucode-mod-fs - 2024.04.07~5507654a-r1
ucode-mod-html - 1
ucode-mod-lua - 1
ucode-mod-math - 2024.04.07~5507654a-r1
ucode-mod-nl80211 - 2024.04.07~5507654a-r1
ucode-mod-rtnl - 2024.04.07~5507654a-r1
ucode-mod-ubus - 2024.04.07~5507654a-r1
ucode-mod-uci - 2024.04.07~5507654a-r1
ucode-mod-uloop - 2024.04.07~5507654a-r1
uhttpd - 2023.06.25~34a8a74d-r3
uhttpd-mod-ubus - 2023.06.25~34a8a74d-r3
umbim - 2022.08.13~146bc77c-r24
uqmi - 2024.01.16~c3488b83-r1
urandom-seed - 3
urngd - 2023.11.01~44365eb1-r1
usb-modeswitch - 2022.02.24~3c8595a4-r1
usign - 2020.05.23~f1f65026-r1
webconsole - 1.000-r1
wget-ssl - 1.24.5-r1
wifi-scripts - 1.0-r1
wireguard-tools - 1.0.20210914-r3
wireless-regdb - 2024.01.23-r1
wpad-basic-mbedtls - 2024.03.09~695277a5-r1
wsdd2 - 2023.12.21~b676d8ac-r1
wwan - 2019.04.29-r6
xtables-nft - 1.8.8-r2
zlib - 1.3.1-r1
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
