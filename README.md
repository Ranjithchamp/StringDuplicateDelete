# StringDuplicateDelete
import java.io.InputStreamReader;
import java.util.Scanner;

public class StingDuplicateCharDelete {

	
	public static void main(String[] args) {
		
		int n = 0;
		int c = 0;
		String a;
		char b[];
		Scanner qq = new Scanner(System.in);
		System.out.println("Enter String");
		a = qq.nextLine();
		b = new char[a.length()];
		System.out.println("ouput String is :");
		for (int i = 0; i < a.length(); i++) {
			for (int j = 0; j <= i; j++) {
				if (a.charAt(i) == b[j]) {
					c = 1;
					continue;
				}
			}
			if (c == 0) {
				b[n++] = a.charAt(i);
			}
			c = 0;
		}
		System.out.println(b);
	}
}
