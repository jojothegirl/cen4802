/**
 * This class provides a method to calculate the nth term of the Fibonacci sequence.
 */
public class FibonacciExample {

    /**
     * Calculates the nth term of the Fibonacci sequence using recursion.
     *
     * @param n the position in the Fibonacci sequence (0-based index)
     * @return the nth term of the Fibonacci sequence
     */
    public static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        }
        return fibonacci(n - 1) + fibonacci(n - 2);
    }

    /**
     * Main method to execute the Fibonacci calculation and display the result.
     *
     * @param args command-line arguments (not used)
     */
    public static void main(String[] args) {
        int n = 10; // The position in the Fibonacci sequence
        int result = fibonacci(n);
        System.out.println("The " + n + "th term of the Fibonacci sequence is " + result + ".");
    }
}
