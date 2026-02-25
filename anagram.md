import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        String b = sc.nextLine();
        char[] x = a.toCharArray();
        char[] y = b.toCharArray();
        Arrays.sort(x);
        Arrays.sort(y);
        String s1 = new String(x);
        String s2 = new String(y);
        if(s1.equals(s2)){
            System.out.print("Anagram");
        }
        else{
            System.out.print("Not Anagram");
        }
    }
}
