---
title: "The MAGIC of Modernization: An Introduction"
date: 2026-04-07
description: "We're talking Application Modernization today with the help of a Trading Card Game"
thumbnail: "/images/MTG_Modernization_1.png"
---

![The MAGIC of Modernization](/images/MTG_Modernization_1.png)

## What does Modernization mean?
When I first started my career, I was at a major commerical bank whose colors are blue and white. I got into their engineering program fresh out of college, and very quickly took on some deep leadership types of roles. I spent the majority of my time in Home Lending Technology, which was cool. The technology stack was pretty verbose and ironically, old. The internal system that drove the end-to-end of their pipeline was written on a language called Progress 4GL. I'm pretty sure that's not ACTUALLY its name, but the name is something like OpenEdge Advance Business Language or something. Anywho, that language was older than I am. Within the mega-class of that codebase was a comment at the top of the file talking about the change some engineer made. Wanna guess when that change was dated? 3 days before I was born, which, fun fact, is an icebreaker I use quite often.

Anyway. Code that's 3 days older than me, which at the time of writing this is 33 years old. Does that mean the code should be modernized? Yes, it does. But does it ACTUALLY mean it needs to be modernized? All jokes aside, no, not necessarily.

Having that's 33+ years old driving the backbone of your business doesn't necessarily mean that you need to immediately run to bank and pull money out to fund a modernization effort. Smart modernization comes out of business and/or technical necessity, not just chasing new technologies or trends for the sake of doing so.

To me, Modernization sits as a cornerstone of business and technology infrastructure. Sort of like how when you do the laundry, you're never actually done, because the clothes you're wearing are technically dirty. To modernize effectively, you need to treat the facets of the technology solution you'd like to modernize as roadmap deliverables, directly how you'd treat the ability to use OCR to scan a document as a new technology deliverable dreamed up by a product owner.

So when do you start? How do you start? Why do you start? Do you hire? Do you split capacity for your team? Do you just not do it? What about the server room in the broom closet? Do we go to the cloud? How do we get to the cloud? Which cloud do we use? How do you cut over to a new modernized system without the entire business grinding to a halt? Great questions. To answer them, lets talk about a little game called Magic the Gathering.

## What's Magic the Gathering?
Magic the Gathering is an extremely expensive card game which is, again, older than me. When I say extremely expensive, it's expensive relative to what it is: text and pictures printed onto little pieces of cardboard. Below is the definition of Magic from Wikipedia: 

