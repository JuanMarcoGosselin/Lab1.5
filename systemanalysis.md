juan-marco@JuanUbuntu:~$ whoami
juan-marco
juan-marco@JuanUbuntu:~$ id
uid=1000(juan-marco) gid=1000(juan-marco) grupos=1000(juan-marco),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users),115(lpadmin)
juan-marco@JuanUbuntu:~$ groups
juan-marco adm cdrom sudo dip plugdev users lpadmin
juan-marco@JuanUbuntu:~$ sudo systemctl list-units --type=service --stte=running
[sudo] contraseña para juan-marco: 
  UNIT                          LOAD   ACTIVE SUB     DESCRIPTION              >
  accounts-daemon.service       loaded active running Accounts Service
  avahi-daemon.service          loaded active running Avahi mDNS/DNS-SD Stack
  colord.service                loaded active running Manage, Install and Gener>
  cron.service                  loaded active running Regular background progra>
  cups-browsed.service          loaded active running Make remote CUPS printers>
  cups.service                  loaded active running CUPS Scheduler
  dbus.service                  loaded active running D-Bus System Message Bus
  gdm.service                   loaded active running GNOME Display Manager
  gnome-remote-desktop.service  loaded active running GNOME Remote Desktop
  ModemManager.service          loaded active running Modem Manager
  NetworkManager.service        loaded active running Network Manager
  packagekit.service            loaded active running PackageKit Daemon
  polkit.service                loaded active running Authorization Manager
  power-profiles-daemon.service loaded active running Power Profiles daemon
  rsyslog.service               loaded active running System Logging Service
  rtkit-daemon.service          loaded active running RealtimeKit Scheduling Po>
  snapd.service                 loaded active running Snap Daemon
  switcheroo-control.service    loaded active running Switcheroo Control Proxy >
  systemd-journald.service      loaded active running Journal Service
  systemd-logind.service        loaded active running User Login Management
  systemd-oomd.service          loaded active running Userspace Out-Of-Memory (>
  systemd-resolved.service      loaded active running Network Name Resolution
  systemd-timesyncd.service     loaded active running Network Time Synchronizat>
  systemd-udevd.service         loaded active running Rule-based Manager for De>
  udisks2.service               loaded active running Disk Manager
  unattended-upgrades.service   loaded active running Unattended Upgrades Shutd>
  upower.service                loaded active running Daemon for power manageme>
  user@1000.service             loaded active running User Manager for UID 1000
  wpa_supplicant.service        loaded active running WPA supplicant

Legend: LOAD   → Reflects whether the unit definition was properly loaded.
        ACTIVE → The high-level unit activation state, i.e. generalization of S>
        SUB    → The low-level unit activation state, values depend on unit typ>

29 loaded units listed.
lines 14-36/36 (END)
