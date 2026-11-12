# blink
Make one of the front LED's on a host blink for a few seconds so you can find it!
I've got a stack of Raspberry PI's and no labels - this script flashes the power LED on the front for a few seconds so I know I'm physically dealing with the correct system. Should work on most systems and OS variants.

## Installation

From this checkout:

```sh
sudo install -o root -g root -m 0755 blink /usr/local/sbin/blink
sudo install -d -o root -g root -m 0755 /usr/local/share/man/man8
sudo install -o root -g root -m 0644 blink.8 /usr/local/share/man/man8/blink.8
sudo mandb
```

Run `sudo blink 5` to flash for five seconds, `blink --help` for usage, or
`man blink` for the manual. Controlling the LED requires root privileges.
