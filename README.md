# Actividad7CJ
import java.util.Scanner;

public class Act7Java {

    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int primo;
        System.out.println("Ingrese hasta que nuemro primo quiere hacer: ");
        primo = sc.nextInt();
            if(primo>0){
                int i =2;
                while(i<=primo){
                    int count = 2;
                    boolean esPrimo = true;
                    while(esPrimo && count < i){
                        if(i%count == 0){
                            esPrimo= false;
                        }
                        else{
                            count++;
                        }
                    }
                    if(esPrimo){
                        System.out.println(i);
                    }
                    i++;
                }
            }
            int init = 0;
            int num = 1;
            int zero;
            int limit;
            System.out.println("Ingrese hasta que numero quiere hacer la serie de fibonacci: ");
            limit=sc.nextInt();
            System.out.println(init);
            System.out.println(num);

                while(num + init <= limit){
                    zero=init;
                    init=num;
                    num=zero+init;
                    System.out.println(num);
                }



    }
}
