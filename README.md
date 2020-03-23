# iSight Disabler

Legacy homepage: http://techslaves.org/isight-disabler/

techslaves.org’s iSight Disabler is an AppleScript that automates the process of disabling and enabling the iSight driver(s) in OS X. The goal is to prevent applications from using the built-in USB iSight found in Macbooks, Macbook Pros and iMacs. I’ve seen various queries online about how to disable the iSight and while the answer was already hanging around, there wasn’t a simple way to disable and enable the iSight without going to the command line.

## Instructions

The traditional or legacy AppleScript method is less convenient since Apple introduced [System Integrity Protection](https://support.apple.com/en-us/HT204899) (SIP) in 10.11. To use the AppleScript on modern macOS systems, you essentially have to disable SIP to run the AppleScript. However, it's probably best to keep SIP enabled most of the time so that turns into a dance of disabling SIP, running the AppleScript and then enabling SIP again.

The [configuration profile or "mobileconfig"](https://github.com/rthomson/isight-disabler/blob/master/camera-disabler.mobileconfig) option is the recommended way to disable the camera on modern macOS. See [Apple documentation on managing profiles](https://support.apple.com/en-ca/guide/profile-manager/pm9cz84lqi/mac) for details on how to install or remove the camera-disabler.mobileconfig profile.
