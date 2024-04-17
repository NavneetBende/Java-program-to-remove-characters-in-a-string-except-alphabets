Remove character in a String except alphabet
In this article we will learn how to Remove character in a String except alphabet.

Take String input from the user and store it in a variable called “s”(in this case). After that use replaceAll() method which was present in string class the work of replaceAll() method is to replace some old thing with some new thing so here we’re using a regular expression to replace character in a string with blank spaces.

Java program to remove characters in a string except alphabets
Algorithm
Take String input from user and store it in a variable called “s”.
After that use replaceAll() method.
Write regex to replace character with whitespaces like this s.replaceAll(“[^a-zA-Z]”,””);.
After that simply print the String after removing character except alphabet.
Code in Java
Output
helloworld
Method 2
Run
class Main
{
    // function to remove characters and
    // print new string
    static void removeSpecialCharacter(String s)
    {
        for (int i = 0; i < s.length(); i++)
        {
            // Finding the character whose
            // ASCII value fall under this
            // range
            if (s.charAt(i) < 'A' || s.charAt(i) > 'Z' && s.charAt(i) < 'a' || s.charAt(i) > 'z')
            {

                // erase function to erase
                // the character
                s = s.substring(0, i) + s.substring(i + 1);
                i--;
            }
        }
        System.out.print(s);
    }
    // Driver code
    public static void main(String[] args)
    {
        String s = "$P*r;e..pi, ns'ta^?";
        removeSpecialCharacter(s);
    }
}
Output
Prepinsta
Run
import java.util.Scanner;

class Main {

public static void main(String[] args) {
     String s = "hel1456lo56wor%^ld";
     s=s.replaceAll("[^a-zA-Z]","");
     System.out.println(s);
   }
}
Related Pages
Juggling algorithm for array rotation
 
Balanced Parenthesis Problem
 
Toggle each character in a string

Count the number of vowels

Length of the string without using strlen() function

Prime Course Trailer

Related Banners
Get PrepInsta Prime & get Access to all 200+ courses offered by PrepInsta in One Subscription

Get Prime
Login/Signup to comment


PRASHANTH import java.util.Scanner; public class removeCharacters {
public static void main(String[] args) {
Scanner sc = new Scanner(System.in);
String str = sc.nextLine();
for (int i = 0; i = ‘a’ && str.charAt(i) = ‘A’ && str.charAt(i) <= 'Z')
System.out.print(str.charAt(i));
}
}
}
