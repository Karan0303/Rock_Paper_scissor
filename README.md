# Rock_Paper_Scissor
import java.util.Random;
import java.util.Scanner;

import javax.swing.BoundedRangeModel;



public class Rock_Paper_Scissor {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter 0 for Rock ," + " Enter 1 for Paper , "+"Enter 2 for Scissor");
        System.out.print("Your choise = ");
        int user = sc.nextInt();
        
        Random computer=new Random();
        int computerint =computer.nextInt(3);
        System.out.println("computer choise = " + computerint);
        
        if(user==computerint){
            System.out.println("Draw");
        }

        else if(user==0 && computerint==2 || user==1 && computerint==0 || user==2 && computerint== 1){
            System.out.println("You win !");
            
    }
    else{
        System.out.println("computer wins !");
    }
}
}

