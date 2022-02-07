# prova-gft-3-2022
prova gft#3

import java.util.Scanner;

public class testaIR {
    public static void main(String[] args) {

        System.out.println("Digite o seu salario bruto");

        Scanner teclado = new Scanner(System.in);

        double salario = teclado.nextDouble();

        if (salario < 1900) {
            System.out.println("nao ha deducao fiscal");

        } else if (salario >= 1900.00 && salario < 2800.00) {
                System.out.println("A deducao fiscal e de 7.5%");
                System.out.println("Voce deve deduzir o valor de " + salario * 0.075 + " reais");

            } else if (salario >= 2800.00 && salario < 3751.00) {
                    System.out.println("A deducao fiscal e de 15%");
                    System.out.println("Voce deve deduzir o valor de " + salario * 0.15 + " reais");

                } else if (salario >= 3751.00 && salario < 4664.00) {
                        System.out.println("A deducao fiscal e de 22,5%");
                        System.out.println("Voce deve deduzir o valor de " + salario * 0.225 + " reais");

                    } else
                        System.out.println("A deducao fiscal e de 27,5%");
                    System.out.println("Voce deve deduzir o valor de " + salario * 0.275 + " reais");

        }
}
