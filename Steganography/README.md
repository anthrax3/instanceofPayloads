Steganography
======
Steganography is a particular branch of cryptology, and is the study of techniques for concealment of a message within another.

Steghide
======
Hide .txt message within .jpg image
```
apt-get install steghide
steghide embed -ef msg.txt -cf img.jpg
```

To extract the message:
```
steghide extract -sf img.jpg -xf secret-msg.txt
```