# 401 Notes-18: Cryptography

[Back to 401 Index](401-index.md)<br>

## [Encryption, decryption, and cracking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.
The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.
Encrypting a message
Imagine Caesar wants to send this message:
SECRET MEETING AT THE PALACE
Here's what that might look like encrypted:
YKIXKZ SKKZOTM GZ ZNK VGRGIK
That looks an awfully lot like gobbledygook at first, but this encrypted message is actually very related to the original text.
The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.
To make the encrypted message above, I shifted the alphabet by 6 and used this substitution table:
A	B	C	D	E	F	G	H	I	J	K	L	M	N	O	P	Q	R	S	T	U	V	W	X	Y	Z
G	H	I	J	K	L	M	N	O	P	Q	R	S	T	U	V	W	X	Y	Z	A	B	C	D	E	F
S shifts 6 letters over to Y, E shifts 6 letters over to K, etc. Here's the first word and its shifts:
S	E	C	R	E	T
Y	K	I	X	K	Z




<!-- notes here -->


[Back to 401 Index](401-index.md)