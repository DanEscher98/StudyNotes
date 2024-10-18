# ICP Concepts

## Flow of a message on ICP

1. The `message` goes to one of the `boundary nodes` (RPC nodes)
2. The `boundary node` routes the message to the `subnet` that
   hosts the target `smart contract`
3. The `consensus algorithm` of that `subnet` adds the message to
   a new `block` in the `subnet`'s blockchain
4. The `message` is added to the input queue of the target `smart
   contract`
5. The `smart contract` executes the `message`

- Each *ICP* `subnet` has a fixed `public key`
- *I
CP* actively gargbage collects old `blocks`
- *ICP* runs `smart contracts` in parallel (like microservices)
- `smart contracts` can have their own `secret keys`
- 
