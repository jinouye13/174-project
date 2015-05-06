# 174-project
Final project - video poker

Roles:

Veronica - create deck, shuffle deck
Isaias - take payment, handle rejected cards (see project requirements)
Jamie - score hand (recognize hands), return winnings
Carlos - write report, assist Isaias

~*Don't forget, send a summary of your work to Carlos to make it easier for him
when writing the report!!*~

//Veronica's Code
+//**CARD CLASS**\\
+Instance variables:
+- String value <--- holds the value
+- String suit <--- holds the suit
+
+public Card()
+- creates an object Card with parameters value and suits
+- Value ranges from numbers 1-13.
+
+If value is 1, value is now Ace. 
+If value is 11, value is now Jack. 
+If value is 12, value is now Queen. 
+If value is 13, value is now King. 
+Any number not 1 or 11-13 does not change its value.
+
+getSuit()
+- returns suit
+
+getValue()
+- returns value
+
+toString() 
+- combines suit and value
+ex) value + "of" + suit ---> Ace of Diamonds
+
+//**DECK CLASS**\\
+Instance variables:
+- Card[] deck <----- an array with Card objects
+- int numOfCards <----- keeps track of cards
+
+public Deck()
+- creates a card array of 52
+- String [] suits <----- initializes a string array with "Spades", "Diamonds",
+  "Clubs", "Hearts"
+
+Inner for loop creates thirteen cards with a value and a suit and adds it to the card array.
+Outer for loop repeats inner loop four times for each suit.
+
+shuffleDeck()
+- shuffles the deck by swapping cards at different positions
+
+int index <----- returns a random card's position from 0-51
+Card temp <----- a card object at position i
+
+- swaps index and temp
+
+toString()
+- String deckString <----- "New deck created\n"
+
+For loop displays each card in the deck with their value and suit.
+
+//**DECKTESTER PROGRAM**\\
+- tests to see if deck and card classes work properly
+- Deck deck <----- creates a object deck
+
+deck.shuffleDeck()
+- shuffles deck
+
+System.out.println(deck.toString())
