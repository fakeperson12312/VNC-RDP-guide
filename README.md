# VNC_guide
So I was messing around one day with docker, and I stumbled upon this wonderful thingy: https://hub.docker.com/r/dorowu/ubuntu-desktop-lxde-vnc
It turns out to actually have a good fps if your computer is good enough (my linux comp that could run stuff wasn't good but the mac one that couldn't run alot of stuff was good)
Basically, I got a vnc/rdp way that mostly has good fps and can run alot of programs. It's even more if the operating system was linux and it supported kvm. Yes, I know about 
using VMs with multipass on docker and doing it there, along with setting KVM=N for my docker compose files, but eh ill do that later. 
# Steps
Open up a new Codespace, wait for it to boot.
Now, in the terminal, run:
```bash
docker compose up
```
On the first launch, it'll take a while to boot up and download and extract everything, and to view the progress, there's a progress bar in the terminal already,
but for a better view, go to ports, forward port 8006 (should auto-forward), open it in a new tab, and you'll see it downloading and extracting, booting up and installing.
For some reason Windows 11 doesn't work sometimes so I decided to go with windows 10, and windows 10 is better than windows 11. So wait for it to launch and boot up, the
default username is docker and password is nonexistant, as in N/A like it doesn't exist. 

After that it's pretty simple, just a windows operating system. You can rdp to it for a better connection, but for the web, just use the client that's provided. 
For some reason I can set the cores to 4 on a 2-core vm, so idk what's up with that but you still can. 
