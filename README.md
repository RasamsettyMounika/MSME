# MSME
MSME project 
// Java implementation to print the pattern 
import java.io.*; 

class GFG 
{ 
	// Function to print required 
	// number of stars 
	static void print1(int i) 
	{ 
		for (int j = 1; j <= i; j++) 
			System.out.print("*"); 
	} 
	static void print(int n) 
	{ 
		for (int i = 1; i <= n; i++) { 
	
			// function calling to print 
			// the initial stars in each line 
			print1(i); 
	
			// printing underscore 
			System.out.print("_"); 
	
			// function calling to print 
			// stars on right side of first half 
			print1(n - i + 1); 
	
			// printing underscore 
			System.out.print("_"); 
	
			// function calling to print 
			// stars on left side of second half 
			print1(n - i + 1); 
	
			// printing underscore 
			System.out.print("_"); 
	
			// function calling to print 
			// the ending stars 
			print1(i); 
			System.out.println(); 
		} 
	} 
	
	// Driver code 
	public static void main (String[] args) 
	{ 
		// number of lines 
		int n = 5; 
	
		// function calling 
		print(n); 

	} 
} 

// This code is contributed by vt_m. 
