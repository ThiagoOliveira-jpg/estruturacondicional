Projeto simples e didático desenvolvido em Java que permite ao usuário descobrir o dia da semana correspondente a um número de 1 a 7. Utiliza a estrutura switch-case com repetição para tornar a experiência interativa. Ideal para praticar lógica condicional, controle de fluxo e entrada de dados com Scanner. 

# switch-case-dia-semana
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int x;
        String dia;

        System.out.println("==== CALENDÁRIO SEMANAL ====");

        do {
            System.out.print("\nDigite um número de 1 a 7 para descobrir o dia da semana (ou 0 para sair): ");
            x = sc.nextInt();

            switch (x) {
                case 1:
                    dia = "Domingo";
                    break;
                case 2:
                    dia = "Segunda-feira";
                    break;
                case 3:
                    dia = "Terça-feira";
                    break;
                case 4:
                    dia = "Quarta-feira";
                    break;
                case 5:
                    dia = "Quinta-feira";
                    break;
                case 6:
                    dia = "Sexta-feira";
                    break;
                case 7:
                    dia = "Sábado";
                    break;
                case 0:
                    dia = "Encerrando o programa...";
                    break;
                default:
                    dia = "Valor inválido! Digite um número entre 1 e 7, ou 0 para sair.";
                    break;
            }

            System.out.println("→ " + dia);

        } while (x != 0);

        sc.close();
    }
}
