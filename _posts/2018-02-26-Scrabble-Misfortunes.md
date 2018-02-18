---
title: Scrabble Misfortunes
author: Jeremy
permalink: /scrabble-misfortunes
date: 2018-02-26
---

My family and I play a lot of Scrabble, which is a word game where you have to use tiles with letters on them to make words on the board. The board containes multipliers that also give you more points, as well as the tiles themselves, which each have a certain number of points associated with them.

In Scrabble, you usually want to start first, because the first person to play gets to double the points they make. For example, if they played the word FISH, which gives a total of $4+1+1+4=10$ points, their score would be twenty points. As such, being first is a nice boost to get you started in the game.

Recently though, one of my family members had two games where they were the first to start, and during both of these games, they couldn't actually play a word! This is because there were no vowels in the initial seven tiles they picked. Consequently, they couldn't play a word, since we don't recognize any word that doesn't contain a vowel. This meant that they had to skip their turn on both occasions, which obviously frustrated them.

This got me thinking: how likely was this to happen? In other words, was this event something that happened oftem? I couldn't remember having this happen before this brief spell of bad luck, so I thought this would be a good application of conditional probability.

There are 100 tiles in total in the game of Scrabble. Out of those 100 tiles, 54 of them are consonants (I'm counting the two blank tiles as vowels, since they can be used as vowels if needed). Then, if we let $A$ be the event that I don't pick any vowels in seven letters, then this is equal to saying that I want to pick *only* consonants. If we apply some basic counting principles from discrete mathematics, then we know that the total number of ways to get seven consonants from fifty-four tiles is $54 \choose 7$. Similarly, the number of ways to pick seven letters from the total bag of tiles is $100 \choose 7$. Finally, since it is probably safe to assume that there's an equally likely chance of picking any given tile, the probability of picking only consonants is then:
$$
\begin{equation}
	P(A) = \frac{54 \choose 7}{100 \choose 7} \approx 0.011.
\end{equation}
$$
In other words, there's about a one-in-one-hundred chance of being unlucky and not being able to start the game. I'd say that this probably matches fairly well with my experience, though I do seem to have noticed this happen more as of recently. Perhaps I'm simply seeing events now that I've focused on them.