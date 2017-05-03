# Clean-Code-Book
Make Meaningful Distinctions 

Tell me the difference between

```java
public void s.play(){
}
```
vs 

```java
public void sound.play(){
}
```
Do you see what is wrong with the naming convention here. Yes? See, having the method name s.play() doesn't tell other developers what the method does. But the developer that wrote the method knows that it means. As developers this is one of the biggest mistakes we can do, give bad names to variables and methods and expect other developers to magically know what the variable does.  

```java
//Adding comments makes the code even more understandable 

//Play's the audio file
public void sound.play(){
}
```
Using pronounceable names . 

```java
public class DtaRc102{

private Data genymdhms;
private Data modymdhms;
private final String pszqint = "102;
}
```
vs 

```java
public class Customer{

private Data generationTimeStamp;
private Data modificationTimeStamp;
private final String recordID = "102;
}
```
The customer class contains words that other programmers can understand, pronounce  and use when programming. Imagine working within your development team and asking your colleague "Hey ben why is pszqint = 102" vs "Hey ben why is record = 102". 
Steve will most likely be able to answer your question quicker(perhaps without even looking at any peace of code), simply because the variable was names correctly and appropriately  . 

Using Searchable Names 

Single-letter names and numeric constants have a particular problem in that they are not easy to locate across a body of text. 

For Example the variable "e" is a rather poor choice, searching for the letter "e" might just show up in every single passage or text in ever program, this is simply because it is the most popular letter/word in the english dictionary.
The only place where "e" or any letter should be used should be within a local variable in a for loop for example or in an if statement;

```java

for(int x=0; x < 20; x++){
//do something cool
}
```


Hope this helps you.  
Sahr Thomas Acton 
(Wrote this in 48mins)
