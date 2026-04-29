# virtual-browser-termux

pkg update && pkg upgrade
pkg install x11-repo
pkg install xfce4 
pkg install xfce4-goodies
pkg install tigervnc
pkg install git python

git clone https://github.com/novnc/noVNC.git
git clone https://github.com/novnc/websockify.git

cd noVNC
./utils/novnc_proxy --vnc localhost:5091 --listen 6080
