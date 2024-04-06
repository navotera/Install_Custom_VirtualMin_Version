# Description 
This will install the virtuamin with the 7.10 version with the Nginx as webserver
This only compatible with Ubuntu 18, 20, 22
See the `install_with_apt` in the `install.sh` and the last line that is modified to install the expected version.
This only install webmin,usermin,virtualmin and its theme. Other apps as default installed by that. 


## How to install 

```
wget https://raw.githubusercontent.com/navotera/Install_Custom_VirtualMin_Version/master/install.sh && sh install.sh --minimal --force --hostname opensynergic.com --bundle LEMP | tee /var/log/webmin_install.log
```

## Other installed package 
1. Nginx 
2. MariaDB



## Version : 
1. webmin_2.105
2. usermin_2.005
3. virtual-server-7.10.0