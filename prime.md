import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("enter a number: ");
        int n = sc.nextInt();
        boolean prime = true;
        if(n<=1){
            System.out.print("Not Prime");
        }
        for(int i=2; i<=Math.sqrt(n); i++){
            if(n%i == 0)
            prime = false;
            break;
        }
        if(prime){
            System.out.print("Prime");
        }
        else{
            System.out.print("Not Prime");
        }
    }
}
