Download Link: https://assignmentchef.com/product/solved-lab-09-variables-and-objects-cse-021
<br>
<h1>Overview</h1>

This week’s assignment will be a review exercise to get you comfortable with OOP and variables. In the first exercise, you will fix some common mistakes people tend to make. The second part gets you comfortable with declaring objects, working with object arrays, using constructors, and calling (overloaded) member methods.




<strong>A</strong>nswer the assessment questions as you encounter them in the next section. This is especially true for this assignment, as each question will to help you finish and understand the point of that particular exercise. The prompts for answering assessment questions are placed immediately following the material to which the listed questions relate.

<h1>Getting Started</h1>

After following the import instructions in the assignment page, you should have a Java project in Eclipse titled Lab 21_9. This PDF document is included in the project in the <strong>doc</strong> directory. The Java files you will use in this lab are in the <strong>src</strong> directory, as usual.

<h2>Part 1: Fix Lab21_Vars.java</h2>

You will implement 7 fixes that are indicated in the code. The following 7 issues (and 10 assessment questions) correspond to the 7 fixes you need to implement.




<strong>Issue 1:</strong> 5.0 is a double but we want to assign it to an integer variable instead. We could of course change it to 5 but what if we couldn’t? Remember, we can always type cast any type to any other type.




[Answer assessment question 1]




<strong>Issue 2:</strong> We want to declare an array of integers, but instead have the following code:




int arri0 = {10, 9, 8, 7, 6, 5, 4, 3, 2, 1};




[Answer assessment question 2]




<strong>Issue 3:</strong> We want to share a variable in the if-clause and else-clause as attempted by the following code:




if (i &lt; j) {  int temp = 0;

System.out.println(“Temp is ” + temp);

} else {  temp = 1;

System.out.println(“Temp is ” + temp); }




[Answer assessment question 3]




<strong>Issue 4:</strong> Another common construct we use is a variable to store the total of some calculation. Suppose we want to do square of sums and want it in total which we later print, as attempted by the following code:




for (int i = 0; i &lt; 10; i++) {

int total = 0;  total += i*i;

}

System.out.println(“i value is ” + i);

System.out.println(“Total is ” + total);




[Answer assessment questions 4 and 5]




<strong>Issue 5:</strong> We can create objects using new, and create pointers that references these objects. Multiple pointers can point to the same object or different objects. Analyze the following code to figure out the logical error.




Cheese jack;

Cheese monterey = new Cheese(“Monterey”);

jack = monterey;

System.out.println(“Monterey name is ” + monterey.getName()); jack.setName(“Jack”);

System.out.println(“Jack name is ” + jack.getName()); System.out.println(“Monterey name is still ” + monterey.getName());




[Answer assessment questions 6 and 7]




<strong>Issue 6:</strong> Sometimes we write code that duplicates or is redundant in different parts of our conditional statements. The following code illustrates this:




Scanner input = new Scanner(System.in);

System.out.print(“Enter first number: “);




if (input.nextInt() &gt; var3) {

System.out.print(“Enter second number: “);  int num2 = input.nextInt();

System.out.println(“First is greater”);  if (num2 &lt; var3)

System.out.println(“Second is Less than”);  else

System.out.println(“Second is Greater or equal”);

} else {

System.out.print(“Enter second number: “);   int num2 = input.nextInt();

System.out.println(“First is Less than or equal”);   if (num2 &lt; var3)

System.out.println(“Second is Less than”);

else

System.out.println(“Second is Greater or equal”); }




[Answer assessment questions 8 and 9]




<strong>Issue 7:</strong> Suppose we want to print out the first number the user entered after all the lines given above.




[Answer assessment question 10]

<h2>Part 2: Fill-in Lab21_Objects.java</h2>

Have a look at Dummy.java. It has 11 constructors and 11 overloaded display() method. Your job is to call every one of them from the main method of Lab21_Objects, and fill in each of the dlist (Dummy list) entries with the appropriate objects. We have included the first two constructor calls and first two display() calls in the file. Fill in 9 more constructor calls and 9 more display() calls.




DO NOT DECLARE NEW VARIABLES. YOU MUST USE ONLY THE GIVEN VARIABLES AS

ARGUMENTS TO THE METHOD CALLS. DO NOT USE ANY CONSTANTS OR NUMBERS AS

ARGUMENTS (e.g., 5, 5.0, etc.)




You can use individual indices of the arrays for the arguments. For example, using dlist[1].display(iarr[0]); is okay, but dlist[1].display(0); is not (as that is using the number 0 directly as an argument).




[Answer assessment questions 11, 12 and 13]

<strong> </strong>

<h1>Part 3: (Assessment) Logic Check and Level of Understanding</h1>

Create a Word document or text file named Part3 that contains answers to the following:

<ul>

 <li>How do you type cast a double into an int?</li>

 <li>How do you declare an array of int that goes from 10 to 1?</li>

 <li>What is the scope of the variable temp declared at line 20 of java? Where does it need to be declared if it is to be used for the if-clause and else-clause?</li>

 <li>What is the scope of the variable total declared in line 29 of java?</li>

 <li>What is X in the print out “i value is X” at line 32 of java? And why is it that value?</li>

 <li>What is the logical error in the code at lines 36-42 of java? (How do you fix it?)</li>

 <li>How many pointers and objects are created in your fixed version of code at lines 36-42 of java?</li>

 <li>What parts are redundant in the code at lines 46-66 of java?</li>

 <li>How do reduce or combine the redundant code at lines 46-66 of java so we have no redundancy?</li>

 <li>How can we figure out what was the first number for code at lines 46-66 of java? What is the println statement to print the first number?</li>

 <li>Give two distinct characteristics of a constructor.</li>

 <li>What is the purpose of ‘.’ in out.println(); or dlist[1].display();?</li>

 <li>What happens if you swap the order of the two lines in java? (and why?) dlist[0].display(); // Goes first dlist[0] = new Dummy(); // Goes after</li>

</ul>


