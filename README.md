// This is a simple Java program demonstrating text output and string manipulation.

/**
 * The Main class contains examples of how to work with text (Strings) in Java.
 */
public class Main {

    /**
     * The main method is the entry point of the Java application.
     * It demonstrates basic text printing and string reversal.
     *
     * @param args Command line arguments (not used in this example).
     */
    public static void main(String[] args) {

        // --- Example 1: Basic Text Output (Hello World) ---
        // This is the simplest way to display text in Java.
        // System.out.println() prints the text and then moves to a new line.
        System.out.println("--- Example 1: Basic Text Output ---");
        System.out.println("Hello, Java World!"); // Prints a classic greeting
        System.out.println("This is a simple text example.");
        System.out.println(); // Prints an empty line for better readability

        // --- Example 2: String Variables and Concatenation ---
        // Strings are sequences of characters. They are objects in Java.
        System.out.println("--- Example 2: String Variables and Concatenation ---");
        String greeting = "Welcome";
        String name = "to Java Programming";
        String fullMessage = greeting + " " + name + "!"; // Concatenating strings using the '+' operator

        System.out.println(fullMessage); // Prints: Welcome to Java Programming!
        System.out.println("The length of the message is: " + fullMessage.length()); // Shows string length
        System.out.println();

        // --- Example 3: String Manipulation - Reversing a String ---
        // This example shows how to reverse a string using a loop.
        System.out.println("--- Example 3: String Manipulation - Reversing a String ---");
        String originalString = "Java is fun!";
        String reversedString = ""; // Initialize an empty string to store the reversed text

        // Loop through the original string from the last character to the first.
        for (int i = originalString.length() - 1; i >= 0; i--) {
            // Get each character and append it to the reversedString.
            reversedString = reversedString + originalString.charAt(i);
        }

        System.out.println("Original String: " + originalString);
        System.out.println("Reversed String: " + reversedString);
        System.out.println();

        // --- Example 4: Using StringBuilder for efficient string manipulation ---
        // For more complex or frequent string modifications, StringBuilder is more efficient
        // than concatenating strings with '+', as it avoids creating many intermediate String objects.
        System.out.println("--- Example 4: Using StringBuilder ---");
        String anotherString = "Efficient Reversal";
        StringBuilder sb = new StringBuilder(anotherString);
        sb.reverse(); // StringBuilder has a built-in reverse method
        String reversedEfficiently = sb.toString(); // Convert StringBuilder back to String

        System.out.println("Original String (efficient): " + anotherString);
        System.out.println("Reversed String (efficient): " + reversedEfficiently);
    }
}



