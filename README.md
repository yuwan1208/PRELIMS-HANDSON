import java.util.Collections;
import java.util.Scanner;
import java.util.ArrayList;

public class Main {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        ArrayList<String> itemProducts = new ArrayList<String>();

        while(true) {
            System.out.println("Inventory Management System");
            System.out.println("1. Add item");
            System.out.println("2. Set quantity");
            System.out.println("3. Display Inventory");
            System.out.println("4. Exit");

            System.out.println("Enter your choice: ");
            int choice = input.nextInt();


            switch(choice) {
                case 1:

                    break;
                case 2:

                    break;

                case 3:
                    System.out.println("Inventory:");
                    System.out.println("Item            Price       Quantity");
                    System.out.println("-------------------------------------");

                    itemProducts.add("Laptop");
                    itemProducts.add("Mouse");
                    itemProducts.add("Keyboard");

                    Collections.sort(itemProducts);
                    for (String i : itemProducts) {
                        System.out.println(i);
                    }
                    break;

                case 4:
                     System.out.println("Exiting...");
                     System.exit(0);
                     break;
                default:
            }
        }
    }
}
