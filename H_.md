~~~java
import java.util.Scanner;

public class Main {
    public static void main(String[] args){
        Scanner keyboard = new Scanner(System.in);
        
        int n = keyboard.nextInt();
        int ticket;
        
        int[] arr = new int[1000000];
        
        for(int i = 0; i < 1000000; i++) {
        	arr[i] = i+1;
        }
        
        for(int i = 0; i < n; i++) {
        	ticket = keyboard.nextInt();
        	arr[ticket - 1] = 0;
        }
        
        for(int i = 0; i < 1000000; i++) {
        	if(arr[i] != 0) {
        		System.out.println(arr[i]);
        		break;
        	}
        }
    }
}
~~~
