# Action-Comedy
package Module;
import java.util.Scanner;
import java.math.*;
public class moviePrediction {
	public static void main(String[] args) {
		int x1 = 100;
		int y1 = 90;
		
		int x2 = 0;
		int y2 = 100;
		
		int x3 = 90;
		int y3 = 17;
		
		int x4 = 21;
		int y4 = 80;
		
		Scanner sc = new Scanner(System.in);
		int t1 = sc.nextInt();
		int t2 = sc.nextInt();
		
		double s1 = Math.sqrt(Math.pow((x1-t1), 2)+Math.pow((y1-t2), 2));
		double s2 = Math.sqrt(Math.pow((x2-t1), 2)+Math.pow((y2-t2), 2));
		double s3 = Math.sqrt(Math.pow((x3-t1), 2)+Math.pow((y3-t2), 2));
		double s4 = Math.sqrt(Math.pow((x4-t1), 2)+Math.pow((y4-t2), 2));
		
		double minimum = Math.min(Math.min(s1, s2),Math.min(s3, s4));
		System.out.println(minimum);
		
		if(s1 == minimum || s3 == minimum) {
			System.out.println("Action Movie");
		}
		else {
			System.out.println("Comedy Movie");
		}
	}
}
