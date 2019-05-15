# shadowsocks_n900
# shadowsocks-libev for Nokia N900 Device

1.You can build your binary files via "build" directory.
  
  . Install toolchain from scratchbox ("http://www.scratchbox.org/documentation/user/scratchbox-1.0/html/tutorial.html")
  
  . run make in build directory
  
  . "target_rootfs" is the target files that you can used on N900 Device.
  
   
2. target_rootfs_for_n900.tgz is the binary files i build on linux mint 18 via scratchbox. It can work on N900 device.
   
   Please try it as below.

  . Download  target_rootfs_n900.tgz to N900 Device.
  
  . tar xvzf target_rootfs_n900.tgz -C /opt/
  
  . Add a line "/opt/target_rootfs/lib" to /etc/ld.so.conf
  
  . Run ldconfig
  
  . You can run /opt/target_rootfs/bin/ss-* programs now.
 
 3. If you like this, please star it!
  

thanks.




