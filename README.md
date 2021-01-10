# ucgenKurali
package çalışmalar;

import java.util.Scanner;

public class üçgen {

	public static void main(String[] args) {
		
		Scanner input=new Scanner(System.in);
		System.out.println("1.kenar gir: ");
		float a=input.nextInt();
		System.out.println("2.kenar gir: ");
		float b=input.nextInt();
		System.out.println("3.kenar gir: ");
		float c=input.nextInt();
		
		 if (a+b>c && a+c>b && b+c>a) {
	            if (a==b && a==c) {
	                System.out.println("Eskenar ucgendir");
	            } else if (a!=b && a!=c && b!=c) {
	                System.out.println("Cesitkenar ucgendir.");
	            } else {
	                System.out.println("Ikizkenar ucgendir.");
	            }
	            float cevre = a + b + c;
	            float s = cevre/2;
	            float alan = (float) Math.sqrt(s*(s-a)*(s-b)*(s-c));
	            System.out.println("Cevre: "+ cevre);
	            System.out.println("Alan: " + alan);
	        } else {
	            System.out.print("Ucgen olusturmaz");
	        }
	}

}
