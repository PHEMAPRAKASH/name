# name
public class hpfroloop {
	public static void main(String[] args) {
		int n = 5;
		for (int i = 1; i <= n; i++) {
			for (int j = 1; j <= n; j++) {

				if (j == 1 || j == 5 || i == 3) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int l = 1; l <= n; l++) { // E
				if (i == 1 || i == 3 || i == 5 || l == 1) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int m = 1; m <= n; m++) { // M
				if (m == 1 || m == 5 || (i == m && i <= n / 2 + 1) || (i + m == n + 1 && i <= n / 2 + 1)) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int k = 1; k <= n; k++) { // A
				if (k == 1 || k == 5 || i == 1 || i == 3) {
					System.out.print("*");
				} else
					System.out.print(" ");

			}
			System.out.print(" ");
			for (int a = 1; a <= n; a++) { // P
				if (a == 1 || (i == 1 && a < n) || (i == n / 2 + 1 && a < n) || (a == n && i > 1 && i < n / 2 + 1)) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");

			for (int b = 1; b <= n; b++) { // R
				if ((b == 1 || i == 1 || i == n / 2 + 1 || (i == b && i >= (n / 2 + 1)))) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int c = 1; c <= n; c++) { // A
				if (c == 1 || c == 5 || i == 1 || i == 3) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int d = 1; d <= n; d++) { // K
				if (d == 1 || d + i == 6 || d + i == 10) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int e = 1; e <= n; e++) { // A
				if (e == 1 || e == 5 || i == 1 || i == 3) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int f = 1; f <= n; f++) { // S
				if (i == 1 || i == 3 || i == 5 || (f == 1 && f == n / 2)) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.print(" ");
			for (int g = 1; g <= n; g++) { // H
				if (g == 1 || g == 5 || i == 3) {
					System.out.print("*");
				} else
					System.out.print(" ");
			}
			System.out.println();
		}
	}
}
