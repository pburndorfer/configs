# Message of the day (MOTD)

![](motd-screen.PNG)

On my raspberry pi I'm using my custom motd which shows me some stats of the system when I connect via ssh to my user.

Custom motd files can have different locations, depending on the system you use. On my raspberry pi running Raspian 10 Buster the corresponding folder is in `/etc/update-motd.d`

All script files contained in this folder will be concatenated by an automatic script operated by the OS itself which adds them up in lexicographical order. Therefore each script has a starting digit which indicates which script is added first and so on.

A detailed description can be found [here](https://ownyourbits.com/2017/04/05/customize-your-motd-login-message-in-debian-and-ubuntu/) and [here](https://wiki.ubuntu.com/UpdateMotd).

When implementing this on your own, make sure your scripts are marked as executable, otherwise they won't take effect.

Enjoy!