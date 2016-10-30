		import java.util.Scanner;
public class chap7ex720 {

	public static void main(String[] args) {
		// *7.20 (Revise selection sort) In Section 7.11, you 
		//used selection sort to sort an array. The selection-sort method
		//repeatedly finds the smallest number in the current array and 
		//swaps it with the first. Rewrite this program by finding the
		//largest number and swapping it with the last. Write a test 
		//program that reads in ten double numbers, invokes the method, and
		//displays the sorted numbers. 
	
		 
		 
	//start a scanner
		  Scanner input = new Scanner(System.in);
		  int[] numbers = new int[10];
		 
	//ask for input
		 
		  System.out.print("Enter ten numbers:");
		
		  //loop
		  for (int i = 0; i < numbers.length; i++) {
		   numbers[i] = input.nextInt();
		  }
		 
		  System.out.print("The sorted numbers are:");
		 
		  //call method
		  selectionSort(numbers);
		  for (int i = 0; i < numbers.length; i++) {
		   System.out.print(numbers[i] + " ");
		  }
		 }
		 
		  //the method
		 public static void selectionSort(int[] list) {
		  for (int i = list.length-1; i > 0; i--) {
		   // Find the max in the list[list.length...1]
		   int currentMax = list[i];
		   int currentMaxIndex = i;
		 
		   for (int j = 0; j < i; j++) {
		    if (currentMax < list[j]) {
		     currentMax = list[j];
		     currentMaxIndex = j;
		    }
		   }
		 
		   
		   //array
		   // Swap list[i] with list[currentMaxIndex] if necessary
	
		  
		 }}}
