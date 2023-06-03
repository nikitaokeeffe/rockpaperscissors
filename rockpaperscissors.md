# Rock–paper–scissors

*From Simple English Wikipedia, the free encyclopedia*

**Rock, paper, scissors** (RPS) is a two-person hand game. It is often used as a selection method in a similar way to coin flipping or drawing straws to randomly select a person for some purpose. However, unlike truly random selections, it can be played with skill if the game extends over many sessions, as a player can often recognize and exploit the non-random behavior of an opponent.

Sportsmen often use RPS (both officially and unofficially, in place of a coin toss) to decide on opening plays. Similarly, uncertain calls, or even the whole game in case of rain, may be so decided. It is also often used as a method for creating appropriately non-biased random results in live action role-playing games, as it requires no equipment. It is also used in some gambling sites as a form of novelty betting.

The exact name of the game can vary, with the three components appearing in a different order, or with "stone" in place of "rock". Non-English speakers may know the game by their local words for "rock, paper, scissors", although it is also known as Janken or Yakyuken in Japan, Kawi Bawi Bo in Korea, Pierre-Papier-Ciseaux in France, Ca-Chi-Pun in Chile, and in South Africa as Ching-Chong-Cha, the words used in the 'count'.

## Rules

The players both count aloud to three, or speak the name of the game (e.g. "Rock! Paper! Scissors!" or "Reaux! Sham! Beaux!"), each time raising one hand in a fist and swinging it down on the count. On the third count, or on a further beat after the third count (saying "shoot"), the players change their hands into one of three gestures, which they then "throw" by extending it towards their opponent.

* Rock is represented by a closed fist. 
* Paper is represented by an open hand. 
* Scissors is represented by the index and middle fingers extended. 

The objective is to select a gesture which defeats that of the opponent. Gestures are resolved as follows:

* Rock blunts/smashes scissors; rock wins. 
* Paper covers rock; paper wins. 
* Scissors cut paper; scissors wins.

In terms of logic, this type of game is intransitive. If both players choose the same gesture, the game is tied and played again.

In some variations of the game, the winner of each round "uses" the weapon on the opponent's weapon, to demonstrate that they have won.

RPS is frequently played in a "best two out of three" match, and tournament players often prepare sequences of three gestures ahead of time.

## Popularity
The game is famous in [Japan](https://en.wikipedia.org/wiki/Japan), [China](https://en.wikipedia.org/wiki/China), and the [United States](https://en.wikipedia.org/wiki/United_States).

Scoring

Below is an example implementation of the scoring algorithm in JavaScript:

```function rockPaperScissors(player1, player2) {
    if (player1 == player2) {
        return "Draw"
    }

    if (player1 == "rock") {
        if (player2 == "scissors") {
            return "Player 1 wins"
        }
        return "Player 2 wins"
    }
    if (player1 == "paper") {
        if (player2 == "rock") {
            return "Player 1 wins"
        }
        return "Player 2 wins"
    }
    if (player1 == "scissors") {
        if (player2 == "paper") {
            return "Player 1 wins"
        }
        return "Player 2 wins"
    }
    return "Invalid input"
}```

console.log(rockPaperScissors('rock', 'paper')) // Player 2 wins
console.log(rockPaperScissors('rock', 'rock')) // Draw
console.log(rockPaperScissors('scissors', 'paper')) // Player 1 wins
console.log(rockPaperScissors('paper', 'rock')) // Player 2 wins