# shadowsocks_n900
# shadowsocks-libev for Nokia N900 Device

It can work on N900 device.

Please try it as below.

1. Download  target_rootfs_n900.tgz to N900 Device.
2. tar xvzf target_rootfs_n900.tgz -C /opt/
3. Add a line "/opt/target_rootfs/lib" to /etc/ld.so.conf
4. Run ldconfig
5. You can run /opt/target_rootfs/bin/ss-* programs now.

thanks.




