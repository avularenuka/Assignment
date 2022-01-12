# Core Java | Assignment 1

1. Find out if the given number is an Armstrong number. Logic-if 153 is the Supplied value, then 1³+5^3+3^3=1+125+27=153.

 - This is the same as supplied value hence it is an Armstrong number.

```java
//file name - Armstrong.java

import java.util.Scanner;
import java.lang.Math;

public class Armstrong {

	public static void main(String[] args) {
	
		//declaring variables	
		int n, temp, rem, res = 0, i = 0;
		
		//user input
		System.out.println("Enter the number: ");
		Scanner scanner = new Scanner(System.in);
		n = scanner.nextInt();
		
		temp = n;
		
		//determining the power (no. of digits)
		for(; temp!= 0; temp/= 10)
		{
			i++;
		}
		temp = n;
		
		//implementing armstrong equation
		for(; temp!= 0; temp/= 10)
		{
			rem = temp % 10;
			res += Math.pow(rem, i);
		}
		
		//validating
		if(res == n)
		{
			System.out.println(n + " is an ArmStrong number.");
		}
		else
		{
			System.out.println(n + " is not an ArmStrong number.");
		}
	}
}
```

Output:

```
Enter the number: 
153
153 is an ArmStrong number.
```

2. Find out all the Armstrong numbers falling in the range of 100-999

```java
//file name - Armstrong_range.java

import java.util.Scanner;
import java.lang.Math;

public class Armstrong_range {

	public static void main(String[] args) {
		
		//condiser a loop to initiate the range of numbers
		
		for(int n = 100; n < 1000; n++)
		{
			//declaring variables
			int temp, rem, res = 0, i = 0;
			
			temp = n;
			
			//determining the power (no. of digits)
			for(; temp!= 0; temp/= 10)
			{
				i++;
			}
			temp = n;
			
			//implementing armstrong equation
			for(; temp!= 0; temp/= 10)
			{
				rem = temp % 10;
				res += Math.pow(rem, i);
			}
			
			//validating
			if(res == n)
			{
				System.out.println(n + " is an ArmStrong number.");
			}
		}
	}
}
```

Output:

```
153 is an ArmStrong number.
370 is an ArmStrong number.
371 is an ArmStrong number.
407 is an ArmStrong number.
```

3. Find out the simple as well as the compound interest of supplied

```java
//file name - SC_Intrest.java

import java.util.Scanner;
import java.lang.Math;

public class SC_Intrest {
	
	public static void main(String[] args) {
		
		//declaring variables
		double rate, amount, years, simple, compound;
		
		//declaring scanner object
		Scanner scanner = new Scanner(System.in);
		
		//user input
		System.out.println("Enter the amount : ");
		amount = scanner.nextDouble();
		System.out.println("Enter the rate : ");
		rate = scanner.nextDouble();
		System.out.println("Enter no. of years : ");
		years = scanner.nextDouble();
		
		//implementing the equations for SI and CI
		simple = (rate * years * amount)/ 100;
		compound = amount * Math.pow(1 + rate/100, years) - amount;
		
		//display
		System.out.println("Simple Interest : "+simple);
		System.out.println("compound Interest : "+compound);	
	}
}

```

Output:

```
Enter the amount : 
10000
Enter the rate : 
7
Enter no. of years : 
12
Simple Interest : 8400.0
compound Interest : 12521.915889608248
```

4. Supply marks of three subject and declare the result, result declaration is based on below conditions:

 - Condition 1: All subjects marks is greater than 60 is Passed
 - Condition 2: Any two subjects marks are greater than 60 is Promoted
 - Condition 3: Any one subject mark is greater than 60 or all subjects marks less than 60 is failed

