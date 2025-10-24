# Student-Grade-Calculator
import java.util.Scanner;
public class StudentGradeCalculator {
   public static void main(String[] args) {
       int marks[] = new int[4];
       int i;
       float total = 0, avg;
       Scanner scanner = new Scanner(System.in);
       for (i = 0; i < 4; i++) {
           System.out.print("Enter Marks of Subject " + (i + 1) + ": ");
           marks[i] = scanner.nextInt();
           total += marks[i];
       }
       scanner.close();
       avg = total / 4;
       System.out.print("The student Grade is: ");
       if (avg >= 90) {
           System.out.print("A");
       } else if (avg >= 85) {
           System.out.print("B");
       } else if (avg >= 80) {
           System.out.print("C");
       } else if (avg >= 70) {
           System.out.print("D");
       } else if (avg >= 60) {
           System.out.print("E");
       } else if (avg >= 50) {
           System.out.print("Poor");
       } else {
           System.out.print("Fail");
       }
   }
}
