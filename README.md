# Helium-Auto-Reboot-for-M5Stack

Here is the start of a M5Stack UIFlow to monitor your Helium hotspot and automatically reboot it if it goes off line.  You will need to edit the hotspot name.

This script is designed to control a [M5Stack ATOM Socket Kit (HLW8023)](https://shop.m5stack.com/collections/m5-atom/products/atom-socket-kit-hlw8023-jp-us?variant=39295191744684).  The script will monitor a Helium Hotspot using the Helium API and will turn the hotspot off and back on automaticlly (rebooting it) if it shows as being "offline" on the API call.

- Helium-Auto-Reboot-for-M5Stack.m5f - this is the [UIFlow](https://flow.m5stack.com) source.
- Helium-Auto-Reboot-for-M5Stack.py  - this is the generated python script.

You can toggle the power to the hotspot by pushing the button on the M5Atom.  Green means the power is on, red means the power is off.  Once an hour, the Atom will check the API to see if the hotspot is online.  If it's not, it will cycle the poewer.  It will also cycle power once ever 24 hours for a daily reboot.
