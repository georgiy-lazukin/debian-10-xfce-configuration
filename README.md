# Live build configuration for debian xfce desktop

## Documentation

[live-build](https://live-team.pages.debian.net/live-manual/html/live-manual/index.en.html)

## Preparation

Check out packages and hooks
  - [archives](skel/archives)
  - [hooks](skel/hooks)
  - [package-lists](skel/package-lists)

Configure theme and other xfce settings for user
- [xfce-perchannel-xml](skel/includes.chroot/etc/skel/.config/xfce4/xfconf/xfce-perchannel-xml)

## Usage

```bash
# lb clean
# lb conf
# lb build
```
## Notes
Extract key
```bash
# apt-key adv —keyserver keyserver.ubuntu.com —recv-keys 36FD5529
apt-key export 36FD5529 > skel/archives/telegram.key.chroot
```
