public class Main {
    public static void main(String[] args) {
        BmiService service = new BmiService();
             float index = service.calculate(86.5f, 1.780f);
        float index1 = service.calculate(90, 1.70f);
        float index2 = service.calculate(88.2f, 1.780f);
        float index3 = service.calculate(45.4f, 1.680f);
        float index4 = service.calculate(56.2f, 1.780f);
        float index5 = service.calculate(100, 1.780f);

        System.out.println(index);
        System.out.println(index1);
        System.out.println(index2);
        System.out.println(index3);
        System.out.println(index4);
        System.out.println(index5);


            }
}

public class BmiService {

    public float calculate(float weight, float height) {
        float index = weight / (height * height);


        return index;
    }
}
