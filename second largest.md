import java.util.*;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("enter size: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            System.out.print("enter: ");
            arr[i] = sc.nextInt();
        }
        for(int i=0; i<n; i++){
            for(int j=i+1; j<n; j++){
                int temp = 0;
                if(arr[i] > arr[j]){
                    temp = arr[i];
                    arr[i] = arr[j];
                    arr[j] = temp;
                }
            }
        }
        System.out.print(arr[n-2]);
    }
}
