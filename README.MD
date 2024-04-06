# Description 
This will install the virtuamin with the 7.10 version with the Nginx as webserver
This only compatible with Ubuntu 18, 20, 22
See the `install_with_apt` in the `install.sh` and the last line that is modified to install the expected version.
This only install webmin,usermin,virtualmin and its theme. Other apps as default installed by that. 

## Tested 
Ubuntu 20.04


## How to install 

```
wget https://raw.githubusercontent.com/navotera/Install_Custom_VirtualMin_Version/master/install.sh && sh install.sh --minimal --force --hostname opensynergic.com --bundle LEMP | tee /var/log/webmin_install.log
```


## After Installation 
If you want to login the the Webmin https, set the passwd first 
type `passwd`, the password will be used for login to the webmin site 
**https://IP_ADDRESS:10000**


## Other installed package 
1. Nginx 
2. MariaDB



## Version : 
Installed version are taken from the version_path file. 
1. Webmin_2.105
2. Usermin_2.005
3. Virtual-server-7.10.0 (Virtualmin Core)
4. Virtual min theme 9.5


## Disabled features

The script automatically disable some of the features : 
1. Mail 
2. DNS 
   
You can enable it by accesing Virtualmin -> System Settings -> Features and Plugin



## Known Error 
On installing the "CA Certificates" 
 [ERROR] Failed with error: 100
 ✘
[ERROR] Something went wrong. Exiting.
[ERROR] The last few log entries were:

**Solution** 
`dpkg --configure -a`
