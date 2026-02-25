import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter String: ");
        String s = sc.nextLine();
        String b = "";
        for(int i=0; i<s.length(); i++){
            b = s.charAt(i) + b;
        }
        System.out.println(b);
        if(s.equals(b)){
            System.out.print("Palindrome");
        }
        else{
            System.out.print("Not Palindrome");
        }
    }
}
