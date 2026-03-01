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

## TITLE : 2a.) implement class mechanisam 
```
class Rectangle{
  double l;
  double b;
  double area(){
    return l*b;
  }
  double perimeter(){
   return 2*(l+b);
   }
 }
class main{
  public static void main(String args[]){
    Rectangle rect =new Rectangle();
    rect.l=6;
    rect.b=12;
    double area = rect.area();
    double perimeter =rect.perimeter();
    System.out.println("area is:" +area);
    System.out.println("perimeter is:" +perimeter);
    }
  }
```
### output:
![output for class mechanism](https://github.com/sreevidya-1234/javalabcseg-g/blob/d92678301d1d5028c3d49f336b916de29b26104c/2a%20output.png)
## 2b) method overloading
```
class sum{
  int sum(int a ,int b){
    return a+b;
  }
  int sum(int a ,int b,int c){
  return a+b+c;
  }
  double sum(double a ,double b){
   return a+b;
  }
}
class main{
 public static void main(String args[]){
   sum s= new sum();
   System.out.println("sum of 2 integers:"+s.sum(20,16));
   System.out.println("sum of 3 integers:"+s.sum(20,16,17));
   System.out.println("sum of two real numbers:"+s.sum(30.465,15.675));
  }
}
```
### output:
![output of method overloading](https://github.com/sreevidya-1234/javalabcseg-g/blob/26366c43418726ef303fdf592984db19f38a4030/2b%20output.png)
## 2c)implement constructor
```
class student{
 String sname;
 int sage;
 double smarks;
 student(String name,int age,double marks){
   sname=name;
   sage=age;
   smarks=marks;
  }
 void display(){
  System.out.println("student name is :"+sname);
  System.out.println("student age is :"+sage);
  System.out.println("stduent marks is:"+smarks);
  }
}
class main{
 public static void main(String args[]){
  student std= new student("sree",12,960);
  std.display();
  }
}
````
### output:
![output of implement constructor](https://github.com/sreevidya-1234/javalabcseg-g/blob/fbfb5b4470bf639d6fea881364c76819f8cd16de/2c%20output.png)
## add 2)
```
class Fibonacis {

    int firstnumber;
    int secondnumber;
    int thirdnumber;
    int sum;
    int size_of_fibsequence;

    Fibonacis(int size) {
        firstnumber = 0;
        secondnumber = 1;
        thirdnumber = 0;
        sum = 0;
        size_of_fibsequence = size;
    }

    void generate_fibsequence() {

        while (size_of_fibsequence > 0) {

            if (size_of_fibsequence == 1)
                System.out.print(firstnumber + " ");
            else
                System.out.print(firstnumber + " ");

            sum += firstnumber;

            thirdnumber = firstnumber + secondnumber;
            firstnumber = secondnumber;
            secondnumber = thirdnumber;

            size_of_fibsequence--;
        }
    }
```
### output
![output of fibonnoci series](


