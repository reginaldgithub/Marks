# Marks
java
/*
 * Calculate average marks of five units
 */
import java.util.Scanner;

public class main {
    public main(String[] args) {
        @SuppressWarnings("resource")
		Scanner Scanner = new Scanner(System.in);

        int totalUnits = 5;
        int[] marks = new int[totalUnits];
        int sum = 0;

        for (int i = 0; i < totalUnits; i++) {
            System.out.print("Enter the marks for Unit " + (i + 1) + ": ");
            marks[i] = Scanner.nextInt();
            sum += marks[i];
        }

        double average = (double) sum / totalUnits;

        System.out.println("The average marks is: " + average);
    }
}
