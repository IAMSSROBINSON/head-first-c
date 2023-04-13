# Sharpen your pencil

## Try to guess what each of these code fragments does

<br>

```C
int card_count = 11;
// declares and initializes a variable of int data-type to value 11

if (card_count < 10) {
  puts("The deck is hot. Increase bet.");
}
// creates an if statement with a condition 
// if the condition is true then the statements inside the block will run
// the statement inside the block prints a string of characters (a sentence of words) to the standard output stream (stdout) / command line terminal and automatically places the cursor pointer on a new line
// the statement will not print because the condition is not true. The value of card_count(11) is not less than 10

int c = 10;
while (c > 0) {
  puts("I must not write code in class");
  c = c - 1;
}
// integer variable declared and initialized to int value 10
// while loop will iterate for as long as the conditional statement is true
// the condition is true with c = 10 being greater than 0 so the block in entered
// puts will print to output the string passed in as an argument
// the value of c is reassigned to be the current value minus 1 (10 - 1 = 9)
// the loop iterates as the condition is still true
// the statement will print 10 times until the value of c == 0, at which time the statement will be false as c will not be greater than 0

/* Assume name shorter than 20 chars. */
// The above line is a way of expressing multi line comments but can also be used for single lines
char ex[20];
puts("Enter boyfriend's name: ");
scanf("%19s", ex);
printf("Dear %s. \n\n\tYou're history.\n", ex);
// variable declared of char data-type with maximum characters storage set to 20
// puts prints a string informing the user to make an action. Double quotes are used to surround a multi character string.
// scanf accepts input from the (stdin) standard input stream / keyboard and will save the user input to the variable named ex as long as it meets the conditions of the %s format specifier and is less than 20 chars. Strings are character arrays and the final character in a char array is the null character '\0' which indicates to the compiler to stop reading the content of the string. Placing the numbers 19 between the '%' and the 's' will restrict the input to 19 characters - anything extra will be ignored.
// printf will print the string provided and insert the value of the variable in place of the placeholder '%s' format specifier, the variable to replace the value with is passed as the second argument to the printf function with the string being the first - there can be multiple format specifiers acting as placeholders for their variable or value parameter counterparts.
// double quotes are used to surround a multi character string.

char suit = 'H';
switch (suit) {

  case 'C':
    puts("Clubs");
    break;
    
  case 'D':
    puts("Diamonds");
    break;

  case 'H':
    puts("Clubs");
    break;

  default:
    puts("Spades");
}
// variable with char data-type declared and initialized to value of character 'H'
// switch statement reads the value of the variable into the statement as an argument
// the cases check to see if the variable value 'H' matches that of the specified case characters
// if there is a match the puts statement will print the string value passed in and place the cursor onto a newline
// the value of the variable is 'H' thus the string "Clubs" is printed to the stdout
// the break clause take the flow of the program out of the switch statement after the puts statement completes
```