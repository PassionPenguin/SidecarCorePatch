Enables Sidecar support on MacOS Catalina 10.15 Beta on non Apple supported devices.
----

Since the last update by Apple the non modifying version of this patch doesn't work anymore.

Have a look [here](https://twitter.com/stroughtonsmith/status/1136413491462594560/photo/1) weather your device is not supported.

Modifying the system brings a certain risk with it. That is why it recommended to backup your system before trying to patch.

By running this patch you take full responsibility for your system, we do not come up for any damage done by this patch. Use it at own risk!

Said that we can start now :D

* Backup `/System/Library/PrivateFrameworks/SidecarCore.framework/Versions/A/SidecarCore` in case something goes wrong.

* Disable [SIP](https://en.wikipedia.org/wiki/System_Integrity_Protection). Check status with `$ csrutil status`

* clone this repo `$ git clone http://dev.zeppel.eu/luca/SidecarCorePatch.git`

* run the patch as root `$ sudo swift patch.swift`

* reboot


Please open issues if something doesn't work!

Testing
----
Beta 19A546d ✅

Beta 19A558d ⚠️ Not tested, please open an issue waether it works or not.

Beta 19A573a ✅



Known issues
----
* #1 Permission issue - read only
* #2 Can't use Sidecar - due to "newer MacOS needed" error **fixed**
