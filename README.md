# sangeetha
# first task
import java.util.Scanner;



public class Main {
    public static void main(String[] args) {


                Scanner scanner = new Scanner(System.in);

               
                System.out.print("Enter first number: ");
                int num1 = scanner.nextInt();

                System.out.print("Enter an operator (+, -, *, /): ");
                char operator = scanner.next().charAt(0);

                System.out.print("Enter second number: ");
                int num2 = scanner.nextInt();

                int result = 0;
                boolean valid = true;

                
                if (operator == '+') {
                    result = num1 + num2;
                } else if (operator == '-') {
                    result = num1 - num2;
                } else if (operator == '*') {
                    result = num1 * num2;
                } else if (operator == '/') {
                    if (num2 != 0) {
                        result = num1 / num2;   // integer division
                    } else {
                        System.out.println(" Error: Cannot divide by zero!");
                        valid = false;
                    }
                } else {
                    System.out.println(" Error: Invalid operator!");
                    valid = false;
                }

                
                if (valid) {
                    System.out.println(" Result: " + result);
                }

                scanner.close();
            }
        }

