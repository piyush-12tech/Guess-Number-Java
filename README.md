import java.util.Scanner;
class GuessNumber{
public static void main(String [] args){
Scanner sc = new Scanner(System.in);
int mynumber = (int)(Math.random()*100);
int usernumber;

do {   
        System.out.print("Guess my number (1 to 100): ");  
        usernumber = sc.nextInt();  

        if(usernumber == mynumber){  
            System.out.println("Congratulations! You guessed the number.");  
            break;  
        }  
        else if(usernumber < mynumber){  
            System.out.println("Too low! Try again.");  
        }  
        else{  
            System.out.println("Too high! Try again.");  
        }  
    } while (usernumber >=0);  
    System.out.println("The number was: " + mynumber);  
}

}