```java
//file name - Condition_Class.java

import java.util.Scanner;

public class Condition_Class {

	public static void main(String[] args) {
		
		//declaring variables
		double sub1, sub2, sub3;
		
		//declaring scanner object
		Scanner scanner = new Scanner(System.in);
		
		//user input
		System.out.println("Enter marks in subject 1: ");
		sub1 = scanner.nextDouble();
		System.out.println("Enter marks in subject 2: ");
		sub2 = scanner.nextDouble();
		System.out.println("Enter marks in subject 3: ");
		sub3 = scanner.nextDouble();
		
		//conditions
		if(sub1 > 60 && sub2 > 60 && sub3 > 60)
		{
			System.out.println("Passed");
		}
		else if((sub1 >60 && sub2 >60) || (sub2 >60 && sub3 >60) || (sub1 >60 && sub3 >60))
		{
			System.out.println("Promoted");
		}
		else
		{
			System.out.println("Failed");
		}
	}
}
```

Output:

```
Enter marks in subject 1: 
76
Enter marks in subject 2: 
11
Enter marks in subject 3: 
13
Failed
```

5. Calculate the income tax on the basis of following table.

 - Note:-Assume slab is consider for Male, Female as well as Senior citizen
 
 | Slab | Income range | Tax Payable in percent |
 |------|--------------|------------------------|
 | Slab A | 0 - 1,80,000 | Nil |
 | Slab B | 1,80,001 - 3,00,000 | 10% |
 | Slab C | 3,00,001 - 5,00,000 | 20% |
 | Slab D | 5,00,001 - 10,00,000 | 30% |
 
 - Accept CTC from user and display tax amount
 
 ```java
 //file name - Income_Tax.java
 
import java.util.Scanner;

public class Income_Tax {

	public static void main(String[] args) {
		
		//declaring variables
		double tax =  0, CTC;
		
		//user input
		Scanner scanner = new Scanner(System.in);
		System.out.println("Enter income : ");
		CTC = scanner.nextDouble();
		
		//conditions
		if(CTC <= 180000)
		{
			tax = 0;
		}
		else if(CTC > 180000 && CTC <= 300000)
		{
			//tax calculation
			tax = (CTC/100)*10;
			System.out.println("Income tax payable is : " + tax);
		}
		else if(CTC > 300000 && CTC <= 500000)
		{
			//tax calculation
			tax = (CTC/100)*20;
			System.out.println("Income tax payable is : " + tax);
		}
		else if(CTC > 500000 && CTC <= 1000000)
		{
			//tax calculation
			tax = (CTC/100)*30;
			System.out.println("Income tax payable is : " + tax);
		}	
	}
}
 ```
 
 Output:
 
 ```
Enter income : 
400000
Income tax payable is : 80000.0
 ```

6. Consider a CUI based application, where you are asking a user to enter his Login name and password, after entering the valid user-id and password it will print the message "Welcome" along with user name. As per the validation is concerned, the program should keep a track of login attempts. After three attempts a message should be flashed saying "Contact Admin" and the program should terminate.

```java
//file name - Login_User.java

import java.util.Scanner;

public class Login_User {

	public static void main(String[] args) {
		
		//declaring variables
		String name, password;
		int count = 0, itr, track = 0;
		
		//while loop for checking and exiting after attempts are complete or logged in successfully
		while(count<3 && track == 0)
		{
			//user input
			Scanner scanner = new Scanner(System.in);
			System.out.println("Enter the login name : ");
			name = scanner.nextLine();
			System.out.println("Enter password : ");
			password = scanner.nextLine();
			
			//validation
			if(name.equals("Subham") && password.equals("satpathy"))
			{
				//login success tracker
				track = 1;
				System.out.println("Welcome " + name);
			}
			else
			{	
				//attempt count
				count++;
				itr = 3-count;
				System.out.println("Try Again. Remaining attempts " + itr);
				
				if(itr == 0)
				{
					System.out.println("Contact Admin");
				}
			}	
		}
	}
}
```

Output:

```
Enter the login name : 
Subham
Enter password : 
sa
Try Again. Remaining attempts 2
Enter the login name : 
Subham
Enter password : 
satpathy
Welcome Subham
```

7. There is an Array which is of the size 15, which may or may not be sorted. You should write a program to accept a number and search if it in contained in the array

 - Example:

