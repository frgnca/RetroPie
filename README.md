# RetroPie
v4.3.2.2

es themes -> install 13pixel-metadata  
retopie setup -> install experimental package emulationstation_dev
```bash
sudo /bin/bash -c 'sed -i "s/exit 0/dmesg --console-off/" /etc/rc.local && echo "exit 0" >> /etc/rc.local && echo "" >> /boot/config.txt && echo "# Retropie" >> /boot/config.txt && echo "disable_splash=1" >> /boot/config.txt && echo "dwc_otg.lpm_enable=0 console=serial0,115200 console=tty3 root=PARTUUID=5728b712-02 rootfstype=ext4 elevator=deadline fsck.repair=yes rootwait loglevel=0 consoleblank=0 plymouth.enable=0 logo.nologo quiet vt.global_cursor_default=0" > /boot/cmdline.txt'
```
