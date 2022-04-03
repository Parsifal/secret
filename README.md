# Secret generator

A random password generator is software program or hardware device that takes input from a random or pseudo-random
number generator and automatically generates a password. Random passwords can be generated manually, using simple
sources of randomness such as dice or coins, or they can be generated using a computer.

While there are many examples of "random" password generator programs available on the Internet, generating randomness
can be tricky and many programs do not generate random characters in a way that ensures strong security. A common
recommendation is to use open source security tools where possible since they allow independent checks on the quality of
the methods used. Note that simply generating a password at random does not ensure the password is a strong password,
because it is possible, although highly unlikely, to generate an easily guessed or cracked password. In fact, there is
no need at all for a password to have been produced by a perfectly random process: it just needs to be sufficiently
difficult to guess.

A password generator can be part of a password manager. When a password policy enforces complex rules, it can be easier
to use a password generator based on that set of rules than to manually create passwords.

Long strings of random characters are difficult for most people to memorize. Mnemonic hashes, which reversibly convert
random strings into more memorable passwords, can substantially improve the ease of memorization. As the hash can be
processed by a computer to recover the original 60-bit string, it has at least as much information content as the
original string. Similar techniques are used in memory sport.

The algorithm was written for a Wikipedia article about
a [random password generator](https://en.wikipedia.org/wiki/Random_password_generator).

### Example:

```ts
const { secret } = require("secret");
secret(); // xZ5<y}EAFaJP)H?UK8ii:c5;q`xt6{:G<j^&2z>7pY]M"OuY3/eX[?(1~fHs0dWG
```

More than 1 quadrillion years needed, in order to have a 1% probability of at least one collision.

### A few values to feel the scale:

- Human lifespan: 79 years.
- Life on Earth will be impossible in ~1.1 billion years.
- Age of the Earth: ~4.543 billion years.
- Age of the Universe: ~13.799 billion years.

### The math behind

- [Birthday problem](https://en.wikipedia.org/wiki/Birthday_problem).
- [Collisions](https://en.wikipedia.org/wiki/Universally_unique_identifier#Collisions).
