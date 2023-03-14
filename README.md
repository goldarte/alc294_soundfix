# alc294_soundfix

Sound fix service for ALC294 on Ubuntu 22.04, tested on Asus Vivobook K6500Z.

Service will autostart after boot and write register data for audiocard.

## Install

1. Clone this repo: 

```bash
git clone https://github.com/goldarte/alc294_soundfix.git
```

2. Make symlinks for service and script

```bash
sudo ln -s <full path to alc294_soundfix>/sound-fix.sh sound-fix.sh
sudo ln -s <full path to alc294_soundfix>/sound-fix.service sound-fix.service
```

3. Enable service

```bash
sudo systemctl enable sound-fix
```

4. Restart system and check the sound
