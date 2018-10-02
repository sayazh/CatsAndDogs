# CatsAndDogs
Counter of appearing Strings "Cat &amp;&amp; Dog"
package Assignments2;

import java.util.Scanner;

public class CatsAndDogs {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
        System.out.println("Enter the word");
		String word = sc.next();
		int catCounter = 0;
		int dogCounter = 0;
		
		for (int letter = 0; letter<word.length(); letter++) {
			if (word.charAt(letter)=='c' && word.charAt(letter+1)=='a' && word.charAt(letter+2)=='t') {
				catCounter++;}
			}
			for (int letter = 0; letter< word.length(); letter++) {
		if (word.charAt(letter)=='d' && word.charAt(letter+1)=='o' && word.charAt(letter+2)=='g') {
			dogCounter++;
		}
					} 
			if (catCounter==dogCounter) {
				System.out.println("true");
			} else {
				System.out.println("false");
			}
			sc.close();
	}

}
