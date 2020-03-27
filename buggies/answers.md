a5 answers:

BUGGY1:
- the isEmpty() function doesn't properly determine whther or not the deck is empty
- this could be due to accidentally setting size == 1 or anything besides 0 

BUGGY2:
- the size() function in the deck class doesn't properly return the size of the deck
- they may have messed up the size value in the deck constructor, or changed the size somewhere they weren't supposed to

BUGGY3:
- there's a problem with the shuffle() method in the deck class
- the method returns the same unshuffled deck, when it should return a newly shuffled deck
- this may be because the coder put the wrong variables into the set function for the array list, which is what I did the first try, e.g. (cards.set(k, cards.get(r)) instead of the incorrect: cards.set(r, cards.get(k)))

BUGGY4:
- something is wrong with the deal() function in the deck class
- this could either be an error with how they set up their deal method, or it could be that they set the size of the deck to one less then it is earlier on, possibly in the constructor or something (e.g. size = 51 intead of 52), which would cause the size-- to return cards at a size of 0 rather than 1, which is what it should return

BUGGY5:
- this could be a problem with the size of the array list, or potentially a problem with one of the many for loops in the deck class
- according to the assertation, the error seems to be held in the shuffle() method of the deck class, or it at least effects the functionality of the shuffle() method
- in one of the for loops, it is likely that instead of setting the nstance variable to start at 0 and go to 51, it starts at 1 and goes to 52, or any one value off type of an error