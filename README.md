# shadowsocks_n900
# shadowsocks-libev for Nokia N900 Device

I build it and looks like it can run on N900 device.

If you need it, you can try it like below.

1. Download  target_rootfs_n900.tgz to N900 Device.
2. tar xvzf target_rootfs_n900.tgz -C /opt/
3. Add a line "/opt/target_rootfs/lib" to /etc/ld.so.conf
4. Run ldconfig
5. You can run /opt/target_rootfs/bin/ss-* programs now.

thanks.




