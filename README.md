# flatpak for kiss

INSTRUCTIONS

```
# NOTE: You must have user namespaces enabled in your kernel.
-> CONFIG_USER_NS=y

# NOTE: The community repository must also be enabled.
-> git clone https://github.com/dylanaraps/kiss-flatpak
-> export KISS_PATH=/path/to/kiss-flatpak/flatpak:$KISS_PATH

-> kiss b flatpak
-> kiss i flatpak

-> flatpak remote-add --user --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-> flatpak install --user gimp
-> flatpak run --user org.gimp.GIMP
```

ISSUES

- [ ] No audio in flatpaks expecting a running PulseAudio server on the host.


OTHER FLATPAK REPOSITORIES

- https://flatpak.citra-emu.org/
