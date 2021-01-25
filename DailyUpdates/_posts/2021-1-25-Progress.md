---
layout: post
title: Jan, 25, 2021
category: DailyUpdates
---

# Starting the work

After some initial difficulty with payment, the project started!

Some details to immediately hash out so that the dev team can get to work:
1. Game End condition.
2. Token initial supply.
3. Token min and max range.
4. The old problem of differentiating gameID's.

The first 3 are pretty straightforward so I'll start there.

# Randomness in Solidity

You can get a PHD in randomness, and for good reason. There are countless examples of when randomness wasnt so random and people use it to exploit loopholes. [An example from a Canadian lottery](https://www.newscientist.com/article/mg21128264-900-lottery-wins-come-easy-if-you-can-spot-the-loopholes/?ignored=irrelevant).

I'm using a solidity function called Keccak256() that just returns the SHA3 hash of whatever the argument is. I honestly think it's random enough for my application and also because I'm not using randomness in a "one man takes all" type fashion, it's ok if one guy does slightly better than the rest. It doesnt really ruin the game. In less words, it's good enough.

Anyway so I use Keccak256 to randomize. The game end condition is triggered on one of two events.
1. The initial supply of tokens is exhausted.
2. if during a transaction, the following condition is held: int(keccack256(WALLET)%10^5)==1

The first point is obvious, the second is just giving a 1/100k chance of the game ending at any transaction.

Initial Supply is 100 Million.

Min token "win" is 1.

Max Token "win" is 1000.

## Differentiating between tokens of different gameID's

The old option of self destructing and spawning new ERC20 tokens is on the table but it is a bit dramatic....

I think there is an easier, less extreme, middle ground.

I'm leaning towards the following implementation:
Create a mapping when the game starts, every wallet with a non zero balance is mapped and added to the mapping upon a transfer, ticket purchase or exchange.
When the game ends, that mapping is erased and reinitialized. Wallets that try to interact that are not in the new mapping cannot participate in ticket buys or trades.

This, combined with some way to exchange ALL old tokens to get 1 ticket might be a good way to go.