> "Players in a game of Magic represent powerful dueling wizards called Planeswalkers. Each card in a player's deck represents either a magical spell, which can be used to their advantage, or a Land, which creates the resource (mana) to be able to cast their spells. Instant and Sorcery cards represent spells a player may cast for a one-time effect, whilst Creature, Artifact, Enchantment, Planeswalker, and Battle cards remain on the Battlefield to provide long-term advantage. Typically, a player defeats their opponent(s) by reducing their life totals to zero, which is commonly accomplished through combat damage by attacking with creatures. Many other sources of damage exist in the game, in addition to alternative win-conditions which do not check life totals"
>
> — Wikipedia contributors. (n.d.). [Magic: The Gathering](https://en.wikipedia.org/wiki/Magic:_The_Gathering). Retrieved March 3, 2026.

For the sake of comparing two things I'm extremely passionate about, I'll probably generalize and gloss over a TON of edge cases in Magic the Gathering for the sake of simplicity.

There's formats of the game that are extremely expensive, where players after decks of cards worth $60k+, and on the other extreme end, decks where players aren't allowed to spend more than $10. That's all find and great, to each their own, but what does Magic after to do with Modernization?

There's a particular format of Magic, called Elder Dragon Highlander. To some individuals who haved played this game for an extremely long time, we know it as EDH. Others, especially with the surge in popularity, know it just generally as "Commander".

> "The Commander format has each player provide a 100-card deck, using cards from any printed sets excluding those that are banned, with the requirement that each card outside basic lands must be unique, in contrast to normal Magic decks that allow up to four copies of a card from the game's current base and expansion sets. The Commander format serves as a casual alternative to normal competitive play."
>
> — Wikipedia contributors. (n.d.). [Magic: The Gathering Commander](https://en.wikipedia.org/wiki/Magic:_The_Gathering_Commander). Retrieved March 3, 2026.

I primarily play Commander/EDH. I've played off and on my entire "life", but primarily picked it up again with a group of friends in 2022 and have been playing rather frequently since. To recap on only the important information, there's two types of cards in Magic: Lands, and Spells. Lands exhaust when you use them, and become available your next turn. You use lands by "tapping" them to indicate to the table they've been used - meaning you just turn them sideways. You "tap" lands in order to pay for spells. Some spells you can only play on your turn, some you can play on your opponents turn, there are spells that let you play cards you can't normally play on an opponents turn, on an opponents turn, and so on. The stack gets rather complicated, but at the end of the day for the sake of this conversation, it'll stay extremely high-level.

Also, yes, I mentioned the stack. Most Senior+ programmers are familiar with a computers stack. They operate PRACTICALLY exactly the same. We'll get to all of that, I promise.

## What does Magic have to do with Modernization?
Great question. Thank you for asking. For turns in Magic, it's relatively straight forward. There's 7 main phases of your turn in Magic:

1. Untap
2. Upkeep
3. Draw
4. Main Phase 1
5. Combat
6. Main Phase 2
7. End Phase

I've included a great helpful cheatsheet from Reddit that helps define these in a nutshell. Phases have phases within them. There's only certain phases you can take certain actions in - like for example you can only play a land during Main Phase 1 and Main Phase 2.

![MTG Turn Phase Order](/images/MTG_Phase_Order.png)

EDH is a 4 player game in its most basic of form, which goes around the table in clockwise order (unless you're a rebel). Each player in turn order gets access to their own turn that consists of the 7 above listed phases. Once eery players goes through their first turn of 7 phases, the game naturally moves on to "turn 2".

With all of this said, I think we're in a position where we can discuss what exactly Magic the Gathering has to do with Application Modernization. It's extremely important when you think about "implementing" Modernization, that you plan accordingly.

## Modernization Planning and Magic the Gathering Planning
In Magic the Gathering, when you're building a commander deck, you're typically following a simple rule: build the deck for fun, but play the deck to win. There ARE tournaments for this once casual-only format, but for the most part the above rule still applies across all brackets of the game. When you're building a commander deck, you're required to build around the color identify of your commander. There are 5 colors in total: Green, Blue, Red, Black, and White. Each of these by definition of their own flavor of "how they win", but over time that definition has become EXTREMELY blurred.

![MTG Color Pie](/images/MTG_Color_Pie.jpg)

*Source: Dan Felder, [How to Bake a Color Pie](https://danfelder.net/2018/07/29/how-to-bake-a-color-pie/)*

Your deck-building and gameplan needs to be effectively built around the Magic Color Pie, your Commander, and your decks overall winning strategy. That said, you're trying to execute your decks overall winning strategy while simultaneously stopping your opponents from winning the game with their OWN win strategy, which immediately introduces extremely complex dynamics on a game that uses a stack equivocal to programming. When building out a deck and gameplan, you're primarily focused on:

1. What is my gameplan?
2. How do I plan around my gameplan?
3. How does my gameplan change against the other 3 players and THEIR gameplans?
4. What is even going on?

Similarly to magic, you can plan as much as your heart desires, but sometimes even the best of planning doesn't prepare you for making on-the-fly decisions during application/architecture modernization. That said, planning is the first step, and application modernization efforts need to be effectively planned around to be successful, which has an infintitely-finite number of considerations that need to be made before you actually start, including:

1. What portion of your application stack are you looking to modernize?
2. Why do you want to modernize? Is it for Security reasons? Scaling? Is your current application stack not maintainable? Do you want to be in a position to adopt new technologies like AI?
3. Do you want to build a new modern solution, or do you buy a new modern solution?
    - If you choose to build a new solution, how do you choose a technology?
    - If you choose to buy a new solution, how do you choose your partner?
4. How do you do the modernization in combination with supporting your current business initiatives?
5. How do you do your rollout? Do you do a bigbang cutover? Blue/Green Deployments?
6. How do you measure success? Does the Technology definition of success match the Business definition of success?
7. How do you ANSWER all of these questions?
8. What do you do when the goals of modernization change mid-flight?

I've got a ton more questions that can be included, but all things considered this seems like a great way to get started in having our conversation.

## Key Modernization components



