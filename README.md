For newer controller and kernel support, this updated repo xpad-noone should be used. https://github.com/forkymcforkface/xpad-noone

## Installation

1. Unplug your Xbox devices and remove `xpad`:

```
sudo modprobe -r xpad
```

2. Clone the repository:

```
git clone https://github.com/medusalix/xpad-noone
```

3. Install `xpad-noone` using the following commands:

```
sudo cp -r xpad-noone /usr/src/xpad-noone-1.0
sudo dkms install -m xpad-noone -v 1.0
```

4. Plug in your Xbox devices and add the module if it is not loaded automatically:

```
sudo modprobe xpad-noone
```
