## Problem:
Write a program in a Scala or JavaScript that takes two strings (S and F) as input. S can be any string, and F should be interpreted as the name of a text file. Your program will determine the percent of words contained in the file represented by F that can be formed using the letters in S. For example, if S was "abcdefghijklmnopqrstuvwxyz" all strictly lowercase basic latin words without repeated letters would be formable. So if F contained the following words:

aardvark - Not formable
uncopyrightable - Formable
United - Not formable

Then the output would be 1/3 or 33.3333. Use your best judgement on how to handle non-alphanumeric characters when tokenizing the input (hyphens and apostrophes should probably be considered part of the token, commas and exclamation marks should probably be considered tokenizers). When in doubt clearly state your assumptions.

Running the program:
terminal>sbt
>console
scala> import com.placeholder.takehome.Probability
import com.placeholder.takehome.Probability
scala> Probability.getProbability("qwertyuioplkjhgfdsazxcvbnm","src/main/resources/data1.txt")
res0: Float = 0.16666667
scala> Probability.getProbability("sf","src/main/resources/data.txt")
res1: Float = 0.16666667
scala> Probability.getProbability("sdf","src/main/resources/data.txt")
res2: Float = 0.5
scala> Probability.getProbability("sd","src/main/resources/data.txt")
res3: Float = 0.0