| Array Elements | 5 | 12 | 14 | 6 | 78 | 19 | 1 | 23 | 26 | 35 | 37 | 7 | 52 | 86 | 47 |
|----------------|---|----|----|---|----|----|---|----|----|----|----|---|----|----|----|
| Indexes | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 |

 - Value to be search is 19

```java
//file name - Array_Search.java

import java.util.Arrays;
import java.util.Scanner;

public class Array_Search {
	
	public static void main(String[] args) {
		
		//initialize array
		int arr[] = {5,12,14,6,78,19,1,23,26,35,37,7,52,86,47};
		
		//display array and user input
		System.out.println(Arrays.toString(arr));
		Scanner scanner = new Scanner(System.in);
		System.out.println("Enter a number to search in array : ");
		int n = scanner.nextInt();
		
		//array search
		for(int i = 0; i< arr.length; i++)
		{
			if(arr[i] == n)
			{
				System.out.println(n + " is found in the array at " + i + "th index.");
			}
		}
	}
}
```

Output:

```
[5, 12, 14, 6, 78, 19, 1, 23, 26, 35, 37, 7, 52, 86, 47]
Enter a number to search in array : 
19
19 is found in the array at 5th index.
```

8. Using the above table write method apply sorting using Bubble Sort

```java
//file name - Bubble_Sort.java

import java.util.Arrays;

public class Bubble_Sort {

	public static void main(String[] args) {
		
		//initialize array
		int arr[] = {5,12,14,6,78,19,1,23,26,35,37,7,52,86,47}, temp;
		System.out.println(Arrays.toString(arr));
		
		//bubble sort algorithm
		for(int i = 0; i < arr.length-1; i++)
		{
			for(int j = 0; j < arr.length - i - 1; j++)
			{
				if(arr[j] > arr[j+1])
				{
					temp = arr[j];
					arr[j] = arr[j+1];
					arr[j+1] = temp;
				}
			}
		}
		
		//display
		System.out.println("Sorted Array :");
		System.out.println(Arrays.toString(arr));
	}
}
```

Output:

```
[5, 12, 14, 6, 78, 19, 1, 23, 26, 35, 37, 7, 52, 86, 47]
Sorted Array :
[1, 5, 6, 7, 12, 14, 19, 23, 26, 35, 37, 47, 52, 78, 86]
```

9. Accept the marks of three students for the subject say A, B, C. Find the total scored and the average in all the subjects. Also Find the Total and Average scored by students in each respective Subject.

```java
//file name - Avg_Marks.java

import java.util.Scanner;

public class Avg_Marks {

	public static void main(String[] args) {
		
		//declare and initialize variables
		Scanner scanner = new Scanner(System.in);
		double a[][] = new double[3][3];
		double total = 0; 
		
		System.out.println("Enter the marks ");
		
		//user input array
		for (int i=0;i<3;i++) 
		{
			for (int j=0;j<3;j++) 
			{
				a[i][j]=scanner.nextInt() ;
			}
		}
		
		//add all marks
		for (int i=0;i<3;i++) 
		{
			for (int j=0;j<3;j++) 
			{
					total += a[i][j];
			}
		}
		
		//average all marks
		System. out. println("Total marks in all subjects is: "+ total);
		System. out. println("Average marks in all subjects is: "+ total/9) ;
		
		total = 0;
		
		//add individual marks
		for (int i=0;i<3;i++) 
		{
			total=0;
			for (int j=0;j<3;j++) 
			{
					total += a[i][j];
			}
		
			//average individual marks
			System.out.println();
			System. out. println("Total marks for student "+ (i+1) +" of each subject is: "+ total) ;
			System. out. println("Average marks for student "+ (i+1) +" of each subject is: "+ total/3);
			System.out.println();
			
			total = 0;
		}
	}
}
```

Output:

```
Enter the marks 
89
87
67
98
71
61
56
99
78
Total marks in all subjects is: 706.0
Average marks in all subjects is: 78.44444444444444

Total marks for student 1 of each subject is: 243.0
Average marks for student 1 of each subject is: 81.0


Total marks for student 2 of each subject is: 230.0
Average marks for student 2 of each subject is: 76.66666666666667
```
