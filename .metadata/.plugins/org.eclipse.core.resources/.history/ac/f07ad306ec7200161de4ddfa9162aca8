/* @AUTHOR: JOHN RUSSELL
 * @CONTACT: j362r647@ku.edu
 * @DATE: 4 September 2016
 * @FILE: LetterCounter.java
 * @PURPOSE: counts the number of each letter given in a string for the purpose
 * 			 of easing frequency analysis
 */

import java.util.Scanner;
public class LetterCounter 
{

	public static void main(String[] args) 
	{
		Scanner reader = new Scanner(System.in);
		String rawInput = reader.nextLine();
		
		//regex edit removes all spaces, credit to StackOverflow user
		//nitro2k01, http://stackoverflow.com/a/5455828
		rawInput=rawInput.replaceAll("\\s","");
		System.out.println(rawInput);
		
		
		
		
		reader.close();
	}
	
	public static void printTally(int[] charCount)
	{
		//Uses unicode values to print chars, then prints equivalent
		//letters counted value in charCount
		//unicode printing numbers taken from coderanch user Monu Tripathi
		//https://coderanch.com/t/435285/java/java/printing-letters-loop
		for(int x=0; x<26; x++ )
		{
			System.out.println((char)(x+65) + "=" + charCount[x]);
		}
	}

}
