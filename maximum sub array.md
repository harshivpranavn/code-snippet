import java.util.*;

class Main{
    public static void main(String[]args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = sc.nextInt();
        }
        int csum = arr[0];
        int msum = arr[0];
        for(int i=1; i<n; i++){
            csum = Math.max(arr[i],csum+arr[i]);
            msum = Math.max(csum,msum);
        }
        System.out.print(msum);
    }
}
