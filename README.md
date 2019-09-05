Enables Sidecar support on MacOS Catalina 10.15 Beta (19A546d) on non Apple supported devices.

----

Since the last update by Apple the non modifying version of this patch doesn't work anymore.

Modifying the system brings a certain risk with it. That is why it recommended to backup your system before trying to patch.

By running this patch you take full responsibility for your system, we do not come up for any damage done by this patch. Use it at own risk!

Said that we can start now :D

* Backup `/System/Library/PrivateFrameworks/SidecarCore.framework/Versions/A/SidecarCore` in case something goes wrong.
* Disable [SIP](https://en.wikipedia.org/wiki/System_Integrity_Protection) check with `$ csrutil status`
* clone this repo `$ git clone http://dev.zeppel.eu/luca/SidecarCorePatch.git`
* run the patch as root `$ sudo swift patch.swift`