# CTF riceteacatpanda – Challenge #That's a Lot of Stuff ...

* **Category:** Cryptography
* **Points:** 275

## Challenge

> Do you want some numbers? Here, take these numbers. I don't need them anyways. I have too many numbers at home, so go on, take them. Shoves numbers towards the computer screen


> 31 34 33 20 31 35 36 20 31 32 32 20 31 35 32 20 31 34 33 20 31 31 30 20 31 36 34 20 31 35 32 20 31 31 35 20 31 30 
37 20 36 35 20 36 32 20 31 31 35 20 36 33 20 31 31 32 20 31 37 32 20 31 31 35 20 31 32 34 20 31 30 32 20 31 36 35 
20 31 34 33 20 36 31 20 37 31 20 31 35 30 20 31 34 33 20 31 35 32 20 31 31 36 20 31 34 36 20 31 31 36 20 31 30 36 
20 37 31 20 31 35 32 20 31 31 35 20 31 30 34 20 31 30 32 20 31 31 35 20 31 33 30 20 36 32 20 31 31 35 20 36 30 20 
31 34 34 20 31 31 30 20 31 31 36 20 37 31

## Solution

### Tools Used
* v2.cryptii.com

### Process

We are presented with a string of numbers and letters.

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution1_That's%20a%20Lot%20of%20Stuff.png)

This content is hexadecimal[1] digits, due to its positional organization being base 16, using numbers and letters.

We converted it to text. The returned are octal[2] digits whose positional organization is base 8.

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution2_That's%20a%20Lot%20of%20Stuff.png)

We converted Octal to Text and returned an unknown string/hash:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution3_That's%20a%20Lot%20of%20Stuff.png)

We identified the type of string/hash:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution4_That's%20a%20Lot%20of%20Stuff.png)

We converted base64[3] to text and returned the flag:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution5_That's%20a%20Lot%20of%20Stuff.png)

```
The flag : rtcp{c0nv3rs10ns_ar3_4_c00L_c4ts}

```

## Glossary
1 [hexadecimal]. This system is widely used to demonstrate binary numbers in a more compact way.

2 [octal]. The octal system was widely used in the world of computing, as a more compact alternative to the binary system, in machine language programming.

3 [base64]. Base64 is a method for encoding data for transferring over the Internet (MIME encoding for transferring content). It is often used to transmit binary data by means of transmission that deal only with text.
