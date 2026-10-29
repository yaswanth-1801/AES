<img width="1197" height="621" alt="image" src="https://github.com/user-attachments/assets/9ace617b-f9fc-47de-9c1a-345690865cee" /># EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state

# PROGRAM:
```
#include <stdio.h> 
#include <string.h> 
void xorCrypt(char *in, char *key) { 
for (int i = 0; in[i]; i++) in[i] ^= key[i % strlen(key)]; 
} 
int main() { 
char msg[] = "Yaswanth R", key[] = "secretkey"; 
printf("Original: %s\n", msg); 
xorCrypt(msg, key); 
printf("Encrypted: %s\n", msg); 
xorCrypt(msg, key); 
printf("Decrypted: %s\n", msg); 
return 0; 
} 

```
# OUTPUT:
<img width="1197" height="621" alt="image" src="https://github.com/user-attachments/assets/d8e4d80b-f6e2-4f5d-ad47-3f280eb32a5f" />



# RESULT:
The Program is executed successfully.

