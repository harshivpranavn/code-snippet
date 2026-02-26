import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.nextLine();
        Set<Character> set = new HashSet<>();
        Set<Character> a = new HashSet<>();
        for(char c : s.toCharArray()){
            if(set.contains(c)){
                a.add(c);
            }
            set.add(c);
        }
        System.out.print(a);
    }
}
