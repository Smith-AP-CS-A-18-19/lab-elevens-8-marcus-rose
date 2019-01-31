# Elevens 8

Follow the instructions provided for Activity 8 in the student lab guide. This is more of an exploratory lab, so you will not need to copy any of your previous code into the repo. Answer the questions from the Student Guide in this document and ensure that you save and push the repo. You have one week to complete this lab.

1. Discuss the similarities and differences between *Elevens*, *Thirteens*, and *Tens*.

    <!-- All the games involve a board and a deck of cards. Methods like deal(), deckSize(), and isEmpty() are used across all three games as well. There are some methods that need to be implemented differently depending on the game (isLegal() and anotherPlayIsPossible()). This is why they are overridden in the subclass: so they could be used differently depending on the game.

      -->

2. As discussed previously, all of the instance variables are declared in the `Board` class. But it is the `ElevensBoard` class that “knows” the board size, and the ranks, suits, and point values of the cards in the deck. How do the `Board` instance variables get initialized with the `ElevensBoard` values? What is the exact mechanism?

    <!-- Through the super() method, the instance variables in the subclass are able to be initialized through the super class. The values are passed through the constructor to the superclass.

     -->

3. Now examine the files `Board.java` and `ElevensBoard.java`, found in this repository. Identify the `abstract` methods in `Board.java`. See how these methods are implemented in `ElevensBoard`. Do they cover all the differences between *Elevens*, *Thirteens*, and *Tens* as discussed in question 1? Why or why not?

    <!--  The two abstract methods in Board.java are isLegal() and anotherPlayIsPossible(). These methods do cover the differences because the methods can be shared throughout all three games whereas the overlapping methods are abstract. This allows them to be implemented in their respective games.

    -->
