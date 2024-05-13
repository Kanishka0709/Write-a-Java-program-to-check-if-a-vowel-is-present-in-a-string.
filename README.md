# Write-a-Java-program-to-check-if-a-vowel-is-present-in-a-string.
import java.util.*;
public class Main{
public static void main(String[] args) {
        String str = "KanishkaAmrutkar";

        if (hasVowel(str)) {
            System.out.println("The string does have a vowel");
        } else {
            System.out.println("The string doesn't have any vowel");
        }
}
    public static boolean hasVowel(String str) {
        str = str.toLowerCase();
        System.out.println(str);
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
                return true; 
            }
        }
        return false;
    }
}
