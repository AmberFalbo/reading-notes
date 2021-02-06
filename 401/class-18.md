# 401 Notes-18: Cryptography

[Back to 401 Index](401-index.md)<br>

## [Encryption, decryption, and cracking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

***History***<br>
One of the earliest encryption techniques is the **Caesar Cipher**, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.
The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.

**Encrypting a message**<br>
>Imagine Caesar wants to send this message:<br>
SECRET MEETING AT THE PALACE<br>
Here's what that might look like encrypted:<br>
YKIXKZ SKKZOTM GZ ZNK VGRGIK

The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.

>S shifts 6 letters over to Y, E shifts 6 letters over to K, etc. Here's the first word and its shifts:<br>
S	E	C	R	E	T<br>
Y	K	I	X	K	Z

**Decrypting a message**<br>
*According to historical records, Caesar always used a shift of 3. As long as his message recipient knew the shift amount, it was trivial for them to decode the message.*

>Imagine Caesar sends this message to a comrade:<br>
EHZDUH EUXWXV<br>
The comrade uses this substitution table, where the alphabet is shifted by 3.<br>
They can then decode the message with certainty. The first letter "E" was shifted by 3 from "B", the second letter "H" was shifted by 3 from "E", etc. The result is this ominous message:<br>
BEWARE BRUTUS<br>


**Cracking the cipher**
- Frequency Analysis
- Known plaintext
- Brute force

**Frequency analysis**
Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.


**Known plaintext**


## [Ceasar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher)

## [Cryptography Crash Course](https://www.youtube.com/watch?v=jhXCTbFnK8o)
**Video**

## [Introduction to Cryptography](https://thebestvpn.com/cryptography/)

## [How Computers Generate Random Numbers](https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/)




<!-- notes here -->


[Back to 401 Index](401-index.md)