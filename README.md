# ZBT-Z8102AX-M2 V1 & V2
My OpenWrt SNAPSHOT / LuCI Main :: user friendly :: build for the Z8102AX-M2 (Z8102AX V1 & V2) router.

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
adb-5.0.2~6fe92d1a-r4
apk-mbedtls-3.0.0_pre20250606-r2
aria2-1.37.0-r3
aria2-openssl-1.37.0-r3
ariang-1.3.11-r1
atinout-0.9.1
base-files-1667~5cb0ccfc8b
block-mount-2025.10.03~12858e28-r1
busybox-1.37.0-r5
ca-bundle-20250419-r1
ca-certificates-20250419-r1
cgi-io-2022.08.10~901b0f04-r21
chat-2.5.2-r2
comgt-0.32-r36
comgt-ncm-0.32-r36
debugfs-1.47.2-r1
dnsmasq-2.91-r2
dropbear-2025.88-r4
e2fsprogs-1.47.2-r1
eip197-mini-firmware-20250917-r1
ekoonepl-luci-20250123 
ekooneplstat-20150706 
ekooneplusb-20230616 
ekooneplusb-luci-20250123  
ethtool-full-6.15-r1  
f2fsck-1.16.0-r4  
fdisk-2.41.1-r2  
firewall4-2025.03.17~b6e51575-r1  
fit-check-sign-2025.07-r1  
fitblk-2  
fstools-2025.10.03~12858e28-r1  
fwtool-2025.10.03~04cd252e-r1  
gawk-5.3.2-r1  
getrandom-2025.10.03~c75525a5-r1  
glib2-2.82.0-r1  
gzip-1.14-r1  
hd-idle-1.05-r2  
hostapd-common-2025.08.26~ca266cc2-r1  
ip-tiny-6.14.0-r1  
iptables-nft-1.8.10-r2  
iw-6.9-r4  
iwinfo-2025.02.06~9cec6b4d-r1  
jansson4-2.14-r3  
jshn-2025.10.04~c163d7ab-r1  
jsonfilter-2025.10.04~f4fe702d-r1  
kernel-6.12.50~88252ac6b57e139854a63a13f28252c9-r1  
kmod-asn1-decoder-6.12.50-r1  
kmod-cfg80211-6.12.50.6.16-r1  
kmod-crypto-aead-6.12.50-r1  
kmod-crypto-authenc-6.12.50-r1  
kmod-crypto-ccm-6.12.50-r1  
kmod-crypto-cmac-6.12.50-r1  
kmod-crypto-crc32-6.12.50-r1  
kmod-crypto-crc32c-6.12.50-r1  
kmod-crypto-ctr-6.12.50-r1  
kmod-crypto-des-6.12.50-r1  
kmod-crypto-ecb-6.12.50-r1  
kmod-crypto-gcm-6.12.50-r1  
kmod-crypto-geniv-6.12.50-r1  
kmod-crypto-gf128-6.12.50-r1  
kmod-crypto-ghash-6.12.50-r1  
kmod-crypto-hash-6.12.50-r1  
kmod-crypto-hmac-6.12.50-r1  
kmod-crypto-hw-safexcel-6.12.50-r1  
kmod-crypto-kpp-6.12.50-r1  
kmod-crypto-lib-chacha20-6.12.50-r1  
kmod-crypto-lib-chacha20poly1305-6.12.50-r1  
kmod-crypto-lib-curve25519-6.12.50-r1  
kmod-crypto-lib-poly1305-6.12.50-r1  
kmod-crypto-manager-6.12.50-r1  
kmod-crypto-md4-6.12.50-r1  
kmod-crypto-md5-6.12.50-r1  
kmod-crypto-null-6.12.50-r1  
kmod-crypto-rng-6.12.50-r1  
kmod-crypto-seqiv-6.12.50-r1  
kmod-crypto-sha1-6.12.50-r1  
kmod-crypto-sha256-6.12.50-r1  
kmod-crypto-sha3-6.12.50-r1  
kmod-crypto-sha512-6.12.50-r1  
kmod-fs-exfat-6.12.50-r1  
kmod-fs-ext4-6.12.50-r1  
kmod-fs-f2fs-6.12.50-r1  
kmod-fs-ksmbd-6.12.50-r1  
kmod-fs-netfs-6.12.50-r1  
kmod-fs-ntfs3-6.12.50-r1  
kmod-fs-smbfs-common-6.12.50-r1  
kmod-fs-vfat-6.12.50-r1  
kmod-gpio-button-hotplug-6.12.50-r5  
kmod-hwmon-core-6.12.50-r1  
kmod-i2c-core-6.12.50-r1  
kmod-ipt-core-6.12.50-r1  
kmod-leds-gpio-6.12.50-r1  
kmod-lib-crc-ccitt-6.12.50-r1  
kmod-lib-crc-itu-t-6.12.50-r1  
kmod-lib-crc16-6.12.50-r1  
kmod-lib-crc32c-6.12.50-r1  
kmod-libphy-6.12.50-r1  
kmod-mac80211-6.12.50.6.16-r1  
kmod-mhi-bus-6.12.50-r1  
kmod-mhi-net-6.12.50-r1  
kmod-mhi-pci-generic-6.12.50-r1  
kmod-mhi-wwan-ctrl-6.12.50-r1  
kmod-mhi-wwan-mbim-6.12.50-r1  
kmod-mii-6.12.50-r1  
kmod-mt76-connac-6.12.50.2025.10.03~ec3f0548-r1  
kmod-mt76-core-6.12.50.2025.10.03~ec3f0548-r1  
kmod-mt7915e-6.12.50.2025.10.03~ec3f0548-r1  
kmod-mt7981-firmware-6.12.50.2025.10.03~ec3f0548-r1  
kmod-nat46-6.12.50.2025.04.23~04923c51-r1  
kmod-nf-conntrack-6.12.50-r1  
kmod-nf-conntrack6-6.12.50-r1  
kmod-nf-flow-6.12.50-r1  
kmod-nf-ipt-6.12.50-r1  
kmod-nf-log-6.12.50-r1  
kmod-nf-log6-6.12.50-r1  
kmod-nf-nat-6.12.50-r1  
kmod-nf-reject-6.12.50-r1  
kmod-nf-reject6-6.12.50-r1  
kmod-nfnetlink-6.12.50-r1  
kmod-nft-bridge-6.12.50-r1  
kmod-nft-compat-6.12.50-r1  
kmod-nft-core-6.12.50-r1  
kmod-nft-fib-6.12.50-r1  
kmod-nft-nat-6.12.50-r1  
kmod-nft-netdev-6.12.50-r1  
kmod-nft-offload-6.12.50-r1  
kmod-nls-base-6.12.50-r1  
kmod-nls-cp437-6.12.50-r1  
kmod-nls-iso8859-1-6.12.50-r1  
kmod-nls-ucs2-utils-6.12.50-r1  
kmod-nls-utf8-6.12.50-r1  
kmod-oid-registry-6.12.50-r1  
kmod-phy-aquantia-6.12.50-r1  
kmod-ppp-6.12.50-r1  
kmod-pppoe-6.12.50-r1  
kmod-pppox-6.12.50-r1  
kmod-sched-cake-6.12.50-r1  
kmod-sched-core-6.12.50-r1  
kmod-scsi-core-6.12.50-r1  
kmod-slhc-6.12.50-r1  
kmod-tcp-bbr-6.12.50-r1  
kmod-thermal-6.12.50-r1  
kmod-tun-6.12.50-r1  
kmod-udptunnel4-6.12.50-r1  
kmod-udptunnel6-6.12.50-r1  
kmod-usb-acm-6.12.50-r1  
kmod-usb-common-6.12.50-r1  
kmod-usb-core-6.12.50-r1  
kmod-usb-ehci-6.12.50-r1  
kmod-usb-net-6.12.50-r1  
kmod-usb-net-cdc-ether-6.12.50-r1  
kmod-usb-net-cdc-mbim-6.12.50-r1  
kmod-usb-net-cdc-ncm-6.12.50-r1  
kmod-usb-net-huawei-cdc-ncm-6.12.50-r1  
kmod-usb-net-qmi-wwan-6.12.50-r1  
kmod-usb-net-rndis-6.12.50-r1  
kmod-usb-ohci-6.12.50-r1  
kmod-usb-ohci-pci-6.12.50-r1  
kmod-usb-printer-6.12.50-r1  
kmod-usb-serial-6.12.50-r1  
kmod-usb-serial-option-6.12.50-r1  
kmod-usb-serial-qualcomm-6.12.50-r1  
kmod-usb-serial-sierrawireless-6.12.50-r1  
kmod-usb-serial-wwan-6.12.50-r1  
kmod-usb-storage-6.12.50-r1  
kmod-usb-storage-extras-6.12.50-r1  
kmod-usb-storage-uas-6.12.50-r1  
kmod-usb-uhci-6.12.50-r1  
kmod-usb-wdm-6.12.50-r1  
kmod-usb-xhci-hcd-6.12.50-r1  
kmod-usb-xhci-mtk-6.12.50-r1  
kmod-usb2-6.12.50-r1  
kmod-usb2-pci-6.12.50-r1  
kmod-usb3-6.12.50-r1  
kmod-usbmon-6.12.50-r1  
kmod-wireguard-6.12.50-r1  
kmod-wwan-6.12.50-r1  
ksmbd-server-3.5.4-r3  
libatomic1-14.3.0-r5  
libattr-2.5.2-r3  
libblkid1-2.41.1-r2  
libblobmsg-json20251004-2025.10.04~c163d7ab-r1  
libbz2-1.0-1.0.8-r1  
libc-1.2.5-r5  
libcap-ng-0.8.4-r1  
libcomerr0-1.47.2-r1  
libe2p2-1.47.2-r1  
libexif-0.6.25-r1  
libext2fs2-1.47.2-r1  
libf2fs6-1.16.0-r4  
libfdisk1-2.41.1-r2  
libffi-3.4.7-r1  
libffmpeg-audio-dec-6.1.3-r1  
libflac-1.4.3-r1  
libgcc1-14.3.0-r5  
libid3tag-0.16.3-r1  
libiptext-nft0-1.8.10-r2  
libiptext0-1.8.10-r2  
libiptext6-0-1.8.10-r2  
libiwinfo-data-2025.02.06~9cec6b4d-r1  
libiwinfo20230701-2025.02.06~9cec6b4d-r1  
libjpeg-turbo-3.1.1-r1  
libjson-c5-0.18-r1  
libjson-script20251004-2025.10.04~c163d7ab-r1  
liblua5.1.5-5.1.5-r11  
liblucihttp-lua-2023.03.15~9b5b683f-r1  
liblucihttp-ucode-2023.03.15~9b5b683f-r1  
liblucihttp0-2023.03.15~9b5b683f-r1  
liblz4-1-1.10.0-r1  
liblzo2-2.10-r4  
libmbedtls21-3.6.4-r1  
libmbim-1.32.0-r1  
libmnl0-1.0.5-r1  
libmount1-2.41.1-r2  
libncurses6-6.4-r3  
libnftnl11-1.3.0-r1  
libnl-core200-3.11.0-r1  
libnl-genl200-3.11.0-r1  
libnl-tiny1-2025.10.03~feca1d34-r1  
libogg0-1.3.5-r1  
libopenssl-conf-3.5.4-r1  
libopenssl-legacy-3.5.4-r1  
libopenssl3-3.5.4-r1  
libpcre2-10.46-r1  
libpthread-1.2.5-r5  
libqmi-1.36.0-r1  
libqrtr-glib-1.2.2-r3  
libreadline8-8.3-r1  
librt-1.2.5-r5  
libsmartcols1-2.41.1-r2  
libsqlite3-0-3.50.4-r1  
libss2-1.47.2-r1  
libstdcpp6-14.3.0-r5  
libubox20251004-2025.10.04~c163d7ab-r1  
libubus-lua-2025.10.04~ad2768bb-r1  
libubus20251004-2025.10.04~ad2768bb-r1  
libuci20250120-2025.10.04~a0720953-r1  
libuclient20201210-2025.10.03~dc909ca7-r1  
libucode20230711-2025.09.29~1090abb1-r1  
libudebug-2025.09.28~5327524e  
libusb-1.0-0-1.0.27-r1  
libustream-openssl20201210-2025.10.03~5a81c108-r1  
libuuid1-2.41.1-r2  
libvorbis-1.3.7-r2  
libxtables12-1.8.10-r2  
logd-2025.10.03~c75525a5-r1  
lsblk-2.41.1-r2  
lua-5.1.5-r11  
luci-25.148.69691~0a09ae1  
luci-app-aria2-25.163.60953~ae5d91d  
luci-app-atinout-1.0.2-r20250106  
luci-app-commands-25.163.60953~ae5d91d  
luci-app-cpu-status-0.6.1-r1  
luci-app-crontab-wizard-1.0.4-r20250924  
luci-app-disks-info-0.4.2-r1  
luci-app-drive-status-mini-0.5-r20250106  
luci-app-easyconfig-transfer-1.0.12-r20250617  
luci-app-ekooneplstat-20231220  
luci-app-filemanager-25.148.69691~0a09ae1  
luci-app-firewall-25.180.64366~472ac31  
luci-app-hd-idle-25.148.69691~0a09ae1  
luci-app-internet-detector-0.4-r1  
luci-app-ksmbd-25.148.69691~0a09ae1  
luci-app-lite-watchdog-1.0.17-r20250920  
luci-app-minidlna-25.148.69691~0a09ae1  
luci-app-modemband-1.0.29-r20250919  
luci-app-modemdata-1.0.17-r20251004  
luci-app-openvpn-25.148.69691~0a09ae1  
luci-app-p910nd-25.148.69691~0a09ae1  
luci-app-package-manager-25.180.63438~8b5dfab  
luci-app-qfirehose-1.0.0-r1  
luci-app-sms-tool-js-2.0.29-r20250609  
luci-app-used-channels-1.0.2-r20250914  
luci-app-zbt-sensors-status-1.0-r1  
luci-base-25.275.49410~a30c8d8  
luci-compat-25.163.60953~ae5d91d  
luci-i18n-aria2-de-25.271.23147~23b515a  
luci-i18n-aria2-it-25.271.23147~23b515a  
luci-i18n-aria2-pl-25.271.23147~23b515a  
luci-i18n-aria2-ru-25.271.23147~23b515a  
luci-i18n-aria2-vi-25.271.23147~23b515a  
luci-i18n-aria2-zh-cn-25.271.23147~23b515a  
luci-i18n-atinout-pl-0  
luci-i18n-base-de-25.275.49533~7911cef  
luci-i18n-base-it-25.275.49533~7911cef  
luci-i18n-base-pl-25.275.49533~7911cef  
luci-i18n-base-ru-25.275.49533~7911cef  
luci-i18n-base-vi-25.275.49533~7911cef  
luci-i18n-base-zh-cn-25.275.49533~7911cef  
luci-i18n-commands-de-25.271.23147~23b515a  
luci-i18n-commands-it-25.271.23147~23b515a  
luci-i18n-commands-pl-25.271.23147~23b515a  
luci-i18n-commands-ru-25.271.23147~23b515a  
luci-i18n-commands-vi-25.271.23147~23b515a  
luci-i18n-commands-zh-cn-25.271.23147~23b515a  
luci-i18n-cpu-status-pl-0  
luci-i18n-cpu-status-ru-0  
luci-i18n-cpu-status-zh-cn-0  
luci-i18n-crontab-wizard-pl-0  
luci-i18n-disks-info-pl-0  
luci-i18n-drive-status-mini-pl-0  
luci-i18n-easyconfig-transfer-pl-0  
luci-i18n-filemanager-de-25.271.23147~23b515a  
luci-i18n-filemanager-pl-25.271.23147~23b515a  
luci-i18n-filemanager-ru-25.271.23147~23b515a  
luci-i18n-filemanager-zh-cn-25.271.23147~23b515a  
luci-i18n-firewall-de-25.275.49533~7911cef  
luci-i18n-firewall-it-25.275.49533~7911cef  
luci-i18n-firewall-pl-25.275.49533~7911cef  
luci-i18n-firewall-ru-25.275.49533~7911cef  
luci-i18n-firewall-vi-25.275.49533~7911cef  
luci-i18n-firewall-zh-cn-25.275.49533~7911cef  
luci-i18n-hd-idle-de-25.271.23147~23b515a  
luci-i18n-hd-idle-it-25.271.23147~23b515a  
luci-i18n-hd-idle-pl-25.271.23147~23b515a  
luci-i18n-hd-idle-ru-25.271.23147~23b515a  
luci-i18n-hd-idle-vi-25.271.23147~23b515a  
luci-i18n-hd-idle-zh-cn-25.271.23147~23b515a  
luci-i18n-internet-detector-pl-0  
luci-i18n-internet-detector-ru-0  
luci-i18n-ksmbd-de-25.271.23147~23b515a  
luci-i18n-ksmbd-it-25.271.23147~23b515a  
luci-i18n-ksmbd-pl-25.271.23147~23b515a  
luci-i18n-ksmbd-ru-25.271.23147~23b515a  
luci-i18n-ksmbd-vi-25.271.23147~23b515a  
luci-i18n-ksmbd-zh-cn-25.271.23147~23b515a  
luci-i18n-lite-watchdog-pl-0  
luci-i18n-minidlna-de-25.271.23147~23b515a  
luci-i18n-minidlna-it-25.271.23147~23b515a  
luci-i18n-minidlna-pl-25.271.23147~23b515a  
luci-i18n-minidlna-ru-25.271.23147~23b515a  
luci-i18n-minidlna-vi-25.271.23147~23b515a  
luci-i18n-minidlna-zh-cn-25.271.23147~23b515a  
luci-i18n-modemband-pl-0  
luci-i18n-modemband-zh-cn-0  
luci-i18n-modemdata-it-0  
luci-i18n-modemdata-pl-0  
luci-i18n-modemdata-ru-0  
luci-i18n-openvpn-de-25.271.23147~23b515a  
luci-i18n-openvpn-it-25.271.23147~23b515a  
luci-i18n-openvpn-pl-25.271.23147~23b515a  
luci-i18n-openvpn-ru-25.271.23147~23b515a  
luci-i18n-openvpn-vi-25.271.23147~23b515a  
luci-i18n-openvpn-zh-cn-25.271.23147~23b515a  
luci-i18n-p910nd-de-25.271.23147~23b515a  
luci-i18n-p910nd-it-25.271.23147~23b515a  
luci-i18n-p910nd-pl-25.271.23147~23b515a  
luci-i18n-p910nd-ru-25.271.23147~23b515a  
luci-i18n-p910nd-vi-25.271.23147~23b515a  
luci-i18n-p910nd-zh-cn-25.271.23147~23b515a  
luci-i18n-package-manager-de-25.275.49533~7911cef  
luci-i18n-package-manager-it-25.275.49533~7911cef  
luci-i18n-package-manager-pl-25.275.49533~7911cef  
luci-i18n-package-manager-ru-25.275.49533~7911cef  
luci-i18n-package-manager-vi-25.275.49533~7911cef  
luci-i18n-package-manager-zh-cn-25.275.49533~7911cef  
luci-i18n-qfirehose-pl-0  
luci-i18n-qfirehose-zh-cn-0  
luci-i18n-sms-tool-js-pl-0  
luci-i18n-sms-tool-js-ru-0  
luci-i18n-sms-tool-js-zh-cn-0  
luci-i18n-used-channels-pl-0  
luci-i18n-zbt-sensors-status-pl-0  
luci-lib-base-25.148.69691~0a09ae1  
luci-lib-ip-25.148.69691~0a09ae1  
luci-lib-jsonc-25.148.69691~0a09ae1  
luci-lib-nixio-25.268.46512~3ee5ad3  
luci-lib-px5g-25.148.69691~0a09ae1  
luci-lib-uqr-25.148.69691~0a09ae1  
luci-light-25.148.69691~0a09ae1  
luci-lua-runtime-25.275.49396~c62117c  
luci-mod-admin-full-25.148.69691~0a09ae1  
luci-mod-network-25.273.63889~bad9c56  
luci-mod-status-25.275.49372~18786c5  
luci-mod-system-25.159.68111~65bdfc6  
luci-proto-3g-25.148.69691~0a09ae1  
luci-proto-ipv6-25.247.44965~183ab68  
luci-proto-mbim-25.148.69691~0a09ae1  
luci-proto-ncm-25.148.69691~0a09ae1  
luci-proto-ppp-25.148.69691~0a09ae1  
luci-proto-qmi-25.148.69691~0a09ae1  
luci-proto-wireguard-25.167.41097~2604b55  
luci-ssl-openssl-25.148.69691~0a09ae1  
luci-theme-bootstrap-25.275.47511~788e470  
mbim-utils-1.32.0-r1  
mhz-2023.06.17~11aac239-r2  
minidlna-1.3.3-r1  
mkf2fs-1.16.0-r4  
modemband-20250928-r1  
modemdata-20250919-r1  
mt7981-wo-firmware-20250917-r1  
mtd-26  
netifd-2025.09.30~ecca21ca-r1  
nftables-json-1.1.5-r1  
odhcp6c-2025.10.03~96d9e0b6-r1  
odhcpd-ipv6only-2025.09.27~bc9f9d93-r1  
openssl-util-3.5.4-r1  
openvpn-easy-rsa-3.2.1-r1  
openvpn-openssl-2.6.14-r3  
openwrt-keyring-2024.11.01~fbae29d7-r1  
opkg-2024.10.16~38eccbb1-r1  
p910nd-0.97-r14  
ppp-2.5.2-r2  
ppp-mod-pppoe-2.5.2-r2  
procd-2025.10.04~3b3501ab-r1  
procd-seccomp-2025.10.04~3b3501ab-r1  
procd-ujail-2025.10.04~3b3501ab-r1  
qfirehose-1.5.1-r1  
qlog-1.5.18-r1  
qmi-utils-1.36.0-r1  
resolveip-2  
rpcd-2025.10.03~cfb93f10-r1  
rpcd-mod-file-2025.10.03~cfb93f10-r1  
rpcd-mod-iwinfo-2025.10.03~cfb93f10-r1  
rpcd-mod-luci-20240305-r1  
rpcd-mod-rrdns-20170710  
rpcd-mod-ucode-2025.10.03~cfb93f10-r1  
smartmontools-7.5-r1  
smartmontools-drivedb-7.5-r1  
sms-tool-2023.09.21~1b6ca032-r1  
sysinfo-20210313  
terminfo-6.4-r3  
ubi-utils-2.2.1-r1
uboot-envtools-2025.07-r1
ubox-2025.10.03~c75525a5-r1
ubus-2025.10.04~ad2768bb-r1
ubusd-2025.10.04~ad2768bb-r1
uci-2025.10.04~a0720953-r1
uclient-fetch-2025.10.03~dc909ca7-r1
ucode-2025.09.29~1090abb1-r1
ucode-mod-digest-2025.09.29~1090abb1-r1
ucode-mod-fs-2025.09.29~1090abb1-r1
ucode-mod-html-1
ucode-mod-log-2025.09.29~1090abb1-r1
ucode-mod-lua-1
ucode-mod-math-2025.09.29~1090abb1-r1
ucode-mod-nl80211-2025.09.29~1090abb1-r1
ucode-mod-rtnl-2025.09.29~1090abb1-r1
ucode-mod-ubus-2025.09.29~1090abb1-r1
ucode-mod-uci-2025.09.29~1090abb1-r1
ucode-mod-uloop-2025.09.29~1090abb1-r1
uhttpd-2025.10.03~ebb92e6b-r1
uhttpd-mod-ubus-2025.10.03~ebb92e6b-r1
umbim-2025.10.04~2939b7d0-r1
unzip-6.0-r9
uqmi-2025.07.30~7914da43-r2
urandom-seed-3
urngd-2025.10.03~f17e33d9-r1
usb-modeswitch-2025.10.04~9b4d0a6e-r1
usign-2025.10.03~c4c72b1b-r1
webconsole-1.000-r1
wget-ssl-1.25.0-r1
wifi-scripts-1.0-r1
wireguard-tools-1.0.20250521-r1
wireless-regdb-2025.07.10-r1
wpad-basic-mbedtls-2025.08.26~ca266cc2-r1
wsdd2-2023.12.21~b676d8ac-r2
wwan-2019.04.29-r6
xtables-nft-1.8.10-r2
zlib-1.3.1-r1
```
</details>

### Useful AT commands (for Quectel modems)
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
