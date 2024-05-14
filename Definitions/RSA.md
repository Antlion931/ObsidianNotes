#pwr #cybersecurity 

[[RSA]] is public key cryptosystem, what means it uses public and private key. It can be used to encrypt/decrypt data or to digitally sign it. 

## Generating keys
1. Choose two large prime numbers $p$ and $q$.
2. Compute module of operations as $n = p \times q$.
3. Compute Carmichael's totient function $\phi (n) = (q - 1)(p - 1)$
4. Choose $e$ where $1 < e < \phi(n)$ and $e$ is coprime to $\phi(n)$.
5. Determine $d = e^{-1} ( \mod \phi(n))$.

Your public key is pair $(n, e)$.
Your private key is pair $(n, d)$.

## Encryption
We split data into block $m$ with value less then $n$. Then we encrypt block with:

$c = m^e(\mod n)$

## Decryption
On every block we use:

$m = c^d(\mod n)$

## Digital signature
To digitally sign an document we can firstly encrypt it with our private key, and other person can decrypt it with our public key.

