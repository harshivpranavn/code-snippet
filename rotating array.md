import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter n: ");
        int n = sc.nextInt();
        System.out.print("Enter k: ");
        int k = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0;i<n;i++){
            System.out.print("Enter val: ");
            arr[i] = sc.nextInt();
        }
        k = k % n;
        int[] res = new int[n];
        for(int i=0; i<n; i++){
            res[(i+k)%n] = arr[i];
        }
        System.out.println(Arrays.toString(res));
    }
}
