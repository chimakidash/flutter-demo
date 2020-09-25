* x11 forwarding setting for MAC 

```bash
$ brew install socat
$ brew cask reinstall xquartz
```

host mac reboot

```bash
$ lsof -i TCP:6000
$ socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\"
```
keep current terminal and open new terminal

```bash
$ docker build -t xeyes .
$ docker run -e DISPLAY=host.docker.internal:0 xeyes
```
open xeyes app !
