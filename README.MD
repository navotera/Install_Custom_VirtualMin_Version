# Descrription 
This will install the virtuamin with the 7.10 version. 
This only compatible with Ubuntu 18, 20, 22
See the `install_with_apt` in the install.sh that is modified to install the expected version.


## How to install 

```
wget https://raw.githubusercontent.com/navotera/Install_Custom_VirtualMin_Version/master/install.sh && sh install.sh --minimal --force --hostname opensynergic.com | tee /var/log/webmin_install.log
```

## Version : 
1. webmin_2.105
2. usermin_2.005
3. virtual-server-7.10.0