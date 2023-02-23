# HPCA'23

## AB-ORAM - Constructing adjustable buckets for space reduction in Ring ORAM
* Main problem area - by snooping on the **memory access patterns**, an adversary can **identify sensitive information**. ORAM obfuscates the memory requests from user program but is EXPENSIVE.
* Though ORAM solves this issue, it degrades the performance of an application. Ring ORAM is a new primitive that improves on the performance. (NEWER BASELINE)
* Main challenge - space consumption is very high. (classic performance vs space tradeoff?)

## Efficient Distributed Secure Memory with Migratable Merkle Tree
* Main problem area - Hardware-assisted enclaves with memory encryption are pervasive in modern CPUs. eg: Intel SGX/TDX, AMD SEV, ARM CCA.
* For distributed shared memory, the enclaves fall short. One simple way is to use cryptography at the application level eg: SSL. 
* Problem - a clear lack of a distributed secure memory which is efficent + secure! 
* Vocabulary - distributed secure memory, distributed confidential computing, merkel trees, integrity forest

# ASPLOS'23
## Characterizing and Optimizing End-to-End Systems for Private Inference

## Open Questions: 
* How would the embedding memory accesses in DLRM inference be connected to RowHammer and Cache Timing attacks? Q1 - are these attacks going to apply in DLRM infernece? Q2 - If yes, what kind of privacy concerns could arise? Q3 - For the super-hot embedding entires (like Criteo TB dataset), does it make the attack very easy to perform? 

## To check: 
* Systems for Parallel and Distributed Large-Model Deep Learning Training - https://arxiv.org/pdf/2301.02691.pdf
* 
