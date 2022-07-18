import java.util.Scanner;
 
public class PermutationCombinationMain
{
    public static int fact(int num){
        int fact=1, i;
        for(i=1; i<=num; i++){
            fact = fact*i;
        }
        return fact;
    }
    public static void main(String args[]){
        int n, r;
        Scanner scanner = new Scanner(System.in);
 
        System.out.print("Enter Value of n : ");
        n = scanner.nextInt();
        System.out.print("Enter Value of r : ");
        r = scanner.nextInt();
 
        System.out.print("NCR is " +(fact(n)/(fact(n-r)*fact(r))));
        System.out.print("\nNPR is " +(fact(n)/(fact(n-r))));
    }
}