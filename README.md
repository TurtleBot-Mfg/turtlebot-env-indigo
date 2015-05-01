# turtlebot-env-groovy
This package configures the Ubuntu environment for operation as a TurtleBot.
The files in this package should work with any recent version of ROS.

---

root/usr/share/glib-2.0/schemas/org.gnome.settings-daemon.plugins.power.gschema.override
  Change power settings to prevent the laptop from entering suspend/hibernate when lid is closed.

root/etc/init.d/ps3joy
  starts instance of pd3joy.py

root/etc/modprobe.d/blacklist-kinect.conf
  Disables Kinect kernel driver to avoid conflict with OpenNI userland driver

root/etc/udev/rules.d/57-kobuki.rules
  Kobuki FTDI Driver

root/etc/udev/rules.d/60-create.rules
  iRobot Create FTDI Driver


DEB_DIVERT_EXTENSION = .turtlebot-env
root/etc/bluetooth/main.conf.turtlebot-env
root/etc/default/avahi-daemon.turtlebot-env
