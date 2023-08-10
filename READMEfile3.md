
## Things I want to know more about
# class3

Q1. Explain the difference between an “int” and an “Integer” in Java.

<pre>
int :primitive data type in Java. It represents a 32-bit signed integer value
integer:a class in the Java that serves as a wrapper for the primitive int
 </pre>

 ---------------------------------------------------------------------------------------------
 Q2.What is the default value for ints? Integers?
 <pre>
 for int :THE default value is 0 an actual numeric value
for integer:The default value is null 
 </pre>

 ---------------------------------------------------------------------------------------------
 Q3. What is autoboxing? Unboxing?
<pre>
The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

autoboxing :process of converting a primitive data type into its corresponding wrapper class object.
Unboxing: process of extracting the primitive value from a wrapper class object.
 </pre>

 ---------------------------------------------------------------------------------------------

 Q4.List the three basic categories of exceptions.
 <pre>
The first thing we use exceptions to handle errors and other exceptional events.
and the three Kinds of Exceptions :
1. checked exception :xceptional conditions that a well-written application should anticipate and recover from.and handle (using try-catch blocks) or declare that your method may throw using the throws .
2.errors:  exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.
3.runtime exception :internal to the application, and that the application usually cannot anticipate or recover from.usually indicate programming bugs, such as logic errors

 </pre>

 ---------------------------------------------------------------------------------------------
Q5. What type of statement can you use to handle an exception?
<pre>
To handle an exception,  the try, catch, and finally blocks .the try block to enclose the code that might throw an exception 
catch  provides code to be executed when that type of exception occurs.
finally :always executes when the try block exits , executed even if an unexpected exception occurs, or  when no exceptions are anticipated.

public void writeList() {
    PrintWriter out = null;
    try {
        System.out.println("Entered try statement");
        FileWriter f = new FileWriter("OutFile.txt");
        out = new PrintWriter(f);
        for (int i = 0; i < SIZE; i++) {
            out.println("Value at: " + i + " = " + list.get(i));
        }
    }}

    catch (IndexOutOfBoundsException e) {
    System.err.println("IndexOutOfBoundsException: " + e.getMessage());
} catch (IOException e) {
    System.err.println("Caught IOException: " + e.getMessage());
}
 </pre>

 ---------------------------------------------------------------------------------------------
Q6. Describe a situation where you think it would be useful to have a program that scans text.
<pre>

Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.
 ScanXan, a program that reads the individual words in xanadu.txt and prints them out, one per line.
 </pre>

 ---------------------------------------------------------------------------------------------
Q7.What is input from a Scanner broken down into?
<pre>
 ScanXan, a program that reads the individual words in xanadu.txt and prints them out, one per line.and ScanXan invokes Scanner's close method when it is done with the scanner object. Even though a scanner is not a stream, you need to close it to indicate that you're done with its underlying stream. use a different token separator, invoke useDelimiter(), specifying a regular expression. For example, suppose you wanted the token separator to be a comma, optionally followed by white space. You would invoke.
 </pre>

 ---------------------------------------------------------------------------------------------