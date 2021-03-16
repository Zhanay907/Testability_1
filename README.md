1. public class Main {
2. public static void main(String[] args) {
3.   BmiService service = new BmiService();
4.   float index = service.calculate(86.5f, 1.780f);
5.   float index1 = service.calculate(90, 1.70f);
6.   float index2 = service.calculate(88.2f, 1.780f);
7.   float index3 = service.calculate(45.4f, 1.680f);
8.   float index4 = service.calculate(56.2f, 1.780f);
9.   float index5 = service.calculate(100, 1.780f);
10.
11.  System.out.println(index);
12.  System.out.println(index1);
13.  System.out.println(index2);
14.  System.out.println(index3);
15.  System.out.println(index4);
16.  System.out.println(index5);
17.
18.       }
19.  }



public class BmiService {

    public float calculate(float weight, float height) {
        float index = weight / (height * height);


        return index;
    }
}
