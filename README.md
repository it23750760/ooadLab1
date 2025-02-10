# ooadLab1

## Java Basics

### Question 1 : Running the First Java Program

Create a java program that asks the users to enter their First name and the Last Name and display Welcome to the Second Year <<FirstName>>  <<LastName>>
Compile and run the program.

- Create a class named Welcome.java
- Use the Scanner class from the java.util package.
- Promt the users to "Enter your First Name: "
- Promt the users to "Enter your Last Name: "
- The diplay a message "elcome to the Second Year <<FirstName>>  <<LastName>>"

Commit the changes and push to the repository.

### Question 2 :
There are ‘n’ number of students in a class. The students are taking 3 subjects each. Mathematics, Chemistry and Physics. You are tasked with creating a small program to let the teacher enter and view the marks of all these students. 
The program should allow the user to view the average mark a student.
The program should allow the user to view the average mark each subject.
The program should allow the user to view the Total Mark of a student for all 3 subjects.
Create a menu driven program to facilitate the above requirement. The menu should allow the below commands.
1.	Add student marks: add [studentID]- student ID will be an integer ranging from 1 to n
2.	Update student mark : update [studentID] [subjectID] - subject ID will be an integer from 1 to 3
3.	Get the average for a subject: average_s [studentID]
4.	Get the average for a student: average [studentID]
5.	Get the total mark of a student : total [studentID]

##### Steps
 - Create a public class named Marks.
 - Create the main method.
 - Create a 

## Question 3 :
Extend the program to display the grades of the student for each subject based on the below criteria.
-	If the score is 90 or above, print "Grade A"
-	If the score is between 80 and 89, print "Grade B"
-	If the score is between 70 and 79, print "Grade C"
-	If the score is between 60 and 69, print "Grade D"
-	If the score is below 60, print "Fail“
The “grades” command should display the grades of all the students in a tabular format as a summary.


##================================================================================================================
## Notes

## Arrays

An array is a collection of elements of the same type stored in contiguous memory locations. Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

### Declaring and Initializing Arrays

You can declare an array by specifying the type of its elements and the array itself. Here’s how you can do it:

```java
int[] array; // Declaration
array = new int[10]; // Initialization with size 10
```
Alternatively, you can declare and initialize an array in a single line:

```java
int[] array = new int[10]; // Declaration and initialization
```
You can also initialize an array with values at the time of declaration:
```java
int[] array = {1, 2, 3, 4, 5}; // Declaration and initialization with values
```
Accessing Array Elements
You can access the elements of an array using the index. The index starts from 0 and goes up to the array length minus one.
```java
int firstElement = array[0]; // Access the first element
array[1] = 10; // Modify the second element
```

Iterating Through an Array
You can use a loop to iterate through the elements of an array:
```java
for (int i = 0; i < array.length; i++) {
    System.out.println(array[i]);
}
```
Alternatively, you can use an enhanced for loop:
```java
for (int element : array) {
    System.out.println(element);
}
```

#### 2D Arrays
A 2D array is an array of arrays. It can be thought of as a matrix with rows and columns.

Declaring and Initializing 2D Arrays
You can declare a 2D array by specifying the type of its elements and the array itself:
```java
int[][] matrix; // Declaration
matrix = new int[3][3]; // Initialization with 3 rows and 3 columns
```

Alternatively, you can declare and initialize a 2D array in a single line:

```java
int[][] matrix = new int[3][3]; // Declaration and initialization
```
You can also initialize a 2D array with values at the time of declaration:
```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
}; // Declaration and initialization with values
```

Accessing 2D Array Elements
You can access the elements of a 2D array using row and column indices:
```java
int firstElement = matrix[0][0]; // Access the first element
matrix[1][2] = 10; // Modify the element at row 1, column 2
```

Iterating Through a 2D Array
You can use nested loops to iterate through the elements of a 2D array:
```java
for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.println(matrix[i][j]);
    }
}
```
Alternatively, you can use enhanced for loops:

```java
for (int[] row : matrix) {
    for (int element : row) {
        System.out.println(element);
    }
}
```
Example: Working with Arrays and 2D Arrays
Here’s a complete example that demonstrates how to work with arrays and 2D arrays in Java:

```java

public class ArrayExample {
    public static void main(String[] args) {
        // 1D Array
        int[] array = {1, 2, 3, 4, 5};
        System.out.println("1D Array:");
        for (int element : array) {
            System.out.println(element);
        }

        // 2D Array
        int[][] matrix = {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        };
        System.out.println("2D Array:");
        for (int[] row : matrix) {
            for (int element : row) {
                System.out.println(element);
            }
        }
    }
}
```
