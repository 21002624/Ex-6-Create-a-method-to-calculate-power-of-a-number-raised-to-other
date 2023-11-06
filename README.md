# Ex-6-Create-a-method-to-calculate-power-of-a-number-raised-to-other
```
import java.util.Scanner;

public class PowerCalculator {
    static double power(double base, int exponent) {
        if (exponent == 0) {
            return 1;
        }
        else {
            return base * power(base, exponent - 1);
        }
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the base: ");
        double base = scanner.nextDouble();
        System.out.print("Enter the exponent: ");
        int exponent = scanner.nextInt();
        double result = power(base, exponent);
        System.out.println(base + "^" + exponent + " is: " + result);
        scanner.close();
    }
}

```
# Output
![Screenshot (70)](https://github.com/21002624/Ex-6-Create-a-method-to-calculate-power-of-a-number-raised-to-other/assets/113762183/c26472bc-bcb4-48ca-8f71-c46b1fcf3b62)

