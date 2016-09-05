import java.util.Scanner;

/* @AUTHOR: JOHN RUSSELL
 * @DATE: 4 SEPTEMBER 2016
 * @FILE: ShiftCipherCracker.java
 * @PURPOSE: Automatically brute force solve a shift cipher
 */

public class ShiftCipherCracker 
{
	//main launches first
	public static void main(String[] args) 
	{
		// take in char array
		Scanner reader = new Scanner(System.in);
		System.out.println("Insert ciphertext string with or without spaces, all caps pls:");
		String cipherTextInput = reader.nextLine();
		
		//regex edit removes all spaces, credit to StackOverflow user
		//nitro2k01, http://stackoverflow.com/a/5455828
		cipherTextInput=cipherTextInput.replaceAll("\\s","");
		System.out.println(cipherTextInput);
		
		//call the convert strint to int array function
		int[] rawCipherTextInts = convertStringToInts(cipherTextInput);
		//
		shiftIt(rawCipherTextInts);
		reader.close();

	}

	//modifies input int[], and passes all 25 other incremented variations to printCipherTranslation
	public static void shiftIt(int[] input)
	{
		for (int x=0; x<26; x++)
		{
			for (int y=0; y<input.length; y++)
			{
				input[y]= (input[y]+1) %26;
			}
			//method that converts int[] to char[] and prints array to console
			printCipherTranslation(input);
		}
		return;
	}
	
	//prints out a line of char value equivalents to an integer array input
	//where 0 is A and 25 is Z
	public static void printCipherTranslation(int[] input)
	{
		char[] decipheredText= new char[input.length];
		for (int x=0; x<decipheredText.length;x++)
		{
			switch (input[x]){
			case 0: decipheredText[x]= 'A';
					break;
			case 1: decipheredText[x]= 'B';
					break;
			case 2: decipheredText[x]= 'C';
					break;
			case 3: decipheredText[x]= 'D';
					break;
			case 4: decipheredText[x]= 'E';
					break;
			case 5: decipheredText[x]= 'F';
					break;
			case 6: decipheredText[x]= 'G';
					break;
			case 7: decipheredText[x]= 'H';
					break;
			case 8: decipheredText[x]= 'I';
					break;
			case 9: decipheredText[x]= 'J';
					break;
			case 10: decipheredText[x]= 'K';
					 break;
			case 11: decipheredText[x]= 'L';
					 break;
			case 12: decipheredText[x]= 'M';
					 break;
			case 13: decipheredText[x]= 'N';
					 break;
			case 14: decipheredText[x]= 'O';
					 break;
			case 15: decipheredText[x]= 'P';
					 break;
			case 16: decipheredText[x]= 'Q';
					 break;
			case 17: decipheredText[x]= 'R';
					 break;
			case 18: decipheredText[x]= 'S';
					 break;
			case 19: decipheredText[x]= 'T';
					 break;
			case 20: decipheredText[x]= 'U';
					 break;
			case 21: decipheredText[x]= 'V';
					 break;
			case 22: decipheredText[x]= 'W';
					 break;
			case 23: decipheredText[x]= 'X';
					 break;
			case 24: decipheredText[x]= 'Y';
					 break;
			case 25: decipheredText[x]= 'Z';
					 break;
			default: decipheredText[x]= ' ';
					break;
			}
		}
		
		//print out shifted message
		for(int y=0; y<decipheredText.length;y++)
		{
			System.out.print(decipheredText[y]);
		}
		System.out.print("\n");
	}
	
	//takes a string, returns a int[] of character values
	public static int[] convertStringToInts(String cipherTextInput)
	{
		char[] cipherTextArray = cipherTextInput.toCharArray();
		int[] cipherTextIntegers= new int[cipherTextInput.length()];
		for (int x=0; x<cipherTextArray.length; x++)
		{
			//Assigns numerical value to cipherTextIntegers for
			//corresponding cipherTextArray characters
			switch (cipherTextArray[x]) {
				case 'A': cipherTextIntegers[x]=0;
						  break;
				case 'B': cipherTextIntegers[x]=1;
						  break;
				case 'C': cipherTextIntegers[x]=2;
						  break;
				case 'D': cipherTextIntegers[x]=3;
						  break;
				case 'E': cipherTextIntegers[x]=4;
						  break;
				case 'F': cipherTextIntegers[x]=5;
						  break;
				case 'G': cipherTextIntegers[x]=6;
						  break;
				case 'H': cipherTextIntegers[x]=7;
						  break;
				case 'I': cipherTextIntegers[x]=8;
						  break;
				case 'J': cipherTextIntegers[x]=9;
						  break;
				case 'K': cipherTextIntegers[x]=10;
						  break;
				case 'L': cipherTextIntegers[x]=11;
						  break;
				case 'M': cipherTextIntegers[x]=12;
						  break;
				case 'N': cipherTextIntegers[x]=13;
						  break;
				case 'O': cipherTextIntegers[x]=14;
						  break;
				case 'P': cipherTextIntegers[x]=15;
						  break;
				case 'Q': cipherTextIntegers[x]=16;
						  break;
				case 'R': cipherTextIntegers[x]=17;
						  break;
				case 'S': cipherTextIntegers[x]=18;
						  break;
				case 'T': cipherTextIntegers[x]=19;
						  break;
				case 'U': cipherTextIntegers[x]=20;
						  break;
				case 'V': cipherTextIntegers[x]=21;
						  break;
				case 'W': cipherTextIntegers[x]=22;
						  break;
				case 'X': cipherTextIntegers[x]=23;
						  break;
				case 'Y': cipherTextIntegers[x]=24;
						  break;
				case 'Z': cipherTextIntegers[x]=25;
						  break;
				default: cipherTextIntegers[x]=0;
						 break;
			}
		}
		
		return(cipherTextIntegers);
	}
}
