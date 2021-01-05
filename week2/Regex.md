# Regular Expressions 
Regular expressions (or **Regex/Regx**p) are used in programming languages to match parts of strings. You create patterns to help you do that matching. JavaScript, regular expressions are also objects. These patterns are used with the** Exec()** and **Test()** methods of **RegEx**p, and with the **Match(**), **MatchAll()**, **Replace()**, **ReplaceAll()**, **Search()**, and **Split()** methods of **string**. 

---

---
**Some examples of common regex usage:** 

**Search() method**: The **search()** method searches a string for a specified value, and returns the position of the match.

Var str = ‘Hello World’ ;
var **regex** = **/**World**/** ;
str.serach(regex) // the result will be 6 

**Replace()** method: The **replace()** method searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced.

Var str = ‘Hello There’;
Var **regex** = **/**World**/**;
Str.replace(regex, There); // new string ‘Hello World’

---

---
#                    **Modifiers**

Modifiers/flags are used to perform case-insensitive and global searches:

/abc/g :- ‘g’ Perform a global match (find all matches rather than stopping after the first match).
/abc/i :- ‘i’ Perform case-insensitive matching.

Example for **g** flag: 
Str = “Mr Blue has a **blue** house and a **blue** car”
str.replace(/blue/**g**, "red") 
Newstr = Mr Blue has a **red** house and a **re**d car.
 
Example for **i** flag :
Str = “Mr **Blue** has a **blue** house and a **blue** car”
str.replace(/blue/**i**, "red");
Newstr = Mr **red** has a **red** house and a **red** car.

---

---
#                      **Brackets**

* [abc]	Find any character between the brackets.
* [^abc]	Find any character NOT between the brackets.
* [0-9]	Find any character between the brackets (any digit).
* [^0-9]	Find any character NOT between the brackets (any non-digit).
* (x|y)	Find any of the alternatives specifie.
---

---
#                   **Metacharacters**
* **\w**	Find a word character. => [a-zA-Z0-9]
* **\W**	Find a non-word character.
* **\d**	Find a digit. =>   [0-9]
* **\D**	Find a non-digit character.
* **\s**	Find a whitespace character.
* **\S**	Find a non-whitespace character.
* **\b**	Find a match at the beginning/end of a word, beginning like this: \bHI, end like this: HI\b.
* **\B**	Find a match, but not at the beginning/end of a word.
---

---
#                      **Quantifiers**

*  n+	Matches any string that contains at least one n. /a+/ => “aaaaabc”
* n*	Matches any string that contains zero or more occurrences of n. /a*/ => “bc” “abc” “aabc”
* n?	Matches any string that contains zero or one occurrences of n. /a?/ => “bc” “abc”
* n{X}	Matches any string that contains a sequence of X n's.  /a{3}/ => “aaa”
* n{X,Y}	Matches any string that contains a sequence of X to Y n's. /a{2,4} => “aa” “aaa” “aaaa”
* n{X,}	Matches any string that contains a sequence of at least X n's. /a{2, } => “aa” “aa..”
* n$	Matches any string with n at the end of it. /a$/ => “bdsa”
