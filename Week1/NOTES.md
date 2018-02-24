## Cryptographic Hash Functions

A [cryptographic hash function](https://en.wikipedia.org/wiki/Cryptographic_hash_function) is a special class of [hash function](https://en.wikipedia.org/wiki/Hash_function) that has certain properties which make it suitable for use in cryptography.

It is a mathematical algorithm that maps data of arbitrary size to a bit string of a fixed size (a hash) and is designed to be a one-way function, that is, a function which is infeasible to invert. 

The input data is often called the **message**, and the output (the _hash value_ or _hash_) is often called the message digest or simply the **digest**.


### Hash Function

A hash function is any function that can be used to map data of arbitrary size to data of fixed size.

The values returned by a hash function are called hash values, hash codes, digests, or simply hashes.

One use is a data structure called a hash table, widely used in computer software for rapid data lookup.

## Properties of Cryptographic Hash Functions

The ideal cryptographic hash function has five main properties:

- it is [deterministic](https://en.wikipedia.org/wiki/Deterministic_algorithm) so the same message always results in the same hash
- it is quick to compute the hash value for any given message
- it is [infeasible](https://en.wikipedia.org/wiki/Computational_complexity_theory#Intractability) to generate a message from its hash value except by trying all possible messages
- a small change to a message should change the hash value so extensively that the new hash value appears uncorrelated with the old hash value
- it is [infeasible](https://en.wikipedia.org/wiki/Computational_complexity_theory#Intractability) to find two different messages with the same hash value

> A problem that can be solved in theory (e.g. given large but finite resources, especially time), but for which in practice any solution takes too many resources to be useful, is known as an **intractable problem**. Conversely, a problem that can be solved in practice is called a _tractable problem_, literally "a problem that can be handled". The term **_infeasible_** (literally "cannot be done") is sometimes used interchangeably with intractable, though this risks confusion with a feasible solution in mathematical optimization.