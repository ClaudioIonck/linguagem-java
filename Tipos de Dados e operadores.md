* [Tipos de Dados e operadores](Tipos de Dados e operadores.md)
  * Tipos de Dados
    ```
    public class Tipos_de_Dados {

         public static void main(String[] args) {
              System.out.println("Tipos de dados em Java: \n" +
                         "\nMenor Byte: " + Byte.MIN_VALUE +
                         "\nMaior Byte: " + Byte.MAX_VALUE +
                         "\nMenor Short Int: " + Short.MIN_VALUE +
                         "\nMaior Short Int: " + Short.MAX_VALUE +
                         "\nMenor Int: " + Integer.MIN_VALUE +
                         "\nMaior Int: " + Integer.MAX_VALUE +
                         "\nMenor Long: " + Long.MIN_VALUE +
                         "\nMaior Long:" + Long.MAX_VALUE +
                         "\nMenor Float: " + Float.MIN_VALUE +
                         "\nMaior Float: " + Float.MAX_VALUE +
                         "\nMenor Double: " + Double.MIN_VALUE +
                         "\nMaior Double: " + Double.MAX_VALUE);

             }

        }
    ```

  * Declarações de variáveis
    ```
       public class Tipos_Primitivos {
           public static void main(String[] args) {
                 byte tipoByte = 127;
                 short tipoShort = 32767;
                 char tipoChar = 'C';
                 float tipoFloat = 2.6f;
                 double tipoDouble = 3.59;
                 int tipoInt = 2147483647;
                 long tipoLong = 9223372036854775807L;
                 boolean tipoBooleano = true;
                 System.out.println("Valor do tipoByte = " + tipoByte);
                 System.out.println("Valor do tipoShort = " + tipoShort);
                 System.out.println("Valor do tipoChar = " + tipoChar);
                 System.out.println("Valor do tipoFloat = " + tipoFloat);
                 System.out.println("Valor do tipoDouble = " + tipoDouble);
                 System.out.println("Valor do tipoInt = " + tipoInt);
                 System.out.println("Valor do tipoLong = " + tipoLong);
                 System.out.println("Valor do tipoBooleano = " + tipoBooleano);
           }
       }
    ```

  * Nomes válidos para variáveis e boas práticas 
    - Use nomes de variáveis curtas ou longas o suficiente para cada escopo do código. Geralmente o tamanho usado é de 1 (um) caractere para contadores em loops; 1 (uma) palavra para variáveis de loops e condicionais; 1-2 palavras para nomes de métodos; 2-3 palavras para nomes de classes; 3-4 palavras para nomes de variáveis globais.

      Use nomes específicos para cada variável, “valor”, “igual”, “dados” não são nomes validos para nenhum caso.

      Use nomes “significativos” para as variáveis. Através do nome da variável você deve ser capaz de saber o que ela contém.

      Não inicie nomes de variáveis com o_, obj_, m_, etc. Uma variável não precisa de prefixos indicando o estado da variável.

      Obedeça aos padrões definidos na empresa onde trabalha e defina nomes de variáveis consistentes com cada aplicação, por exemplo, “txtUserName”, “lblUserName”, “cmbSchoolType”, caso contrário a falta de legibilidade irá ser prejudicada e o uso de ferramentas para “find/replace” será prejudicado.

      Obedeça aos padrões da linguagem de programação que está sendo utilizada, no caso do Java:
      :arrow: Use para nomes de classes: VelocityResponseWritter

      :arrow: Use para nomes da pacotes: com.company.project.ui

      :arrow: Use para nomes de variáveis: studentName

      :arrow: Não use “_” (underscore) em lugar algum exceto para constantes e valores de enums.

      Não reuse o mesmo nome de variável na mesma classe em diferentes contextos.

      Não use o mesmo nome de variável para diferentes propósitos em um método ou condicional.

      Não use caracteres não-ASCII em nomes de variáveis.

      Não use tamanhos muito longos para nomes de variáveis (mais de 50 caracteres). Caso contrário ficará difícil de ler o código além de que o mesmo pode não rodar em alguns compiladores por causa da limitação de tamanho das linhas.

      Decida pelo uso de uma linguagem natural apenas: ou seja, só português ou só inglês.

      Use nomes significativos para nomes de métodos. O nome deve especificar exatamente a ação executada pelo método, em alguns casos o nome do método deve iniciar por um verbo.

      Use nomes significativos para os parâmetros dos métodos, dessa forma eles podem ser auto-explicativos sem a necessidade de uma documentação explicativa adicional.

      Convenções de código do Java: http://www.oracle.com/technetwork/java/codeconv-138413.html 
  
  * Atribuição de valores
    ```
    int lado = 2;
    float pi = 3.1426F;
    String texto = “DevMedia”;
    lado = 3;
    ```
    
  * Operadores
    * Operadores aritméticos
    * 
      ![image](https://user-images.githubusercontent.com/78597253/188227853-b1fbeabb-56cc-4ef9-a46b-0b963fd8634a.png)
     
   
      ![image](https://user-images.githubusercontent.com/78597253/188228036-f01f1aae-7f96-4861-ad68-40259b45b274.png)
      
      
    * Operadores booleanos
      ![image](https://user-images.githubusercontent.com/78597253/188228248-a126c480-964c-4499-a07d-6ace4e6725ac.png)
      
     
  * Conversão de tipos de dados
    ```
    using System;
    class Teste {
           public static void Main() {
              int i = 1234567;
              double v;
              v = (double) i;
           }
    }
    ```
