IntelEdison
===========

Access serial console @ J3
screen /dev/tty.usbserial-A402IWCC 115200 -L

++++
Alternate Flashing Method
Install Homebrew by running the command
type/run: ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
Install dfu-util, coreutils, and gnu-getopt
type/run: brew install dfu-util coreutils gnu-getopt
Download and extract Edison Image (Step 1 and 2 need to be done only once on the MAC OS X host)
Extract the contents of the pre-built Edison image
In your terminal change to the directory where you extracted the linux image.  Example: your directory may be different
type/run: cd ~/Downloads/edison-image-ww36-14
Run the flashall script and then plug usb cable into board
type/run: ./flashall.sh
Note:
The script can take up to 5 minutes to complete the flashing
