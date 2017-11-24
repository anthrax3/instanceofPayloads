Fingerprint
======
Fingerprint is one of the main techniques for collecting information about the target that we want to attack. The goal is to identify versions and applications on the target.

Netcat HTTP banner grabbing
======
Send a HEAD request to the victim
```
nc victim.com.br 80

HEAD / HTTP/1.0
```

Sometimes the server returns the name of the application (```nginx/1.10.3 (Ubuntu)```)
```
HTTP/1.1 200 OK
Server: nginx/1.10.3 (Ubuntu)
Content-Type: text/html; charset=UTF-8
Connection: close
Cache-Control: private, must-revalidate
Date: Thu, 05 Oct 2017 21:40:52 GMT
pragma: no-cache
expires: -1
...
```
