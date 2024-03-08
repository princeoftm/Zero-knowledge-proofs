A merkle tree is a mathematical data structure that is composed of hashes of different blocks of data which serves as a summary of all the transactions in a block(also known as Hash Tree).

How do Merkle trees work?
They are calculated by creating hashing pairs until there is only one left

Every leaf node is a hash of transactional data, and the non-leaf node is a hash of its previous hashes.
 _Merkle trees are in a binary tree, so it requires an even number of leaf nodes. If there is an odd number of transactions, the last hash will be duplicated once to create an even number of leaf nodes._

Merkle trees have three benefits:

It provides a means to maintain the integrity and validity of data.
It helps in saving the memory or disk space as the proofs, computationally easy and fast.
Their proofs and management require tiny amounts of information to be transmitted across networks.

