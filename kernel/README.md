## linux kernel for the nanopi-r6

<i>Note: This script is intended to be run from a 64 bit arm device such as an odroid m1 or a rock 5b.</i>

<br/>

**start a screen session**
```
screen
```

<br/>

<i>compilation can take a while: it is important to run the build from a screen or tmux session so it is not interrupted</i>

<br/>

**build the kernel**
```
sh make_kernel.sh
```

<i>* note: kernel .deb package is linked in the ```kernel``` directory when the build finishes successfully</i>

<br/>

**install the kernel to mmc image**
```
cd ../debian
sudo sh install_kernel.sh
```

<br/>

