# mpv_flatpak
mpv player flatpak

```
flatpak --user remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak -y --user install flathub \
                    org.freedesktop.Sdk/x86_64/20.08 \
                    org.freedesktop.Platform/x86_64/20.08
git clone https://github.com/fastrizwaan/mpv_flatpak.git
cd mpv_flatpak
flatpak-builder --install --user --force-clean build-dir io.mpv.Mpv.yml 
```
