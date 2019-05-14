# shadowsocks_n900
# shadowsocks-libev for Nokia N900 Device

tar xvzf target_rootfs_n900.tgz -C /opt/

add a line "/opt/target_rootfs/lib" to /etc/ld.so.conf
run ldconfig

then you can run /opt/target_rootfs/bin/ss-* programs.

thanks.




