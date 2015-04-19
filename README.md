# lightdm-webkit-win7
windows 7 theme for lightdm-webkit

Works with Xubuntu 14.04.1

sudo apt-get install lightdm-web-greeter

sudo update-alternatives --install /etc/alternatives/lightdm-webkit-theme lightdm-webkit-theme /usr/share/lightdm-webkit/themes/win7 90

cd /etc/alternatives

sudo ln -s /etc/lightdm/lightdm-webkit-greeter.conf lightdm-gtk-greeter-config-derivative

cd /usr/share/lightdm-webkit/themes

sudo ln -s /etc/alternatives/lightdm-webkit-theme default

cd /etc/lightdm

sudo vi lightdm.conf
[SeatDefaults]
greeter-session=lightdm-webkit-greeter

cd /usr/share/lightdm-webkit/

git clone https://github.com/tweakmy/lightdm-webkit-win7.git win7

sudo reboot

##Do it at your own risk##
