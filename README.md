# flatpak for kiss

TODO

- [x] Clean up builds.
- [x] Document needed changes to community packages.
- [ ] Remove as many dependencies as possible.
    - Bye bye `fuse2`, `mozjs`, `polkit`, `libuuid`, etc.
    - [ ] libcap?
    - [ ] ???????
- [x] Finalize dependencies.

INSTRUCTIONS

```
# NOTE: You must have user namespaces enabled in your kernel.

# NOTE: The community repository must also be enabled.
-> git clone https://github.com/dylanaraps/kiss-flatpak
-> export KISS_PATH=/path/to/kiss-flatpak/flatpak:$KISS_PATH

-> kiss b flatpak
-> kiss i flatpak

-> flatpak remote-add --user --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-> flatpak install --user gimp
-> flatpak run --user org.gimp.GIMP
```
