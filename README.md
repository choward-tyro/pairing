  #Tennis
  
  Write a class that tracks the current score in a tennis match.  The class should receive the input of the player that has scored a point, and it should return a string describing the current score within a set.
   
  In real tennis, a game is won by the first player to win four points in total with at least two more than their opponent.  Scores start at 0 ("love") and progress through 15, 30 and 40.  If both players are tied at 40, then the score is called "deuce".  In this case, the player winning the next point is said to have "advantage".  They can win the game if they win the next point, otherwise the score goes back to "deuce".  A set is won by the first player to win at least six games with at least two more than their opponent.  If both players reach six games, then a "tie-break" is played to determine the set.
   
  For the purposes of this exercise:
   
  - Ignore the terms "love" and "deuce", and simply use the numbers 0, 15, 30 and 40.  Use "Adv" for "advantage".  
  - Ignore the convention used in real tennis that the player serving the game has their score listed first.  Instead, always list player 1's score before player 2's.
  - Ignore tie-breaks.  Instead, the set is won by the first to six games.
  
  For example, a match might start along the following lines:
  
  | Point won by | Current score |
  |--------------|---------------| 
  | N/A | games: 0-0, current game: 0-0 |
  | Player 1 | games: 0-0, current game: 15-0 |
  | Player 1 |	games: 0-0, current game: 30-0 |
  | Player 2 |	games: 0-0, current game: 30-15 |
  | Player 1 |	games: 0-0, current game: 40-15 |
  | Player 1 |	games: 1-0, current game: 0-0 |
  | Player 2 |	games: 1-0, current game: 0-15 |
  | Player 2 |	games: 1-0, current game: 0-30 |
  | Player 2 |	games: 1-0, current game: 0-40 |
  | Player 1 |	games: 1-0, current game: 15-40 |
  | Player 1 |	games: 1-0, current game: 30-40 |
  | Player 1 |	games: 1-0, current game: 40-40 |
  | Player 2 |	games: 1-0, current game: 40-Adv |
  | Player 1 |	games: 1-0, current game: 40-40 |
  | Player 1 |	games: 1-0, current game: Adv-40 |
  | Player 1 |	games: 2-0, current game: 0-0 |