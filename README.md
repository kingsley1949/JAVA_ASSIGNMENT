# JAVA_ASSIGNMENT
import java.util.Scanner;

// Press Shift twice to open the Search Everywhere dialog and type `show whitespaces`,
// then press Enter. You can now see whitespace characters in your code.
public class Main {


    public static void main(String[] args) {

        // creating our input with Scanner class
        Scanner scanner = new Scanner(System.in);

        //first input
        System.out.println("what is your weight");
        int weight = scanner.nextInt();

        //second input
        System.out.println("what is your height");
        double height = scanner.nextDouble();

        //Formula => (weight /  height * height) * 10000

       double cal = ((double) weight / (height * height))*10000;

        //BMI ranges from 18.5 to 24.9 NORMAL_WEIGHT
        if (cal >= 18.5 & cal <= 24.9){
            System.out.println("YOUR WEIGHT IS " +cal+ " " + "SO YOUR WEIGHT IS" + " " + "NORMAL WEIGHT");
        }

        //BMI of more than 25.0 is OVER_WEIGHT.
        else if (cal >=25.0){
            System.out.println("YOUR WEIGHT IS " +cal+ " " +"SO YOUR WEIGHT IS" + " " + "OVER WEIGHT");

        }

        //BMI of less than 18.5 is UNDER_WEIGHT.
        else {
            System.out.println("YOUR WEIGHT IS " +cal+ " " +  "SO YOUR WEIGHT IS" + " " + "UNDER_WEIGHT");

        }


    }
}
