# CTF riceteacatpanda.wtf – Challenge #That's a Lot of Stuff . . .

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

É nos apresentado uma string de números e letras.

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution1_That's%20a%20Lot%20of%20Stuff.png)

Tal conteúdo é um hexadecimal[1], devido a sua organização posicional ser base 16 utlizando números e letras.

Convertemos para Texto e o retorno é um Octal[2] cuja a sua organização posicional é base 8.  

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution2_That's%20a%20Lot%20of%20Stuff.png)

Convertemos o Octal para Texto e nos retornou uma string/hash desconhecida:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution3_That's%20a%20Lot%20of%20Stuff.png)

Identificamos o tipo de string/hash:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution4_That's%20a%20Lot%20of%20Stuff.png)

Convertemos o base64[3] para texto e nos retornou a flag:

![](/RiceTeaCatPanda/2020/Cryptography/That's%20a%20Lot%20of%20Stuff%20.%20.%20./Solution5_That's%20a%20Lot%20of%20Stuff.png)

```
The flag : rtcp{c0nv3rs10ns_ar3_4_c00L_c4ts}

```

## Glossary
1. Este sistema é muito utilizado para demonstrar números binários de uma forma mais compacta.

2. O sistema octal foi muito utilizado no mundo da computação, como uma alternativa mais compacta do sistema binário, na programação em linguagem de máquina.

3. Base64 é um método para codificação de dados para transferência na Internet (codificação MIME para transferência de conteúdo). É utilizado frequentemente para transmitir dados binários por meios de transmissão que lidam apenas com texto
