#JAVA PROGRAM TO ADD AN ARRAY ELEMENTS.
STEP1: First create a class 
STEP2: Now create a method 
STEP3: Create two array with its size,as stored in a variable.
STEP4: Apply for loop to the variable value and stores in array.
STEP5: Then apply for loop again in array,and add the elements as follows:
  arr[0]=arr[0]+arr[i] ,where i is the value of for loop using for arrray.
  
now in main method create an object of method and Scanner class (used to input values from user).

#THE PROGRAM IS GIVE HERE
import java.util.Scanner;

public class CalculatorS {

    public void addition() {
        try (Scanner sc = new Scanner(System.in)) {
            System.out.print("Enter Number Of Elements You Want To Add :");
            int numelements = sc.nextInt();
            int adda[] = new int[numelements];
            int added[] = new int[numelements];
            for (int i = 0; i < numelements; i++) {
                System.out.print("Value"+" "+(i+1)+" : ");
                adda[i] = sc.nextInt();
            }
            System.out.println("You Entered the Following Values:");
            for (int i = 0; i < numelements; i++) {
                System.out.print(" " + adda[i] + " ");
            }

            System.out.println(" ");
            System.out.println("Calculating Your Expression ... .");
            for (int i = 0; i < adda.length; i++) {
                added[0] = added[0] + adda[i];
            }
            System.out.println("Your Expression is Calculated.");
            for (int i = 0; i < 1; i++) {
                System.out.println(" " + added[i] + " ");
            }
        }
        catch(Exception e){
            System.out.println(e);
        }
    }

    public static void main(String[] args) {
        CalculatorS optionobj = new CalculatorS();
        optionobj.addition();
    }
}

# Do like my Youtube chenel and also visit my profile on my instagram account.
