~~~java
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner keyboard = new Scanner(System.in);
        
        int n = keyboard.nextInt();
        int temp, avr;
        int sum = 0;
        
        for(int i = 0; i < n; i++) {
        	temp = keyboard.nextInt();
        	if(temp >= 60 && temp < 70)
        		temp += 30;
        	if(temp == 0 || temp == 10 || temp == 20 || temp == 30 || temp == 40 || temp == 50 || temp == 60 || temp == 70 || temp == 80 || temp == 90) 
        		temp += 9;
        	if(temp == 6 || temp == 16 || temp == 26 || temp == 36 || temp == 46 || temp == 56 || temp == 66 || temp == 76 || temp == 86 || temp == 96)
        		temp += 3;
        	if(temp > 100) temp = 100;
        	
        	sum = sum + temp;
        }
        
        avr = Math.round((float)sum / n);
        
        System.out.println(avr);
    }
}
~~~
