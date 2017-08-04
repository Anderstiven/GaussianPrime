# GaussianPrime
Este código calcula primos gaussianos
package primosg;

public class PrimosG {

    public static void main(String[] args) {

        int c = 0, cont = 0; //se inicializa variables y contadores
        for (int i = 0; i < 10; i++) {
            for (int j = 0; j < 10; j++) {
                cont = 0;
                c = i * i + j * j;//se realiza la operacion 
                for (int k = c; k > 1; k--) {
                    if (c % k == 0) { //cont cuenta el numero de divisores de c   
                        cont++;
                    }
                }
                if (cont == 1) {//si cont=1 se muestra la pareja (i,j) obtenida
                    System.out.println(i + "+" + j + "i");
                }

            }

        }
    }

}
