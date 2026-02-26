import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.nextLine();
        Stack<Character> stack = new Stack<>();
        boolean isBalanced = true;
        for (char a : s.toCharArray()) {
            if (a == '{') {
                stack.push('}');
            } 
            else if (a == '(') {
                stack.push(')');
            } 
            else if (a == '[') {
                stack.push(']');
            } 
            else {
                if (stack.isEmpty() || stack.pop() != a) {
                    isBalanced = false;
                    break;
                }
            }
        }
        if (!stack.isEmpty()) {
            isBalanced = false;
        }
        System.out.println(isBalanced);
    }
}
