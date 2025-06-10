# NVIDIArch

sudo pacman -S nvidia-open-dkms

From the wiki notes:
The DKMS variants are not tied to a specific kernel, as they recompile the NVIDIA kernel module for each kernel for which header files are installed.
This means that when installing dkms the kernel is passed as argurment -k 'kernel_v'

https://wiki.archlinux.org/title/NVIDIA
https://wiki.archlinux.org/title/NVIDIA/Troubleshooting

---

**Card 4070Ti 8GiB**
k= 6.15.1-arch1-2

My issue was that the game would run perfectly for 2-3h then start randomly having 50-100ms to draw frames.

Using x11 sddm session with sdl_videodriver=wayland for game itself seemed to fix this issue. + Config files used here /etc
