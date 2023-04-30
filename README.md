Download Link: https://assignmentchef.com/product/solved-cs271-assignment-4
<br>
Write a program to calculate composite numbers.  First, the user is instructed to enter the number of composites to be displayed, and is prompted to enter an integer in the range [1 .. 400].  The user enters a number, <em>n</em>, and the program verifies that 1 ≤ <em>n</em> ≤ 400.  If <em>n</em> is out of range, the user is reprompted until s/he enters a value in the specified range.  The program then calculates and displays all of the composite numbers up to and including the <em>n</em><u><sup>th</sup></u> composite.  The results should be displayed 10 composites per line with at least 3 spaces between the numbers.

<strong> </strong>

<strong>Requirements: </strong>

<ul>

 <li>The programmer’s name must appear in the output.</li>

 <li>The counting loop (1 to <em>n</em>) must be implemented using the MASM <em>loop</em></li>

 <li>The <em>main</em> procedure must consist (mostly) of procedure calls. It should be a readable “list” of <u>what</u> the program will do.</li>

 <li>Each procedure will implement a section of the program logic, i.e., each procedure will specify <u>how</u> the logic of its section is implemented. The program must be modularized into at least the following procedures and sub-procedures :

  <ul>

   <li><em>introduction </em></li>

   <li><em>getUserData </em></li>

   <li><em>validate </em></li>

   <li><em>showComposites </em></li>

   <li><em>isComposite </em></li>

   <li><em>farewell </em></li>

  </ul></li>

 <li>The upper limit should be defined and used as a <u>constant</u>.</li>

 <li>Data validation is required. If the user enters a number outside the range [1 .. 400] an error message should be displayed and the user should be prompted to re-enter the number of composites.</li>

 <li>The usual requirements regarding documentation, readability, user-friendliness, etc., apply. 8) Submit your text code file (.<em>asm</em>) to Canvas by the due date.</li>

</ul>

<strong> </strong>

<strong>Notes: </strong>

<ul>

 <li>For this program, you may use global variables instead of passing parameters. This is a onetime relaxation of the standards so that you can get accustomed to using procedures.</li>

 <li>A number <em>k</em> is composite if it can be factored into a product of smaller integers. Every integer greater than one is either prime or composite. Note that this implies that

  <ol>

   <li>1 is not composite.</li>

   <li>The number must be positive.</li>

  </ol></li>

 <li>There are several ways to make your <em>isComposite</em> procedure efficient. (I recommend discussing this in your groups!)</li>

 <li>See next page for an example execution</li>

</ul>

page 1 of 2

<strong>Example</strong> (user input in <strong><em>italics</em></strong>):

Composite Numbers     Programmed by Euclid




Enter the number of composite numbers you would like to see. I’ll accept orders for up to 400 composites.




Enter the number of composites to display [1 .. 400]: <strong><em>501</em></strong> Out of range.  Try again.

Enter the number of composites to display [1 .. 400]: <strong><em>0</em></strong> Out of range.  Try again.

Enter the number of composites to display [1 .. 400]: <strong><em>31</em></strong>




4   6   8   9   10   12   14   15   16   18

20   21   22   24   25   26   27   28   30   32

33   34   35   36   38   39   40   42   44   45 46




Results certified by Euclid.  Goodbye.

<strong> </strong>

<strong>Extra Credit: </strong>

<ul>

 <li>Align the output columns.</li>

 <li>Display more composites, but show them one page at a time. The user can “Press any key to continue …” to view the next page.  Since length of the numbers will increase, it’s OK to display fewer numbers per line.</li>

 <li>One way to make the program more efficient is to check against only prime divisors, which requires saving all of the primes found so far (numbers that fail the composite test). It’s easy in a high-level language, but you will have to look ahead in the textbook to figure out how to do it in assembly language.</li>

</ul>


