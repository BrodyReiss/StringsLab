# StringsLab

For this lab, you will create three static methods of a `FunString` class.  

1. `GuessTheString(String guess)`  

Consider a guessing game in which a player tries to guess a hidden word. The hidden word contains only capital letters and has a length known to the player. A guess contains only capital letters and has the same length as the hidden word.  
After a guess is made, the player is given a hint that is based on a comparison between the hidden word and the guess. Each position in the hint contains a character that corresponds to the letter in the same position in the guess. The following rules determine the characters that appear in the hint.  

If the letter in the guess is …   
1)	 In the same position in the hidden word,   PRINT: the matching letter
2)	In the hidden word, but in a different position,    PRINT:  "+"
3)	Not in the hidden word,   PRINT:   "*"  

For Example:  
```
//After the call to setHiddenWord(), see method 3  
FunString.setHiddenWord("HARPS");   //see the implementation of setHiddenWord below   
FunString.GuessTheString("AAAAA")   //Returns:   +A+++  
FunString.GuessTheString("HELLO")   //Returns:   H****  
FunString.GuessTheString("HEART")   //Returns:  H*++*  
FunString.GuessTheString("HARMS")   //Returns:  HAR*S  
FunString.GuessTheString ("HARPS")  //Returns:  HARPS  
```


2. `setHiddenWord(String hiddenWord)`  

You will have to set the "Hidden Word" by calling the method `setHiddenWord` in `GuessTheString` and passing the hidden word in the parameters.  



---

## When completed with the above (and if there is time) work on the method below.  

3. `removeLetter(String phrase, String letter)`  

Running FunString.removeLetter( “Apple” , “p”); will remove all instances of that letter “p” out of the String “Apple”, returning the “chopped up” String “Ale. If the letter you are trying to remove is NOT in the String, simply return the original String.   
 
```
String Example = “eat at a cool place”;  
String test = FunString.removeLetter(Example, “e”);// Returns “at at a cool plac”  
String test2 = FunString.removeLetter(test, “a”);//Returns “t t  cool plc”  
String test3 = FunString.removeLetter(Example, “z”);//Returns “eat at a cool place”  
```
