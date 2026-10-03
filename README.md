# Hackathon1_2620030091
1a)Data Types:


import java.util.Scanner;


public class HouseholdDetails {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter number of family members: ");
        int familyMembers = scanner.nextInt();

        System.out.print("Enter water consumed (in litres): ");
        double waterConsumed = scanner.nextDouble();

        System.out.print("Enter house number: ");
        int houseNumber = scanner.nextInt();

        System.out.print("Enter water usage status: ");
        char usageStatus = scanner.next().charAt(0);

        System.out.println("\nHousehold Details");
        System.out.println("Family Members: " + familyMembers);
        System.out.println("Water Consumed: " + waterConsumed + " litres");
        System.out.println("House Number: " + houseNumber);
        System.out.println("Usage Status: " + usageStatus);

        scanner.close();
    }
}



1b) If-Else Condition:



import java.util.Scanner;

public class WaterBillCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter water consumption in litres: ");
        double consumption = scanner.nextDouble();

        int bill;
        if (consumption <= 500) {
            bill = 100;
        } else {
            bill = 200;
        }

        System.out.println("Water Bill: Rs." + bill);

        scanner.close();
    }
}
