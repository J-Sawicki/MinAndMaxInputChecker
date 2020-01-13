//# MinAndMaxInputChecker
//Simple program that checks highest and lowest user input.

import java.util.Scanner;

public class MaxAndMinChecker {

    public static void main(String[] args) {
	Scanner scanner = new Scanner(System.in);
	int min = Integer.MAX_VALUE;
	int max = Integer.MIN_VALUE;
	while (true){
        System.out.println("Enter number:");
        if (!scanner.hasNextInt()){
            break;
        }
        int number = scanner.nextInt();
        scanner.nextLine();
        if (max < number){
            max = number;
        }
        if (min > number){
            min = number;
        }
    }
        System.out.println("Max = " + max);
        System.out.println("Min = " + min);
	scanner.close();
    }
}
