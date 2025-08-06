# ad

sudo apt update

sudo apt install build-essential dkms linux-headers-$(uname -r)

sudo mount /dev/cdrom /media/cdrom

sudo /media/cdrom/VBoxLinuxAdditions.run

sudo reboot


# Create mount point (if needed)
sudo mkdir -p /media/cdrom

# Mount the ISO (try both /dev/sr0 and /dev/cdrom)
sudo mount /dev/sr0 /media/cdrom || sudo mount /dev/cdrom /media/cdrom

# Check if mounted correctly
ls /media/cdrom
