---
layout: post
category: BlogPosts
title: The Ultimate Guide to the Lotto Project, A revision
---

I'm writing this in response to feedback from friends and family about my project, which I'll sometimes refer to as "The Lotto Project".

##Current State of Crypto 
Crypto right now is weird. NFT's are molten hot jet fuel, Bitcoin is in the stratosphere and there are some exciting new projects on the corner like Avalanche. The crypto team is just all over the place and we're getting to a breaking point where we leave the world of "crypto" and categories start to pop up. It's like trying to draft Simone Biles to play on Shaq's 3v3 basketball team, or signing Lionel Messi to compete with Michael Phelps in the pool because they're both athletes. Clearly the differentiation matters, Simone Biles, Messi, Phelps and Shaq are all athletes, but that distinction is no where near as important as their categorical placement.

All of this is my way of trying to say that the "maturing" crypto world is beginning to step into that world where differentiation is key, otherwise you look at this circus and it makes no sense.

One category that I've always been fascinated with is the Stable Coin like USDC (United States Dollar Coin) that is pegged at $1 by some miracle of finance by people a lot smarter than me. Take a second to think about this though, **the USDC team made a stable crypto currency**. Bitcoin's value increased by like $40k this year, NFT's are selling for $69 million dollars. The concept of stability almost seems foreign when it comes to crypto.

So I started thinking about the opposite. What if I could make a an **unstable coin**? A coin that is optimized for high variance, an always shifting mean and more excitement than a japanese game show. That's how Lotto was born.

##What is Lotto (Take 2)
I described it as a lottery before because I was coming at this from a statistics perspective and I liked the randomness aspect. However calling it a lottery leads to a lot of assumptions that make it difficult to explain to my friends and family. I find myself having to deconstruct their idea of a lottery and re explaining it in my context. 

The better way to explain it is as a **High Entropy Coin**. Say it with me, "Lotto = High Entropy Coin". 

Now I can focus on what makes it high entropy in my creatively titled next section.

###What makes Lotto a "High Entropy Token"?

So let me first say that Lotto is simply something that is referred to as a "smart contract", which is just a term for a piece of code that can do things, that's it. What can mine do?

1. Users can send the Smart contract ethereum, and the smart contract will send back a random number of Lotto. I refer to this as "buying a ticket".

The exact amount of ethereum scales with users. The first transaction cost .001 Ethereum, and it increases by .00001 Ethereum with every subsequent transaction. Some mental math, the 100th person to buy a ticket will pay .001 eth+ .00001x100 = .002 Eth. They can receive between 1, and 1000 + the number of ticket purchases. So in the same 100th person example as earlier, the 100th person to buy a ticket can get between 1 and 1100 Tokens.

So you, fellow reader, send my contract some money, and it sends you back a random number of Lotto tokens, uniformly distributed between 1 and 1000 + the number of transactions, which my smart contract keeps track of.

2. Users can send the smart contract Lotto tokens, and in exchange, the smart contract will send back a random number of Lotto. I refer to this as an "exchange".

This is essentially an exchange of a fixed amount of Lotto, which starts at 50 Lotto and increases by 1 Lotto for every exchange initiated. This user will send that amount of Lotto and will receive a random number back, from 1 to 1000 + number of tickets purchased.

Let's go through an example quickly. You are the 500th person to initiate an exchange so your cost is 50+500 = 550 Lotto, which you send to the smart contract. The smart contract verifies this event using blockchain magic (thanks ethereum) and sends you back a random number of Lotto, from 1 to 1500.

3. Every interaction with my contract, whether it be a ticket buy or an exchange, can trigger an "end game". Which means that the contract stops interacting with any old Lotto and whips up a batch of new Lotto that has a new game ID field.

This means that the players in this game are incentized to move. In other words, holding Lotto forever has a guaranteed outcome of losing money. The game becomes a Martingale, which is an optimal stopping problem. How long do you hold? Do you sell your tokens to another user? Do you try to initiate an exchange, hoping to profit?

###Economics from an engineer
I hope that the mechanics are clear, I want to dive into the economics of this a little bit now. This is coming from me, an engineer/math person who's formal finance experience was self studying for microeconomics in high school over a weekend and getting a 3 on the AP test.

My little coin, Lotto, is under a lot of pressure from 4 main forces that all fight to determine its value.

1. The increasing price of it's inherent value from an increasing price to "buy a ticket".
2. An increasing price of it's inherent value from an increasing exchange price.
3. A randomness with a sliding mean that doesn't allow for any kind of price normalization.
4. The existence of something called a "uniswap pool", these pools are just exchanges where anyone can list their weird tokens in exchange for a different token.

Side note on point 4. One of the reasons why Lotto is build on the ethereum ecosystem is to take advantage of this uniswap pool, it's really easy for any ERC20 (basically ethereum built) token to be traded.

Side side note, using coinbase to buy crypto is like asking the police to buy you drugs. The entire point of crypto is decentralization.

Anyway, let me give a hypothetical scenario.

A user interacts with the Lotto smart contract and buys a ticket, he sends .001 Eth, gets a random return of 1000 Lotto tokens, he got really lucky.

Now his cost average is 1000/.001 Eth, lets say that .001 Eth is worth $10 for simplicity. Then this user paid 1 cent per Lotto token.

Now this user lists his 1000 tokens on a uniswap pool for 1.5 cents each, a 50% return. A second user comes and has 2 options, either send .00101 Eth (remember the scaling by .00001 per transcation) for a random number of tokens, or buy 50 Lotto from the first user which is enough to initiate an exchange.

This is a very fine view of how this thing gets crazy. I'll leave it to the reader to think of how insane and complicated this can get.

And that's all folks, if you want to reach out to me with questions or comments, hit me up on twitter https://twitter.com/B_Bigdelle





















