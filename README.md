Manjaro Numix
===========================

This is a LightDM webkit greeter theme for Manjaro Linux. Based on [LightDM Webkit Arch Theme](https://github.com/shosca/lightdm-webkit-archlinux-theme)

Installation Instructions
-------------------------
You will need lightdm as your login manager and the lightdm-webkit-greeter. You need to make the webkit greeter the default greeter. This is done by editing the lightdm configuration under:

<pre>
/etc/lightdm/lightdm.conf
</pre>

and changing the greeter-session value to lightdm-webkit-greeter. lightdm.conf should have:

<pre>
[SeatDefaults]
greeter-session=lightdm-webkit-greeter
allow-guest=false
</pre>

The second step is to install the actual theme. This is done by copying the files of this repository into the following location:

<pre>
/usr/share/lightdm-webkit/themes/manjaro-numix
</pre>

Finally, change the /etc/lightdm/lightdm-webkit-greeter.conf file to contain the following line:

<pre>
webkit-theme=manjaro-numix
</pre>

Now you can reboot and enjoy the new theme.
