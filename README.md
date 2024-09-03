# Templates Wireguard
You can use this templates to create your own peer.conf and server.conf file.
    
## Reminder to create keys
Create your base64-encoded public and private keys :
```
sudo umask 077
```
```
sudo wg genkey > privatekey
```
    
The derive your public key from your private key
```
sudo wg pubkey < privatekey > publickey
```
    
When all at once:
```
sudo wg genkey | tee privatekey | wg pubkey > publickey
```
### For more informations check the quick start section from Wireguard website
https://www.wireguard.com/quickstart/
