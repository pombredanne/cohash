## Source code of following paper: ##

_Coherent parallel hashing_

Ismael Garcia, Sylvain Lefebvre, Samuel Hornus, Anass Lasram

ACM Transactions on Graphics (Proceedings of SIGGRAPH Asia), Vol. 30(6), 2011

http://www.ismaelgarcia.org/papers/cohash_siga2011

## Abstract ##

Recent spatial hashing schemes hash millions of keys in parallel, compacting sparse spatial data in small hash tables while still allowing for fast access from the GPU. Unfortunately, available schemes suffer from two drawbacks: Multiple runs of the construction process are often required before success, and the random nature of the hash functions decreases access performance.
We introduce a new parallel hashing scheme which reaches high load factor with a very low failure rate. In addition our scheme has the unique advantage to exploit coherence in the data and the access patterns for faster performance. Compared to existing approaches, it exhibits much greater locality of memory accesses and consistent execution paths within groups of threads. This is especially well suited to Computer Graphics applications, where spatial coherence is common. In absence of coherence our scheme performs similarly to previous methods, but does not suffer from construction failures.
Our scheme is based on the Robin Hood scheme modified to
quickly abort queries of keys that are not in the table, and to preserve coherence. We demonstrate our scheme on a variety of data sets. We analyze construction and access performance, as well as cache and threads behavior.