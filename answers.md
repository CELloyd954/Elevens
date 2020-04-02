a7 questions:

1) 
- a deck of cards
- a table

2) 
- needs to create a deck with 52 cards (traditional deck), then create a board/table, then allow the player to select, unselect, and move cards to different positions, while counting the remaining deck size, and approving or disapproving if the two cards selected to replace either add up to eleven or are the jack queen king triplet
- players need to be able to click the replace button, which will take two remaining cards out of the deck, place them in the selected or empty spots, and decrease the remaining deck size by either 2 or 3
- the game needs to realize when the game is won or lost, and restart or end it

3)
- it's a lot to look over, but it doesn't seem like the class does everything that I stated above, and some of the classes are obviously empty because I'll have to do them later

4)
a. line 206, under most of the other functions and directly under the anotherPlayIsPossible() function
b. the isLegal() function and the anotherPlayIsPossible() function
c. 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8
  --------------------------------------
   2 | 4 | 5 | 8 |   |   |   |   |

d. 
public static printCards(ElevensBoard board) {
 	List<Integer> cIndexes = board.cardIndexes();
 	/* Your code goes here. */
 	for (int k = 0; k < cIndexes.length; k++) {
 		System.out.println(cards[cIndexes.get(k)].toString());
 	}
}

e. isLegal(), since it needs to make sure that there is even two or three cards that can be put through the containsPairSum11() or containsJQK() method