Pyramid number pattern
In this section, we learn how to print pyramid number pattern in the java. 

here  we create half pyramid, inverted half pyramid and the triangle pyramid using a number in java.

this pattern example are useful also in interview question in java, so see every step carefully of each pattern.

To create a simple number pattern using , you have to use two loop. Due to this, nested for loop define rows to create with the columns of the number.

The first for loop define the number of rows for the pattern. The second Loop prints each row with the number.

number pattern
1. Write the Program to print the following pattern
Enter the row 5

1
1 2
1 2 3 
1 2 3 4
1 2 3 4 5
Working
Step 1-  first we need to initialize two variable for loop.

Step 2- The first loop work for the row. so loop work from 1 to row;

Step 3- The second loop work for the number in a row. so this loop work from 1 to i.

Step 4. Inside the second loop, print the j.

Step 5- Outside the second loop and inside the first loop, give new line.

 Step 6- Stop.

C	JAVA	Python	C++
n=5
for i in range(n):
    for j in range(i+1):
        print(j+1,end=” “)
    print()
2. Write a program to print the following pattern
Enter number  5

1 2 3 4 5
1 2 3 4
1 2 3
1 2 
1
C	JAVA	Python	C++
n=5
for i in range(n):
    for j in range(n-i):        
        print(j+1,end=” “)
    print()
3. Write a program to print the following pattern
Enter the row 5

             1
           2 3 2
         3 4 5 4 3
       4 5 6 7 6 5 4
     5 6 7 8 9 8 7 6 5
C	JAVA	Python	C++
n=5
for i in range(n):
    x=i+1
    for j in range(2*n-1):
        if(i+j<n-1 or i+j>=n+2*i):   
            print(” “,end=“”)
        else:
            print(x,end=“”) 
            if(j<n-1):
                x+=1
            else:
                x-=1
    print()
