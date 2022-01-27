# ArithmeticCalculator
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    char operator;
    Double n1, n2, output;
    Scanner scn = new Scanner(System.in);
    System.out.println("Choose an operator: +, -, *, or /");
    operator = scn.next().charAt(0);
    System.out.println("Enter first number");
    n1 = scn.nextDouble();
    System.out.println("Enter second number");
    n2 = scn.nextDouble();

    switch (operator) {
      case '+':
        output = n1 + n2;
        System.out.println(n1 + " + " + n2 + " = " + output);
        break;
      case '-':
        output = n1 - n2;
        System.out.println(n1 + " - " + n2 + " = " + output);
        break;
      case '*':
        output = n1 * n2;
        System.out.println(n1 + " * " + n2 + " = " + output);
        break;
      case '/':
        output = n1 / n2;
        System.out.println(n1 + " / " + n2 + " = " + output);
        break;
     default:
        System.out.println("Invalid operator!");
        break;
    }
}
}
