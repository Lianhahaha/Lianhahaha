import java.util.Scanner;

public class Store {

    
    public static void main(String[] args) {
       
        System.out.println("Welcome To Jurassic Park");

       
        order();
    }

    
    public static void order() {
        
        Scanner input = new Scanner(System.in);

        
        int choice;
        int quantity;
        double total = 0;
        double pay;
        String again;
        
        
        

        double[] prices = {15.00
                          , 35.00
                          , 25.00              
                          ,500.00
                          ,99.00}; 
              
                         
      

        
        String[] items = {"Iphone 20 Bedrock", "Samsung", "Viva y16 Pro", "Nokia", "Red Magic"};

        do {
            
            System.out.println("What's in the menu?");
            System.out.println("""
                               1. Iphone 20 bedrock - 15.00
                               2. Samsung - 35.00
                               3. Viva y16 Pro - 25.00
                               4. Nokia - 500.00
                               5. Red Magic - 99.00
                               6. Press here if you want to leave the park""");
          
           
                
            
            
         
         
            System.out.println("Choose between 1/2/3/4/5 or press 6 to LEAVE:");
            choice = input.nextInt();

           
            if (choice >= 1 && choice <= 5) {
                System.out.println("You chose " + items[choice - 1]);
                System.out.print("How many can i get for ya? ");
                quantity = input.nextInt();

               
                total += quantity * prices[choice - 1];
                System.out.println("Current total: " + total);

            } else if (choice == 6) {
              
                System.out.println("Exiting the park.");
                break; 
            } else {
             
                System.out.println("Invalid choice. Please choose between 1/2/3/4/5/6.");
            }

          
            System.out.print("Would ya like to buy more? (Yep/No): ");
            again = input.next();

        } while (again.equalsIgnoreCase("Yep")); 
          
        double discount = 0;
        if (total >= 700) {
            discount = total * 0.05;
            total -= discount;
            System.out.println("Discount applied: " + discount);
        }

        
        if (total > 0) {
            System.out.println("Total amount to pay: " + total);
            System.out.print("Enter payment amount: ");
            pay = input.nextDouble(); 

            
            if (pay < total) {
                System.out.println("Sorry, you don't have enough balance.");
            } else {
               
                double change = pay - total;
                System.out.println("Payment successful! Your change: " + change);
            }
        } else {
           
            System.out.println("No items bought.");
        }
    }
}
