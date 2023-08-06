## USAGE
###  Get and execute:  
```shell
wget -qO proxmox_toolbox.sh https://raw.githubusercontent.com/sielnet/proxmox_toolbox/main/proxmox_toolbox.sh && bash proxmox_toolbox.sh
```

###  Execute these numbers:

- 1 No-subscription Sources Configuration 
- 2 Update host & create proxmox-update command
- 6 Enable S.M.A.R.T self-tests

### Updating host & remove subscription
The script will update your host and detect if the no-enterprise source is configured, if so, remove the subscription message.
- If you still encounter it after, clear your broswer cache.
- If you update your host directly within the system, the no subscribtion message may reappear when the file gets updated.  
- In order to nerver see this again, you have to update Proxmox with one of the following options:

To start an update only, without menu or prompt:
```shell
bash proxmox_toolbox.sh -u
```
Once the tool has been used to update host, you can execute this command to fully update your host - kind of an alias of bash proxmox_toolbox.sh -u
```shell
proxmox-update
```
