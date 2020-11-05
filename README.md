# StringsLab

For this lab, you will create methods of a `FunString` class.  

1. `GuessTheString(String guess)`  

Consider a guessing game in which a player tries to guess a hidden word. The hidden word contains only capital letters and has a length known to the player. A guess contains only capital letters and has the same length as the hidden word.  
After a guess is made, the player is given a hint that is based on a comparison between the hidden word and the guess. Each position in the hint contains a character that corresponds to the letter in the same position in the guess. The following rules determine the characters that appear in the hint.  

If the letter in the guess is …   
1)	In the same position in the hidden word,   PRINT: the matching letter
2)	In the hidden word, but in a different position,    PRINT:  "+"
3)	Not in the hidden word,   PRINT:   "*"  

For Example:  
```
//After the call to setHiddenWord(), see method 3
FunStrings fun = new FunStrings();

fun.setHiddenWord("HARPS");   //see the implementation of setHiddenWord below   
fun.guessTheString("AAAAA")   //Returns:   +A+++  
fun.guessTheString("HELLO")   //Returns:   H****  
fun.guessTheString("HEART")   //Returns:  H*++*  
fun.guessTheString("HARMS")   //Returns:  HAR*S  
fun.guessTheString ("HARPS")  //Returns:  HARPS  
```


2. `setHiddenWord(String hiddenWord)`  

You will have to set the "Hidden Word" by calling the method `setHiddenWord` in `GuessTheString` and passing the hidden word in the parameters.  


---

## When completed with the above (and if there is time) work on the method below.  

3. `removeLetter(String phrase, String letter)`  

Running FunString.removeLetter( “Apple” , “p”); will remove all instances of that letter “p” out of the String “Apple”, returning the “chopped up” String “Ale. If the letter you are trying to remove is NOT in the String, simply return the original String.   
 
```
FunStrings fun = new FunStrings();

String Example = “eat at a cool place”;  
String test = fun.removeLetter(Example, “e”);// Returns “at at a cool plac”  
String test2 = fun.removeLetter(test, “a”);//Returns “t t  cool plc”  
String test3 = fun.removeLetter(Example, “z”);//Returns “eat at a cool place”  
```
