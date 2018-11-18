import java.util.Scanner;

public class Main {
    public static void main(String[] args){
        Scanner keyboard = new Scanner(System.in);
        
        int n = keyboard.nextInt();
        String[] arr = new String[n];
        
        for(int i = 0; i < n; i++) {
        	int sum = 1;
        	int num = keyboard.nextInt();
        	
        	arr[i] = "GoHanGang";
        	
        	for(int j = 2; j <= num; j++) {
        		sum += j;
            	if(((num - sum) % j) == 0) {
            		arr[i] = "Gazua";
            		break;
            	}
        	}
        }
        
        for(int i = 0; i < n; i++) {
        	System.out.println(arr[i]);
        }
        
    }
}
