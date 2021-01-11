---
layout: post
category: Blog_Post
title: Game Plan & Staying Accountable
---

## Background
I'm making this blog/website/whatever to act both as a journal to document my progress and struggles as well as to keep myself accountable. I know myself, putting down my thoughts on paper, or the internet in this case, keeps me focused on whatever I am doing. 

## My Project
Before I go into it, I want to explain a little bit about who I am. I promise that this will tie together in the end.

Generally speaking, there are 3 distinct paths in Electrical Engineering:
1. Analog
2. "Software" aka CS, aka fake ECE who has some degree of identity crisis.
3. Signals/Math

If you prioritize money, you take option 2. If you're hardcore, wicked smaht, and have a love for op-amps, you take option 1.

That leaves the Signals/Math guys, the black sheep of the ECE world that inevitably go into Analog or Software in order to make a living. At Cornell, My friends and I were hardcore in the Signals/Math world. I did it for 2 reasons, 1 is that I nearly failed my microelectronics course early in my sophomore year that scared me away from Analog, and 2 is that I found genuine intellectual interest from my Signals and Mathy courses. When it came time to graduate, I still felt that I had a lot to learn and I went into a Part time Master's program through JHU to study Applied Math. 

At this time in my life, there are a couple of factors that are working to influence me into a particular direction. The biggest driver is that I hated my job. I'll probably write up a post to go more into this eventually but for now just leave it as me not being happy in my first job (so unique, right?). At the same time, I'm also going into the belly of the beast and seeing how the ecosystem of federal subcontractors operate and make their money. Finally, I'm also going deeper into graduate studies in Mathematics. I decide around this time that I want to ultimately be my own boss, making money from something I find intellectually stimulating.

Skip forward a few months, I am in Iraq as a Technical Program Manager. This is in a civilian role, I never served, I was never in uniform, I am a normal civilian who was effectively "loaned out" to go over to Iraq to do some work. We're working ~16 hour days with spurts of being busier than I've ever been in my life and times when there is literally nothing to do but bullshit. During these bullshitting sessions, I had an idea to develop a "DApp", or decentralized App, on the ethereum blockchain. My DApp would be the technologically cooler version of a lottery, and use all of the fun math concepts I worked on a Cornell and Hopkins.

## A Dope Dapp
I will link the white paper when I get a chance, for now I'll just describe it. Imagine if I wanted to make a lottery in software, what would I need? I think that you would need 3 main ingredients:

1. A trusted lottery body.
2. A way to buy lottery tickets.
3. A financial incentive to actually purchase a ticket. 

Well with the ethereum blockchain, or any blockchain, we have a way to satisfy ingredient 1. Blockchains contain ledgers of every transaction and these are approved by the community, while there are ways to attack a Proof of Work algorithm, it's insanely difficult on any large enough blockchain and even if it somehow did happen, there would be massive ramifications that would make my stupid problems insignificant.

Ethereum and it's solidity development language make ingredient 2 a breeze for a decent developer or even an ECE who just wants to read articles and do math. The ecosystem to buy and sell is there and the implementation is easy enough.

My idea, is the solution to ingredient 3. I propose an ERC20 compliant token (aka a cryptocurrency that is built on the Ethereum network) that has a game ID linked to it. This Game ID will increment whenever a new game starts and the old one finishes. A token for game n has no value in game $k /neq n$, same as how a lottery ticket cannot. 
My idea, is the solution to ingredient 3. I propose an ERC20 compliant token (aka a cryptocurrency that is built on the Ethereum network) that has a game ID linked to it. This Game ID will increment whenever a new game starts and the old one finishes. A token for game n has no value in game k!=n, same as how a lottery ticket is worthless after that particular lottery it was purchased for has a winner. When a game starts, a random number of lottery tickets are born into existence for that specific game number and these are all sent to a wallet (my wallet), to be distributed. A player who wants to play in the lottery can pay me and I will send him a random number of tokens. He may get lucky and receive 10 million tokens or be unlucky and only get 10. This player now can exchange his tickets on an open market of other players, for ideally a profit relative to what he paid me, or he can "burn" some tokens in exchange for another swing at the lottery. 

This market goes on with buying and selling until a random condition is met. I haven't decided yet but for now just imagine that every transaction has a chance to end the game. Then you want to buy and sell tickets before the game ends and they have no value. There is a second mechanism to help the game be actively played, the cost of a lottery ticket will raise every time one is purchased. An early users might pay /$1 per ticket, as the supply grows due to more tickets being generated I want to avoid the costs dropping so I will raise the tickets price so a ticket after 10k transactions might be $5.

Eventually the game will end, and users can either make a profit, which would be reflected in their ethereum wallets from exchanging ETH for lottery tokens to burn or even hold, or they can lose it all. It's "stat-sy", it is technical and unlike most of my ideas, I have the ability to develop this one.

## Goals for this blog
I think this idea can go somewhere and I want a way to stay on top of my progress so I can follow my own progression and deliver status updates to myself. I want daily status updates with code problems, goals and whatever I worked on that day to be documented. It can feel like a day was a waste when I'm stuck on some stupid bug but in reality it's just a day closer to the finished product. This blog/journal will help me a ton to stay organized and motivated.
