Anonymity
======
It's very important to remain anonymous when performing a pentest, this way it's harder to track you back

TOR and Proxychains
======
You can use TOR proxy to camouflage your IP address and use Proxychains to run any software trough the proxy
```
//Install TOR
apt-get install tor

// Run any program on the proxy
proxychains nmap -u 127.0.0.1
```