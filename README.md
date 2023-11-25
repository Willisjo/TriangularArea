# TriangularArea

import java.util.Scanner;

public class TriangleAreaCalculator {

    public static void main(String[] args) {
        TriangleAreaCalculator calculator = new TriangleAreaCalculator();
        calculator.calculateAndDisplayArea();
    }

    public void calculateAndDisplayArea() {
        double base = getUserInput("Enter the base of the triangle: ");
        double height = getUserInput("Enter the height of the triangle: ");

        double area = calculateArea(base, height);

        displayResult(area);
    }

    private double getUserInput(String message) {
        Scanner scanner = new Scanner(System.in);
        System.out.print(message);
        return scanner.nextDouble();
    }

    private double calculateArea(double base, double height) {
        return 0.5 * base * height;
    }

    private void displayResult(double area) {
        System.out.println("The area of the triangle is: " + area);
    }
}
