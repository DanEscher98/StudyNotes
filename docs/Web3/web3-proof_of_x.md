# Proof of X

The term refers to a consensus mechanism or validation method in a distributed
system that establishes trust, agreement and prevents malicious
behavior without relying on a central authority. It ensures that
only valid transactions are added to the blockchain, while
discouraging attacks.


1. A **set of participants** $P$ (nodes, validators, miners)
2. A **condition** $C_X$ that must be satisfied for validation
3. A **validation function** $V(p)$ for verifying that a $p \in P$
   satisfies $C_X$
4. Thus, the essence of any $\text{Proof of } X$ mechanism boils down to:

$$M_X := V(p) = \left\{
\begin{array}{ll}
    1 &\text{if } p \text{ satisfies } C_X,\\
    0 &\text{otherwise}
\end{array}\right.$$


## Examples

- `Proof of Work`: its condition $C$ is tied to **computation effort**. The
participants must find a **nonce** $n$ such that the hash of the block and
nonce is less than a certain target value $T$. This process ensures the
difficulty of mining new blocks, requiring energy expenditure to secure the
network. Its used by `Bitcoin`.

$$C_\text{PoW}: H(\text{block}, n) < T$$


- `Proof of Stake`: its condition $C$ is based on ownership of stake in the
network. To being eligible to be selected as a validator, participants must own
a stake $S_p$ that is higher than some threshold $S_\text{min}$. By tying
validation rights to economic stake, `PoS` incentivizes good behavior by
imposing potential financial losses for dishonest actions. Different versions
of this mechanism are implemented by `Cardano`, `Ethereum 2.0` and `Polkadot`.

$$C_\text{PoS}: S_p > S_\text{min}$$


- `Proof of History`: its condition $C$ is based on the participant's ability
to cryptographically prove that certain evets happened in a specific sequence
in time. In order to do this, the participant must generate a verifiable
cryptographic sequence $S$ where each element of the sequence depends on the
previous element. It provides a cryptographic clock for the network, enabling
efficient consensus in combination with `PoS`. `Solana` implements this model.

$$C_\text{PoH}: S = \{ s_1, s_2, s_3, \ldots, s_n \} \text{ where } s_{i+1}=H(s_i)$$ 
