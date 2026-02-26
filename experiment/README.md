#experiment 1
## TITLE : 1a.) DISPLAY PRIMITIVE DATA TYPES
```
class DefaultPrimitiveType {
    byte primbyte;
    short primshort;
    int primint;
    double primdouble;
    char primchar;
    float primfloat;
    long primlong;
    boolean primboolean;
    public static void main(String args[]) {
        DefaultPrimitiveType dDpt = new DefaultPrimitiveType();
        System.out.println("default value of byte:" + dDpt.primbyte);
        System.out.println("default value of short:" + dDpt.primshort);
        System.out.println("default value of int:" + dDpt.primint);
        System.out.println("default value of double:" + dDpt.primdouble);
        System.out.println("default value of char:" + dDpt.primchar + " '");
        System.out.println("default value of float:" + dDpt.primfloat);
        System.out.println("default value of long:" + dDpt.primlong);
        System.out.println("default value of boolean:" + dDpt.primboolean);
    }
  }
```
### output:
![output for DefaultPrimitiveType](https://github.com/sreevidya-1234/javalabcseg-g/blob/5dbcb29d8e92f00f4541dc6cb8360635cc495c41/1a.output.png)
## TITLE : 1b.) QUADRATIC EQUATION
```
import java.util.Scanner;
class Quadratic {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the value of a: ");
        double a = sc.nextDouble();
        System.out.print("Enter the value of b: ");
        double b = sc.nextDouble();
        System.out.print("Enter the value of c: ");
        double c = sc.nextDouble();
        double D = b * b - 4 * a * c;
        if (D > 0) {
            double x1 = (-b + Math.sqrt(D)) / (2 * a);
            double x2 = (-b - Math.sqrt(D)) / (2 * a);
            System.out.println("Two real roots:");
            System.out.println("x1 = " + x1);
            System.out.println("x2 = " + x2);
        } else if (D == 0) {
            double y = -b / (2 * a);
            System.out.println("Roots are equal:");
            System.out.println("y = " + y);
        } else {
            double real = -b / (2 * a);
            double img = Math.sqrt(-D) / (2 * a);
            System.out.println("Roots are complex:");
            System.out.println("x1 = " + real + " + " + img + "i");
            System.out.println("x2 = " + real + " - " + img + "i");
        }
        sc.close();
    }
}
```
### output:
![output for qudratic](https://github.com/sreevidya-1234/javalabcseg-g/blob/017adf91c7cddcfbe542a6a028ce0817c44f8446/1b%20java.png)
