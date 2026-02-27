package modelo;

import java.util.Scanner;

public class CalculaPrestacao {

    private static Object system;

    public static void main (String[] args) {
        Scanner input = new Scanner(System.in);
    System.out.println("Informe o valor");
    double valor = input.nextDouble();

    System.out.println("Informe a taxa");
    double taxa = input.nextDouble();
    System.out.println("Informe o tempo");
    int tempo = input.nextInt();

    double prestacao = valor + (valor * (taxa/100) * tempo);
    System.out.println(prestacao);

    input.close();
    }
}
