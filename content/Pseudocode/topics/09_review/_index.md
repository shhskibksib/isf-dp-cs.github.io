---
title: Review
weight: 10
# draft: true
---

# Review

This page contains information and coding exercises for all our pseudocode topics: `variables`, `loops`, `arrays`, `parallel arrays`, `searching`, `methods`, `sorting`,`collections`.

Open up the [pseudocode compiler](http://ibcomp.fis.edu/pseudocode/pcode.html) in a new tab. You will be using this website to complete the exercises below.

{{<aside>}}
Make sure you are never using `output` or `return` inside an `if` statement! Instead, use a variable to store the `output`/`return` value, and `output`/`return` it at the end.
{{</aside>}}

<!-- ## Choosing Your Level
You can choose whether you want to work at Level 1 or Level 2. 

**Level one is review for what we've already learned.**
**Level 2 is quite a complex challenge - more than can be  done in just 1 class period.**

Choose wisely. If you want to choose Level 2, you must first complete 1 exercise from Level 1 and paste it into your lab log to prove your understanding.

## Level 1 -->

<br>

---


## Conditionals, Loops, Mod 

{{<aside>}}
Remember, you can use `a mod b` or `a%b` to find the remainder after integer division `a//b`. If the remainder is 0, that means `a` is evenly divisible by `b`.  
{{</aside>}}

{{< code-action "Write a method that outputs a checkerboard pattern of `#` and `_`.">}} 
> input: number of rows, number of columns
> return: none

example output:
```java
#_#_#
_#_#_
#_#_#
_#_#_
#_#_#
```

<br>

---


## Collections, Array, Search, Mod

A number is prime if it cannot be evenly divided by any number besides 1 and itself. For example 5 is prime, and can only be evenly divided by 5 and 1.    

To check if `n` is prime, you can try dividing it by every number lower than `n`. If you are able to evenly divide it, it is not prime. If you try every number and none work, then it is prime.

{{< code-action "Write a method that determines whether or not a number is prime.">}}
> input: a number
> return: true/false

{{< code-action "Write a method that searches through a collection. Each time it finds a prime number, it should add that prime number to a new array. It should return that array.">}}
> input: a collection of numbers
> return: an array of all the primes found in the collection

<br>

---


## Collections, Arrays, Loops

{{< code-action "Write a method that transfers the elements of a collection into an array, but in the opposite order.">}} 

> input: a collection
> return: an array, which contains the same elements but in the opposite order


<br>

---


## Selection Sort, Collections

We cannot swap easily within a `Collection`, so to sort a `Collection`, you can create a brand new collection. The new collection will store the new, sorted collection.

{{< code-action "Write a method that uses selection sort to create a new, sorted collection.">}} 

> input: a collection
> return: a new collection, which contains the same elements but ordered



<!-- 
## Level 2

### Poker Challenge

This exercise comes from [project euler](https://projecteuler.net/problem=54)

In the card game poker, a hand consists of five cards and are ranked, from lowest to highest, in the following way:

*   **High Card**: Highest value card.
*   **One Pair**: Two cards of the same value.
*   **Two Pairs**: Two different pairs.
*   **Three of a Kind**: Three cards of the same value.
*   **Straight**: All cards are consecutive values.
*   **Flush**: All cards of the same suit.
*   **Full House**: Three of a kind and a pair.
*   **Four of a Kind**: Four cards of the same value.
*   **Straight Flush**: All cards are consecutive values of same suit.
*   **Royal Flush**: Ten, Jack, Queen, King, Ace, in same suit.

The cards are valued in the order:  
2, 3, 4, 5, 6, 7, 8, 9, 10, Jack, Queen, King, Ace.

If two players have the same ranked hands then the rank made up of the highest value wins; for example, a pair of eights beats a pair of fives (see example 1 below). But if two ranks tie, for example, both players have a pair of queens, then highest cards in each hand are compared (see example 4 below); if the highest cards tie then the next highest cards are compared, and so on.

Consider the following five hands dealt to two players:

| Hand | Player1                                         | Player2                                          | Winner   |
|------|-------------------------------------------------|--------------------------------------------------|----------|
| 1    | 5H 5C 6S 7S KD  Pair of Fives                   | 2C 3S 8S 8D TD Pair of Eights                    | Player 2 |
| 2    | 5D 8C 9S JS AC Highest card Ace                 | 2C 5C 7D 8S QH Highest card Queen                | Player 1 |
| 3    | 2D 9C AS AH AC Three Aces                       | 3D 6D 7D TD QD Flush with Diamonds               | Player 2 |
| 4    | 4D 6S 9H QH QC Pair of Queens Highest card Nine | 3D 6D 7H QD QS Pair of Queens Highest card Seven | Player 1 |
| 5    | 2H 2D 4C 4D 4S Full House With Three Fours      | 3C 3D 3S 9S 9D Full House with Three Threes      | Player 1 |

The file, [poker.txt](https://projecteuler.net/resources/documents/0054_poker.txt), contains one-thousand random hands dealt to two players. Each line of the file contains ten cards (separated by a single space): the first five are Player 1's cards and the last five are Player 2's cards. You can assume that all hands are valid (no invalid characters or repeated cards), each player's hand is in no specific order, and in each hand there is a clear winner.

How many hands does Player 1 win? -->

<br>

---



## Deliverables

{{< deliverables >}}
Paste all your code in your Code Log

<!-- Complete the [Exit Ticket](https://docs.google.com/forms/d/e/1FAIpQLScgcYSCyOc-9A60yAu78deLLUhKunf9wPlE_D1hJHy12Hzq1Q/viewform?usp=sf_link) -->

{{< /deliverables >}}