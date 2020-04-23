# flatpak for kiss

TODO

- [ ] Clean up builds.
- [ ] Document needed changes to community packages.
- [ ] Remove as many dependencies as possible.
- [ ] Finalize dependencies.

INSTRUCTIONS

```
-> git clone https://github.com/dylanaraps/kiss-flatpak
-> export KISS_PATH=/path/to/kiss-flatpak/flatpak:$KISS_PATH

-> kiss b flatpak
-> kiss i flatpak

-> flatpak remote-add --user --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-> flatpak install --user gimp
-> flatpak run --user org.gimp.GIMP
```
