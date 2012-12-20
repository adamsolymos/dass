dass
====

Delayed Application Starter Script, written in BASH.

This is shockingly simple BASH script for starting applications with few seconds delay. It can be useful, when the loading of your windowing system is too long or uncertain (as in my case) because a couple of background application tries to start up.

Edit your ~/.dass/config file, add each starter command to a separate line. Empty lines, and comment lines (beginning with #) will be ignored. Then you need only to add this script to your Startup Applications, this will load the configured apps after a few seconds.

The default delay is 15 seconds, but it can be controlled by the first command line argument (as an integer):

```/path/to/dass 10```

Sample config file:
```
# First app
my.app -a -b -c
# Favorite terminal
gnome-terminal
```
