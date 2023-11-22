import java.util.Random;
import java.util.Scanner;

public class NumberGuessingGame {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Random random = new Random();
        
        int lowerBound = 1;
        int upperBound = 100;
        int numberToGuess = random.nextInt(upperBound - lowerBound + 1) + lowerBound;
        int attempts = 0;
        int userGuess = 0;
        
        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I have selected a random number between " + lowerBound + " and " + upperBound + ". Can you guess it?");
        
        while (userGuess != numberToGuess) {
            System.out.print("Enter your guess: ");
            userGuess = scanner.nextInt();
            attempts++;
            
            if (userGuess < lowerBound || userGuess > upperBound) {
                System.out.println("Please enter a number between " + lowerBound + " and " + upperBound + ".");
            } else if (userGuess < numberToGuess) {
                System.out.println("Too low! Try again.");
            } else if (userGuess > numberToGuess) {
                System.out.println("Too high! Try again.");
            }
        }
        
        System.out.println("Congratulations! You guessed the number in " + attempts + " attempts.");
        scanner.close();
    }
}
