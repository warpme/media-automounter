media-automounter
===========================

Utility to auto-mount / un-mount external storage and execute predefined script at
mount / un-mount event.

How it works:

1. When attaching /detaching ext. storage, script calls 90-media-automount.rules
udev rule.

2. Udev rule calls shell script /usr/bin/media-automount.

3. Shell script looks at media-automount.conf to see how and where to mount ext. storage.

4. After successful mount, media-automount calls to execute <disk label>.mount.script

enjoy

