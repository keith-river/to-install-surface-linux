# to-install-surface-linux
How to install surface-linux

wget -qO - https://raw.githubusercontent.com/linux-surface/linux-surface/master/pkg/keys/surface.asc | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/linux-surface.gpg > /dev/null

echo "deb [arch=amd64] https://pkg.surfacelinux.com/debian release main" | sudo tee /etc/apt/sources.list.d/linux-surface.list

sudo apt update

sudo apt install linux-image-surface linux-headers-surface libwacom-surface
