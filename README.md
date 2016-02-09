# Infinite PuTTY Tunnel ([download ipt.exe][current-release])
*Infinite PuTTY Tunnel* allows you to quickly open persistent ssh tunnels from your system tray using [PuTTY][putty].

## Features

- **Quick:** Start and stop ssh tunnels [defined in PuTTY][putty-config-ssh-portfwd] from the system tray.
- **Persistent Tunnels:** Automatically start previously active tunnels when ipt.exe is launched.
- **Watchdog:** Restart tunnels that close unexpectedly.
- **Secure:** No support for password based authentication because it is insecure.
- **Department Of Redundancy:** *TODO:* Keep track of open tunnels and prevent multiple tunnels from listening on the same port

## Screen Shots

![](screen-shots/SystemTray-Menu.png)
![](screen-shots/SystemTray-CurrentTunnels.png)

## Installation

1. Download and install the .NET 4.6.1 Framework. Most computers will already have this installed via Windows Update.
2. [Download][putty-installer] and install the latest version of PuTTY.
3. [Download][current-release] and install the latest version of *Infinite PuTTY Tunnel*.

## Configuration

1. [Configure your tunnel][putty-config-ssh-portfwd] using putty.exe and [save it as a session][putty-config-session].
2. [Configure Pageant][putty-pageant-cmdline-command] to start ipt.exe after your keys are loaded.
3. Using PuTTY, Ensure that the session works and does not trigger any interactive prompts.
4. Begin using *Infinite PuTTY Tunnel* to automatically start and maintain your tunnel.

## History
This software is a fork of *PuTTY Tunnel Manager*. The [original][downstream] appears to be no longer maintained.
This program is nearly a complete rewrite of the original *Putty Tunnel Manager*. I've made many changes and have done my best to improve the reliability and code quality of this software.

[current-release]: https://github.com/dietsche/infinite-putty-tunnel/releases/latest/
[downstream]: https://github.com/joeribekker/putty-tunnel-manager
[putty]: http://www.chiark.greenend.org.uk/~sgtatham/putty/
[putty-installer]: http://the.earth.li/~sgtatham/putty/latest/x86/putty-installer.exe
[putty-config-ssh-portfwd]: http://the.earth.li/~sgtatham/putty/latest/htmldoc/Chapter4.html#config-ssh-portfwd
[putty-config-session]: http://the.earth.li/~sgtatham/putty/latest/htmldoc/Chapter4.html#config-session
[putty-pageant-cmdline-command]: http://the.earth.li/~sgtatham/putty/latest/htmldoc/Chapter9.html#pageant-cmdline-command
