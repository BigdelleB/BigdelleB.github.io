---
layout: post
title: Jan, 14, 2021
category: DailyUpdates
---

Last night I stumbled upon an interesting profile on Linkedin while looking for some potential developers to hire. I found a gentlemen who has about a decade experience in blockchain dev, ethereum and DApps, pretty much exactly what I'm looking for. We got on the phone and had a positive conversation.

I realized during the call though that I haven't hashed out one element, how to actually go about making a market.

Let me backtrack a bit...
My DApp is nothing more than a Token (inheriting ERC20), and then some basic logic. The token has one unique element, it has a gameID associated with it. This gameID can last for a while but once the game ends, a new one comes by. 

The problem is that once the game dies, the token with the unique gameID is fundamentally a new coin. This means that I cannot be hosted on an exchange because they would need to continue to add a new coin for the corresponding game. At the root of it, ERC20 tokens are ALL IDENTICAL, my game would not work with ERC20 because eventually a game ends.

Now I was looking around briefly and there is a solution, use an ERC721 standard and manage all transactions on a marketplace in my game. ERC721 is like the exact opposite of ERC20, each token is unique and has unique identifiers. This would allow for the ticket functionality to still work, send me ETH, I'll send you ERC721 tokens. Then you take these tokens and you need to either send them back to me for another lottery ticket. My website can have a button to Buy A Ticket and one to Exchange A Ticket. 

The question that I am struggling with is the marketplace though. Once a user has tokens, how the hell do they sell? I need to look into this and figure this out sooner rather than later because the marketplace functionality is a big part of this whole project. My token is neither ERC20 or ERC721, it is like a long lived ERC721 token or a really annoying ERC20 token because it dies and lives so rapidly.

The gist of the problem is that ERC721 tokens need to trade for ETH and it has to be an open market. What I imagined is to have a realtime updating price plot and then a simple option to list an amount of tokens desired and a price to buy or sell at. Then there would be some match making to fulfill that order

There are some promising open source [links](https://medium.com/coinmonks/how-to-implement-an-erc721-market-f805959ddcf) of people who make ERC721 markets and its not too heavy in code.

This is going to take some creativity to solve.