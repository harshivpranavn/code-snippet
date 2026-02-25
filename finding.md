import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter n: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0;i<n;i++){
            System.out.print("Enter val: ");
            arr[i] = sc.nextInt();
        }
        System.out.print("Enter target: ");
        int target = sc.nextInt();
        for(int i=0; i<n; i++){
            if(arr[i] == target){
                System.out.print(i);
            }
            else{
                System.out.print("not found");
            }
        }
    }
}
