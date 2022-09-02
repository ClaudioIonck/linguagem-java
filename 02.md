* [Hello World](02.md)
  * Estrutura mínima de um código Java
      ```
      public class MyClass{
      // código vai aqui
      }
      ```
     
  * Nome do arquivo e Extensão
      - ".java"

  * Nome da classe
      ```
      public class MyClass
      ```
 
  * Método main
      ```
      public static void main(String [] args){ 
      System.out.println("executando código"); }
      ```
      
  * Escrever dados no console
      ```
      import java.util.Scanner;

    /**
     * Neste exemplo pedimos para o usuário digitar a idade,
     * depois imprimimos uma frase com a idade lida.
     */
    public class ExemploScanner {
      public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

    System.out.println("Digite sua idade: ");
    int idade = s.nextInt();
    System.out.println("Vc tem " + idade + " anos.");
      }
    }
      ```
      
  * Indentação de código
    ```
       public class TesteIR {

       public static void main(String[] args) {

           double salary = 3300.00;

           System.out.println("Não deixe de pagar os seus impostos!!");

           if (salary < 1900.00) {
               System.out.println("Pelo valor do seu salário, você não precisa "
                       + "pagar impostos!");

           } else if (salary >= 1900.00 && salary <= 2800.00) {
               System.out.println("O IR a ser pago é de 7.5%, sendo o valor de "
                           + "R$ 142,00 reais!");

           } else if (salary >= 2800.01 && salary <= 3751.00) {
               System.out.println("O IR a ser pago é 15%, sendo o valor de "
                               + "R$ 350,00 reais!");

           } else if (salary >= 3751.01 && salary <= 4664.00) {
               System.out.println("O IR a ser pago é de 22.5%, sendo o "
                                   + "valor de R$ 636,00");
           } else {
               System.out.println("O IR a ser pago para salários acima "
                                   + "de R$ 4664,01 é de 30%");    
           }     
       }        
    }
    ```
    
  * Delimitação de uma instrução
    ```
        public class Exemplo {

        public static void main(String[] args) {
            int resposta = 10;
            if (resposta == 10) { 
                System.out.println(“A resposta é exatamente 10!”);
            } else if (resposta > 10) {
                System.out.println(“A resposta é maior que 10!”);
            } else {
                System.out.println(“A resposta é menor que 10!”);
            }
        }

    }
    ```
    
  * Delimitação de bloco de instruções
    ```
        public class Aula0032 {

        static short c = 'd';

        public static void main(String[] args) {

            short s = 3;
            //Bloco de instrução
            System.out.println("O programa começou.");

            if(1==1){
                double d = 1;

                c = '1';
                s = 1 + 1;
            }

            {
                System.out.println("O mundo é pequeno pra caramba.");
            }
            }
    }
    ```
    
  * Compilação e Execução via linha de comando
    ```
    javac -d bin HelloWorld.java
    ```
