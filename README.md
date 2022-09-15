# Linguagem de programação Java
Revisão sobre a linguagem Java

## Tópicos de Estudos

* [Linguagem de programação Java](01.md)
  * Paradigmas de Programação
      - Orientado a objeto
      
  * Modelo de Tipagem de dados
      - Os tipos primitivos são boolean, byte, char, short, int, long, float e double.
      
  * Modelo de construção da Linguagem  
      - Class:
       public class MyClass{
       // código vai aqui
       }
       
      - Methods:
      ```
       public class MyClass{
       public  void meuMetodo(/*argumentos*/){
       }
       }
      ```
      
      - Main:
      ```
       public class MyClass{
       public static void main(String[] args){
       }
       }
      ```
      
  * Estilo de código
      - Chamada de metodo:
      ```
       someMethod(longExpression1, longExpression2, longExpression3,
        longExpression4, longExpression5);

       var = someMethod1(longExpression1,
                       someMethod2(longExpression2,
                               longExpression3));
      ```
      
      - Metodos aritmeticos:
      ```
       longName1 = longName2 * (longName3 + longName4 - longName5)
           + 4 * longname6; // PREFER

       longName1 = longName2 * (longName3 + longName4
                              - longName5) + 4 * longname6; // AVOID
      ```
      
      - Netodos ternarios:
      ```
       alpha = (aLongBooleanExpression) ? beta : gamma;

       alpha = (aLongBooleanExpression) ? beta
           : gamma;

       alpha = (aLongBooleanExpression)
           ? beta
           : gamma;
       ```
       
      - Comentarios:
      ```
       /*
       *Aqui está um bloco de comentário...
       */
      ```
       
      - Declarações:
      ```
       int level; // indentation level
       int size;  // size of table
      ```
      
      - Classes e interfaces:
      ```
       class Sample extends Object {
       int ivar1;
       int ivar2;

       Sample(int i, int j) {
           ivar1 = i;
           ivar2 = j;
       }

       int emptyMethod() {}

       ...
       }
      ``` 
  * Versões
    * Java 1.8
      Funcionalidades do Java 8:
           Aqui há um breve resumo das melhorias incluídas na release 8 do Java:
           Métodos de Expressão Lambda e Extensão Virtual
           O destaque do Java SE 8 é a implementação de expressões Lambda e funcionalidades de suporte para a linguagem de programação e plataforma Java.
           API de Data e Hora
           Essa nova API permitirá que os desenvolvedores tratem data e hora de maneira mais natural, clara e fácil de entender.
           Nashhorn JavaScript Engine
           Uma nova implementação leve de alto desempenho do motor JavaScript foi integrada ao JDk e está disponível para aplicações Java por meio das APIs                      existentes.
           Maior Segurança
           A lista manual existente de métodos sensíveis do chamador foi substituída por um mecanismo que identifica com precisão esses métodos e permite que seus                chamadores sejam descobertos com confiança.
           
    * Java 11
      Funcionalidade do Java 11:
           10 novos scripts, incluindo Adlam, Newa, Tangut e Zanabazar Squar;
           Um coletor de lixo escalável e de baixa latência, ZGC ou Z Garbage Collector, é adicionado junto com o Epsilon GC, um Coletor de Lixo No-op experimental;
           Acessível por meio da JVMTI, um perfil de heap de baixa sobrecarga agora está disponível;
           Adição de um novo método padrão toArray (IntFunction) à interface java.util.Collection;
           As cifras ChaCha20 e ChaCha20-Poly1305 estão disponíveis. ChaCha20 é uma nova cifra de fluxo destinada a substituir a antiga e insegura cifra de fluxo RC4;
           Combina Unicode 9.0.0 e 10.0.0;
           Provedor SunEC aprimorado, suportando 4 curvas adicionais de Brainpool;
           Implementação de um novo esquema de acordo chave usando Curve25519 e Curve448;
           Lançador Java aprimorado para executar um programa fornecido como um único arquivo de código-fonte Java;
           Inclui a implementação do TLS 1.3;
           Introdução de jceks.key.serialFilter, uma propriedade de segurança;
           A JVM agora suporta a organização de classes e interfaces em um ninho, um novo contexto de controle de acesso;
           Novo sinalizador de linha de comando, -XX: + UseDynamicNumberOfCompilerThreads. É adicionado para controlar dinamicamente os threads do compilador;
           O suporte ao algoritmo de assinatura RSASSA-PSS é adicionado ao provedor SunMSCAPI;
           Cliente HTTP Padronizado;
           Suporte para os tipos de criptografia Kerberos 5 de aes128-cts-hmac-sha256-128 e aes256-cts-hmac-sha384-192;
           Dados de localidade atualizados com base no CLDR (Common Locale Data Registry) do Unicode Consortium;
           var, um nome de tipo reservado, é utilizável ao declarar os parâmetros formais de uma expressão lambda.
           
    * Java 18
      Funcionalidades do Java 18:
          Atualizações e melhorias nas bibliotecas

          JEP 400: UTF-8 por padrão – Define UTF-8 como o conjunto de caracteres padrão das APIs Java padrão. Com essa alteração, as APIs que dependem do conjunto de           caracteres padrão se comportarão de forma consistente em todas as implementações, sistemas operacionais, localidades e configurações.
          JEP 408: Simple Web Server – Uma ferramenta de linha de comando e API para iniciar um servidor web mínimo que serve apenas arquivos estáticos. Esta                   ferramenta será útil para prototipagem, codificação ad-hoc e propósitos de teste, particularmente em contextos educacionais.
          JEP 416: Reimplementar Core Reflection com Method Handles – Reimplementa java.lang.reflect.Method, Constructor e Field sobre os handles de método                     java.lang.invoke. Ao tornar o método manipula o mecanismo subjacente para reflexão, ele reduz o custo de manutenção e desenvolvimento das APIs                         java.lang.reflect e java.lang.invoke.
          JEP 418: Resolução de endereço de Internet SPI – Define uma interface de provedor de serviço (SPI) para resolução de nome e endereço de host, para que                 java.net.InetAddress possa usar resolvedores diferentes do resolvedor integrado da plataforma.

          Ferramentas

          JEP 413: Trechos de código JEP na documentação da API Java – Introduz a tag @snippet para o Doclet padrão do JavaDoc para simplificar a inclusão de código-           fonte de exemplo na documentação da API.

          Visualização e incubadoras para versões posteriores do JDK

          JEP 417: Vector API (Terceira Incubadora) – Fornece uma API para desenvolvedores alavancarem de forma confiável arquiteturas de CPU que fornecem extensões             vetoriais escaláveis. Isso levará a um desempenho superior em comparação com cálculos equivalentes em processadores não estendidos.
          JEP 419: Função Estrangeira e API de Memória (Segunda Incubadora) – Permite que programas Java interoperem com código e dados fora do tempo de execução               Java. Ao invocar eficientemente funções externas (ou seja, código fora da JVM) e ao acessar com segurança a memória externa (ou seja, memória não gerenciada           pela JVM), a API permite que programas Java chamem bibliotecas nativas e processem dados nativos sem a fragilidade e as armadilhas de JNI.
          JEP 420: Correspondência de padrões para switch (segunda visualização) – Aprimora a linguagem de programação Java com correspondência de padrões para                 expressões e instruções de switch, juntamente com extensões para a linguagem de padrões. Estender a correspondência de padrões para switch permite que uma             expressão seja testada em vários padrões, cada um com uma ação específica, para que consultas complexas orientadas a dados possam ser expressas de forma               concisa e segura.

          Programas Java à prova de futuro

          JEP 421: Finalização obsoleta para remoção – A finalização permanece habilitada por padrão por enquanto, mas pode ser desabilitada para facilitar o teste.             Em uma versão futura, ela será desabilitada por padrão e, em uma versão posterior, será removida. Os mantenedores de bibliotecas e aplicativos que dependem           da finalização devem considerar a migração para outras técnicas de gerenciamento de recursos, como a instrução try-with-resources e limpadores .

          Suporte a clientes Java

          O Oracle Java SE Subscription é uma oferta previsível de pagamento conforme o uso, oferece aos clientes o melhor suporte da categoria, direito ao GraalVM             Enterprise, acesso ao Java Management Service e flexibilidade para atualizar no ritmo de seus negócios. Isso ajuda as organizações de TI a gerenciar a                 complexidade, conter custos e mitigar os riscos de segurança.
          
    * Java 19 
      Funcionalidades do Java 19:
          
      Uma prévia dos genéricos universais, da Valhalla. Entregues por meio de três JEPs, os genéricos universais unificariam o tratamento de tipos de referência e           primitivos no código genérico, permitindo que as variáveis ​​de tipo Java abrangessem os dois tipos de tipos.Uma visualização de objetos de valor, também um           aprimoramento do Valhalla, fornecendo 
      instâncias de classe que possuem apenas campos de instância final e não possuem identidade de objeto. Classes de valor sem identidade seriam declaradas.
      Uma visualização de padrões de registro, para desconstruir valores de registro. Isso faz parte do Projeto Amber.
      Fixação de região para o coletor de lixo G1, para reduzir a latência implementando a fixação de região para G1 para que a coleta de lixo não precise ser               desabilitada durante regiões 
      críticas JNI (Java Native Interface).Uma porta Linux do JDK para RISC-V, uma arquitetura de conjunto de instruções de código aberto e isenta de royalties.
      
  * Conjunto de palavras reservadas
       - Modificadores de acesso
            private: acesso apenas dentro da classe

            protected: acesso por classes no mesmo pacote e subclasses

            public: acesso de qualquer classe

       - Modificadores de classes, variáveis ou métodos
            abstract: classe que não pode ser instanciada ou método que precisa ser implementado por uma subclasse não abstrata

            class: especifica uma classe

            extends: indica a superclasse que a subclasse está estendendo

            final: impossibilita que uma classe seja estendida, que um método seja sobrescrito ou que uma variável seja reinicializada

            implements: indica as interfaces que uma classe irá implementar

            interface: especifica uma interface

            native: indica que um método está escrito em uma linguagem dependente de plataforma, como o C

            new: instancia um novo objeto, chamando seu construtor

            static: faz um método ou variável pertencer à classe ao invés de às instâncias

            strictfp: usado em frente a um método ou classe para indicar que os números de ponto flutuante seguirão as regras de ponto flutuante em todas as                       expressões

            synchronized:indica que um método só pode ser acessado por uma thread de cada vez

            transient: impede a serialização de campos

            volatile:indica que uma variável pode ser alterada durante o uso de threads

       - Controle de fluxo dentro de um bloco de código
            break: sai do bloco de codigo em que ele está

            case: executa um bloco de código dependendo do teste do switch

            continue:pula a execução do código que viria após essa linha e vai para a próxima passagem do loop

            default:executa esse bloco de codigo caso nenhum dos teste de switch-case seja verdadeiro

            do:executa um bloco de código uma vez, e então realiza um teste em conjunto com o while para determinar se o bloco deverá ser executado novamente

            else: executa um bloco de código alternativo caso o teste if seja falso

            for:usado para realizar um loop condicional de um bloco de código

            if: usado para realizar um teste lógico de verdadeiro o falso

            instanceof: determina se um objeto é uma instância de determinada classe, superclasse ou interface

            return: retorna de um método sem executar qualquer código que venha depois desta linha (também pode retornar uma variável)

            switch:indica a variável a ser comparada nas expressões case

            while: executa um bloco de código repetidamente enquanto a condição for verdadeira

       - Tratamento de erros
            assert: testa uma expressão condicional para verificar uma suposição do programador

            catch: declara o bloco de código usado para tratar uma exceção

            finally:bloco de código, após um try-catch, que é executado independentemente do fluxo de programa seguido ao lidar com uma exceção

            throw:usado para passar uma exceção para o método que o chamou

            throws: indica que um método pode passar uma exceção para o método que o chamou

            try: bloco de código que tentará ser executado, mas que pode causar uma exceção

       - Controle de pacotes
            import:importa pacotes ou classes para dentro do código

            package: especifica a que pacote todas as classes de um arquivo pertencem

       - Primitivos
            boolean:um valor indicando verdadeiro ou falso

            byte: um inteiro de 8 bits (signed)

            char: um caracter unicode (16-bit unsigned)

            double: um número de ponto flutuante de 64 bits (signed)

            float: um número de ponto flutuante de 32 bits (signed)

            int: um inteiro de 32 bits (signed)

            long: um inteiro de 64 bits (signed)

            short: um inteiro de 32 bits (signed)

       - Variáveis de referência
            super: refere-se a superclasse imediata

            this: refere-se a instância atual do objeto

       - Retorno de um método
            void: indica que o método não tem retorno

       - Palavras reservadas não utilizadas
            const: Não utilize para declarar constantes; use public static final

            goto: não implementada na linguagem Java por ser considerada prejudicial.

  * Ambiente de Desenvolvimento e Ferramentas
    * Documentação oficial
      - https://docs.oracle.com/en/java/
    * JDK
      - https://www.oracle.com/java/technologies/downloads/
    * IDEs
      - 1 – Eclipse. 
        2 – Netbeans. 
        3 – IntelliJ IDEA. 
        4 – BlueJ. 
        5 – JDeveloper. 
        6 – JCreator. 
        7 – JGrasp. 
        8 – DrJava.
        
      - Criando um projeto: https://www.alura.com.br/conteudo/intellij-idea-truques-para-aumentar-sua-produtividade-em-projetos-java?                                                             gclid=CjwKCAjwsMGYBhAEEiwAGUXJae_4Anz228D8giU5A9ycNmlfFKhayDRzH117ct6ODugObtKQKieMWxoCXbcQAvD_BwE
        
  * Mercado
    * Popularidade 
      * Tiobe: https://www.tiobe.com/tiobe-index/java/
      * Survey da Stackoverflow: https://survey.stackoverflow.co/2022/
      * Survey da Jetbrains: https://blog.jetbrains.com/blog/tag/survey/
    * Vagas e salários 
      * Survey da Stackoverflow: https://survey.stackoverflow.co/2022/
      * Survey da Jetbrains: https://blog.jetbrains.com/blog/tag/survey/
    * Áreas de aplicações da linguagem Java 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
    * Principais bibliotecas/frameworks 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
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
    
* [Tipos de Dados e operadores](03.md)
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
      !(![image](https://user-images.githubusercontent.com/78597253/188227853-b1fbeabb-56cc-4ef9-a46b-0b963fd8634a.png)
      )
      
      !(![image](https://user-images.githubusercontent.com/78597253/188228036-f01f1aae-7f96-4861-ad68-40259b45b274.png)
      )
      
    * Operadores booleanos
      !(![image](https://user-images.githubusercontent.com/78597253/188228248-a126c480-964c-4499-a07d-6ace4e6725ac.png)
      )
     
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

* [Saída de Dados](04.md)
  * Método System.out.println
    ```
    public class Texto_Simples {
          public static void main(String[] args) {
                        System.out.println(“Seu texto é inserido aqui, entre aspas duplas”);
          }
    }
    ```
    
  * Método System.out.print
    ```
    public class Texto_Simples_print {
          public static void main(String[] args) {
                  System.out.print(“José”);
                  System.out.print(“Silva Moraes”);
          }
    }
    ```

  * Exibir o valor de uma variável
    ```
    public class Main {
        public static void main(String[] args) {
            final float pi = 3.146f;
            final double e;

            e = 1.234e2;

            String nome = "Estevao Dias";
            String dataAniversario = "23/05/2000";
            int lote = 35456;
            boolean aprovado;

            aprovado = true;

            System.out.println(pi); // vai imprimir "3.146f"
            System.out.println(e);// vai imprimir "1.234e2"
            System.out.println(nome);// vai imprimir "Estevao Dias"
            System.out.println(dataAniversario);// vai imprimir "23/05/2000"
            System.out.println(lote);// vai imprimir "35456"
            System.out.println(aprovado);// vai imprimir "true"
        }
    }
    ```

  * Exibir o valor de um decimal 
    ```
    {
        
        Scanner ler = new Scanner(System.in);
        double tempoGasto, vm, distanciaPercorrida, automovel, litros;
        automovel = 12;
        
        System.out.print("Informe o tempo gasto na viagem (em horas): ");
        tempoGasto = ler.nextDouble();
        System.out.print("Informe a velocidade média durante a viagem em km/h: ");
        vm = ler.nextDouble();
        
        distanciaPercorrida = vm / tempoGasto;
        litros = automovel / distanciaPercorrida;
        
        System.out.println(String.format("A distância percorrida´foi de: %.3f Km", distanciaPercorrida));
        System.out.println(String.format("Quantidade de litros necessária: %.3fl.", litros));
    }
    ```
    
* [Classe Math](05.md)
  * Definição
    - A Classe Math (Class Math) do Java
      Para ilustrar o uso de métodos de outras classes e,  de quebra, para nos auxiliar nos cálculos de constantes (como do número pi, do número de euler), no cálculo       de funções trigonométricas (senos, cossenos, tangentes etc) e outras funcionalidades, vamos apresentar e usar a classe Math.
      
  * Principais operações 
    !(![image](https://user-images.githubusercontent.com/78597253/188229604-68a064c9-112f-4888-9947-1c7882f60e36.png)
    )

* [String](06.md)
  * Concatenação de String
    ```
    String txt1 = "Bóson ";
    String txt2 = "Treinamentos ";
    String txt3 = "em Tecnologia";

    System.out.printf("Concatenando: %s%n",txt1.concat(txt2).concat(txt3));
    ```

  * Principais operações sobre String
    - concat:
      ```
      String nomeCompleto = nome + sobrenome;
      ```
      
    - String.valueOf:
      ```
      public class Testa_Metodo_valueOf {
      public static void main(String[] args) {
      double numero = 102939939.939;
      boolean booleano = true;

      System.out.println("Retorna Valor : " + String.valueOf(numero));
      System.out.println("Retorna Valor: " + String.valueOf(booleano));
      ```
      
    - Length:
      ```
      String nomeCurso = "Java";

      System.out.printf("\nTamanho da variável nomeCurso: %d", nomeCurso.length());
      ```
      
    - charAt:
      ```
      String nomeCurso = "JAVA";

      if(nomeCurso.charAt(1) == ‘A’) {
          System.out.println(“O caractere A está na posição 1”);
      }
      ```
      
    - getChars:
      ```
      String nomeCurso = "Curso Java Web";
      //É A DIFERENÇA DO 1º E 2º PARÂMETRO DO MÉTODO getChars
      //SE DIMINUIR OS 2 O RESULTADO TEM QUE SER O MESMO INICIADO NO ARRAY
      char[] numIndice = new char[7];

      nomeCurso.getChars(2, 9, numIndice, 0);
      System.out.print("Valores Copiados \n");

      for(char caracter : numIndice) {
          System.out.print("["+caracter+"]");
      }

      System.out.println("\n\n Abaixo Índice demonstrativo dos valores copiados\n");

      int[] b = {0,1,2,3,4,5,6};
      for(int i = 0; i < b.length; i++) {
          System.out.print("["+b[i]+"]");
      }
      ```
      
    - startsWith e endsWith:
      ```
      String[] nomes = {"iniciado", "iniciando", "finalizado", "finalizando"};

      for (String recebeNomes : nomes) {
          if (recebeNomes.startsWith("in"))
              System.out.printf("\"%s\" inicia com \"in\" \n", recebeNomes);
      }

      System.out.println();

      for (String recebeNomes : nomes) {
          if (recebeNomes.startsWith("ici", 2))
              System.out.printf("\"%s\" inicia com \"ici\" na posição 2 \n", recebeNomes);
      }

      System.out.println();

      for (String recebeNomes : nomes) {
          if (recebeNomes.endsWith("ado"))
              System.out.printf("\"%s\" termina com \"ado\" \n", recebeNomes);
      }
      ```
      
    - indexOf e lastIndexOf:
      ```
      String letras = "abcadefghijklmcopqrsdeftuvz";
      //TESTA indexOf PARA LOCALIZAR UM CARACTERE EM UM STRING
      System.out.printf("Último 'c' está localizado no index %d\n", letras.indexOf('c'));
      System.out.printf("Último 'a' está localizado no index %d \n", letras.indexOf('a', 1));

      //-1 NÃO EXISTE
      System.out.printf("'$' está localizado no index %d\n\n", letras.indexOf('$'));

      //TESTA lastIndexOf PARA LOCALIZAR UM CARACTERE EM UMA STRING
      System.out.printf("Último 'c' está localizado no index %d\n", letras.lastIndexOf('c'));
      System.out.printf("Último 'a' está localizado no index %d\n", letras.lastIndexOf('a', 5));
      System.out.printf("Último '$' está localizado no index %d\n", letras.lastIndexOf('$'));

      //TESTA indexOf PARA LOCALIZAR UMA SUBSTRING EM UMA STRING
      System.out.printf("\"def\" está localizado no index %d\n", letras.indexOf("def"));

      //2 argumento string e outro o ponto inicial que começará a pesquisa
      System.out.printf("\"def\" está localizado no index %d\n", letras.indexOf("def", 7));
      System.out.printf("\"hello\" está localizado no index %d\n\n", letras.indexOf("hello"));
      ```
      
    - substring:
      ```
      String nome = "José Silveira";
      System.out.println("String : " + nome);

      String substring = nome.substring(5);
      System.out.println("String depois da 3º index: " + "["+substring+"]");

      substring = nome.substring(1, 6);
      System.out.println("Substring (1,6): " + "["+substring+"]");
      ```
      
    - replace:
      ```
      String nome = "mesquita";
      String nomeAlterado = nome.replace('e', 'o');
      System.out.println(nomeAlterado);
      ```
      
    - toUpperCase e toLowerCase:
      ```
      String nomeA = "joaquina";
      String nomeB = "Paulo";

      System.out.println(nomeA.toUpperCase());
      System.out.println(nomeB.toLowerCase());
      ```
      
    - toCharArray:
      ```
      String s1 = "olá";
      String s2 = "TCHAU";
      String s3 = " espaços ";

      System.out.println("s1 = "+ s1 + "\n" + "s2 = "+ s2 + "\n" + "s3 = "+s3);

      //MÉTODO REPLACE
      System.out.printf("Replace 'l' por 'L' no s1: %s\n\n", s1.replace('l', 'L'));

      //MÉTODO UPPER E LOWERCASE
      System.out.printf("s1.toUpperCase() = %s\n", s1.toUpperCase());
      System.out.printf("s2.toUpperCase() = %s\n\n", s2.toLowerCase());

      //MÉTODO TRIM - REMOVE OS ESPAÇOS
      System.out.printf("s3 depois do trim = \"%s\"\n\n", s3.trim());

      //CONVERTEU O olá PARA CHAR
      char[] charArray = s1.toCharArray();
      System.out.printf("s1 como um caracter array = ");

      for(char caracter : charArray) {
          System.out.print(caracter);
      }
      ```

  * Comparação de String
    ```
    String s1 = "a";
    String s2 = "a";
    System.out.println(s1.equals(s2));
    ```
    
  * Diferença entre String e caracter
    - Em Java, char é um tipo de dados primitivo usado para conter um único caractere. Significa um único caractere do conjunto de caracteres UTF-16. Em comparação,         String é uma classe que contém uma sequência de caracteres e pode ser considerada uma matriz de caracteres.
    
* [Entrada de Dados](07.md)
  * Classe Scanner
    * Obter um valor inteiro; Obter um valor decimal; Obter um valor de texto:
      ```
      public class Pessoa {

          private Integer codigo;
          private String nome;
          private String endereco;
          private Integer idade;

          public Integer getCodigo() {
            return codigo;
          }

          public void setCodigo(Integer codigo) {
            this.codigo = codigo;
          }

          public String getNome() {
            return nome;
          }

          public void setNome(String nome) {
            this.nome = nome;
          }

          public String getEndereco() {
            return endereco;
          }

          public void setEndereco(String endereco) {
            this.endereco = endereco;
          }

          public Integer getIdade() {
            return idade;
          }

          public void setIdade(Integer idade) {
            this.idade = idade;
          }

          @Override
          public String toString() {
            return "Código: "+codigo+ "" +
                    "\n"+ "Nome: "+nome+"" +
                        "\n"+"Endereço: "+endereco+"" +
                            "\n"+"Idade: "+idade+"\n";
          }
      }
      ```
* [Fluxo de Controle](08.md)
  * Estruturas de Decisões
    * if-else-then
      ```
      class IfElseDemo {
         public static void main(String[] args) {

             int testscore = 76;
             char grade;

             if (testscore >= 90) {
                 grade = 'A';
             } else if (testscore >= 80) {
                 grade = 'B';
             } else if (testscore >= 70) {
                 grade = 'C';
             } else if (testscore >= 60) {
                 grade = 'D';
             } else {
                 grade = 'F';
             }
             System.out.println("Grade = " + grade);
         }
      }
      ```
      
    * switch:
      ```
      switch (expressão) {

      case valor1:

      // bloco de código que será executado

      break;

      case valor2:

      // bloco de código que será executado

      break;

      case valorN:

      // bloco de código que será executado

      break;

      default:

      // bloco de código que será executado se nenhum dos cases for aceito

      }
      ```
      
  * Estruturas de Repetições
    * for
      ```
      public class forSimples{
          public static void main(String[] args) {
              for(int count=10 ; count >= 1; count--){
                  System.out.println(count);
              }
          }
      }
      ```
      
    * while
      ```
      public class Aula0021 {

          public static void main(String[] args) {
              //Estrutura While

      //        enquanto(<=9){
      //            //incremento da variável que está servindo a nossa condição
      //            inteira = inteira + 1;
      //            imprima("essa msg");
      //        }

              //INCREMENTADO - de 0 à 9
              int i = 0;
              while(i<=9){
                  i = i + 1;
                  System.out.println( i );
              }
              /*
               * 1
               * 2
               * 3
               * 4
               * 5
               * 6
               * 7
               * 8
               * 9
               * 10
               */

              //DE-CREMENTADO - de 9 à 0
              int x = 0;
              while(x>=0){
                  x = x - 1;
                  System.out.println( x );
              }
              /*
              * 10
              * 9
              * 8
              * 7
              * 6
              * 5
              * 4
              * 3
              * 2
              * 1
              * 0
              * */

          }

      }
      ```
      
    * do-while 
      ```
      public class JavaDoWhileLoop {

       public static void main(String[] args) {

        int i = 5;
        do {
         System.out.println(i);
         i++;
        } while (i <= 10);
       }
      }
      ```
      
    * Comandos break e continue
      ```
      public class breakTest {
          public static void main(String[] args) {
              long i = System.currentTimeMillis();
              boolean imprimir = true;

              for(int count=1 ; count <=1000000 ; count++){
                  if((count % 17 == 0) && (count % 19 == 0))
                      if(imprimir){
                          System.out.println(count);
                          imprimir=false;
                      }
              }

              System.out.println("Tempo de execução, em milisegundos: "+ (System.currentTimeMillis() -i));
          }

      }
      
      
      public class continueTest {
          public static void main(String[] args) {
              long i = System.currentTimeMillis();

              for(int count=1 ; count <=1000000 ; count++){
                  if(count % 2 == 0){
                      continue;
                  }
                  if((count % 17 == 0) && (count % 19 == 0)){
                      System.out.println(count);
                      break;
                  }

              }

              System.out.println("Tempo de execução, em milisegundos: "+ (System.currentTimeMillis() -i));
          }

      }
      ```
* [Arranjos e Matrizes](09.md)
  * Definição matemática
    - As linguagens de programação procuram dar suporte à implementaçao do conceito de vetores e matrizes existentes na matemática. Na linguagem Java a base deste           suporte são os arranjos. Um arranjo é constituído de uma seqüência indexável de variáveis todas do mesmo tipo. É importante enfatizar que, a menos de algum           vício de linguagem, o termo "arranjo"  e "variável do tipo arranjo" são conceitos bem distintos.

      Um tipo arranjo é uma especialização do tipo referência:
      Já vimos como utilizar as variáveis correspondentes aos oito tipos primitivos. Na linguagem Java, além dos oito tipos primitivos - long, int, short, byte, char,       float, double e boolean, existem as variáveis que podem conter endereços ou referências de memória. Em Java as variáveis do tipo arranjo são especializações de       variáveis deste tipo, denominado tipo referência, ou seja as variáveis do tipo arranjo são também variáveis do tipo referência. Todas as variáveis que não são         de um dos oito tipos primitivos são genericamente conhecidas como variáveis do tipo referência.
      
  * Declaração de arranjos
    ```
    public class Declaracao_Array {
        public static void main(String[] args) {
            //[] - são inseridos em uma variável que referecia um array
            int[] a = new int[4];
            //OUTRA MANEIRA DE FAZER UMA DECLARAÇÃO DE ARRAY
            int[] b;
            b = new int[10];
            //DECLARANDO VÁRIOS ARRAYS
            int[] r = new int[44], k = new int[23];

    //{} - inicializar valores em um array sua declaração
            int[] iniciaValores = {12,32,54,6,8,89,64,64,6};

    //DECLARA UM ARRAY DE INTEIROS
            int[] meuArray;

            //ALOCA MEMÓRIA PARA 10 INTEIROS
            meuArray = new int[10];

            //INICIALIZA O PRIMEIRO ELEMENTO
            meuArray [0] = 100;
            meuArray [1] = 85;
            meuArray [2] = 88;
            meuArray [3] = 93;
            meuArray [4] = 123;
            meuArray [5] = 952;
            meuArray [6] = 344;
            meuArray [7] = 233;
            meuArray [8] = 622;
            meuArray [9] = 8522;
            //meuArray [10] = 564; //ESTOURA A PILHA POIS NÃO EXISTE O ÍNDICE 10

            System.out.println(meuArray[9]);
            System.out.println(meuArray[2]);
        }
    }
    ```
    
  * Declaração de matrizes
    ```
    int [][]matriz = new int[2][];
 
    for(int i=0; i<matriz.length; i++){
        matriz[i] = new int[3]; // ou, por exemplo, = { i, i+1, i+2 };
       for(int j=0; j<matriz[i].length; j++){
          matriz[i][j]=5;
          System.out.print(matriz[0][j]);
       }
       System.out.println(matriz[i][0]);
    }
    ```

  * Percorrer arranjos
    ```
            ArrayList lista = new ArrayList();
                String[] array = {"true", "true", "true", "false", "false"};
                for(int x = 0; x < array.length; x++){
                    if(array[x].equals("true")){
                        lista.add(x);
                    }
                }
                System.out.println(lista.size());
                //verifica o tamanho do arraylist
                if(lista.size() >= 8){
                     System.out.println("aluno aprovado");
                }   
    ```
    
  * Percorrer matrizes
    * Linha a linha:
      ```
      String[][] matriz = {{"Nome1", "Sobrenome1"}, {"Nome2", "Sobrenome2"}, {"Nome3", "Sobrenome3"}};

      for (String[] conjunto : matriz) {
         System.out.println(conjunto[0] + " " + conjunto [1]);
      }

      // ou assim tbm... 
      for(int indice = 0; indice < matriz.length; indice++) {
         String[] conjunto = matriz[indice];
         for(int indiceConjunto = 0; indiceConjunto < conjunto.length; indiceConjunto++) {
            System.out.println(conjunto[indiceConjunto++] + " " + conjunto [indiceConjunto]);	
         }
      }
      ```
      
    * Coluna a coluna:
      ```
      public static void compararColunas(int[][] matriz, int colunaParaComparar) {


          for (int c = 0; c < matriz.length; c++) {
              if (colunaParaComparar != c) {
                  boolean iguais = true;

                  for (int l = 0; l < matriz.length; l++) {
                      if (matriz[l][colunaParaComparar] != matriz[l][c]) {
                          iguais = false;
                          break;
                      }
                  }
                  if (iguais) {
                      System.out.println("A coluna " + colunaParaComparar + " é igual à " + c);
                  }
              }
          }
      }
      ```
      
    * Em diagonal:
      ```
      int D = 0; // soma dos números da diangonal 2

      for (i=0; i<N; i++) {
        D += m[i][i];
      }

      int d = 0; // somas dos números da diangonal 1

      for (i=0; i<N; i++) {

        for (j=N-1; j>=0; j--) {
           d += m[i][j];
           break;
        }
      }
      int df = d - D; // resultado da diferença da soma dos números das diagonais (o que voce quer :D)
      ```
      
  * Utilizar arranjos e matrizes como parâmetros de métodos
    ```
    class aindacpf{
      static int dezena(String cpf){
        int somaprod=0;
        for(int i=0; i<cpf.length(); i++)
          somaprod=somaprod+(cpf.charAt(8-i)-'0')*(i+2);
        int restoAux=somaprod%11;
        return restoAux<2 ? 0 : 11-restoAux;
      }
      static int unidade(String cpf10){
        int somaprod=0;
        for(int i=0; i<cpf10.length(); i++)
          somaprod=somaprod+(cpf10.charAt(9-i)-'0')*(i+2);
        int restoAux=somaprod%11;
        return restoAux<2 ? 0 : 11-restoAux;
      }
      public static void main(String args[]){
        if(args.length!=1){
          System.out.println("Forneca o numero do CPF na linha de comando");
          System.exit(0);
        }
        String cpf= args[0];
        System.out.println("calculo dos digitos verificadores do cpf:"+cpf);
        int dezena=dezena(cpf);
        int unidade=unidade(cpf+dezena);
        System.out.print(dezena);
        System.out.println(unidade);
      }
    }
    ```
    
  * Utilizar arranjos e matrizes como retorno de métodos
    ```
    public class Inicializando_Arrays_Bidimensionais {
        public static void main(String[] args) {

            int[][] array1 = { { 1,2,3 }, { 4, 5, 6 } };
            int[][] array2 = { { 1, 2 }, { 3 }, { 4, 5, 6} };

            System.out.println("Valores no array1 passados na linha são");
            outputArray( array1 ); //exibe o array 2 por linha

            System.out.println("Valores no array2 passados na linha são");
            outputArray( array2 ); //exibe o array 2 por linha

            }
        //FAZ UM LOOP PELAS LINHAS DO ARRAY
        public static void outputArray(int[][] array)
        {
            //FAZ UM LOOP PELAS COLUNAS DA LINHA ATUAL
            for(int linha = 0; linha < array.length; linha++)
            {
                //FAZ LOOP PELAS COLUNAS DA LINHA ATUAL
                for( int coluna = 0; coluna < array[linha].length; coluna++)
                    System.out.printf("%d ", array[linha][coluna]);
                System.out.println();
            }
        }
    }
    ```
    
* [Tratamento de Exceções](10.md)
  * Definição
    - Uma maneira de tentar contornar esses imprevistos é realizar o tratamento dos locais no código que podem vir a lançar possíveis exceções, como por exemplo,           campo de consulta a banco de dados, locais em que há divisões, consulta a arquivos de propriedades ou arquivos dentro do próprio computador.
      Para tratar as exceções em Java são utilizados os comandos try e catch.
      
  * Exceções comuns
    * Divisão por zero
      ```
      // Java Program to Handle Divide By Zero Exception
      import java.io.*;
      class GFG {
          public static void main(String[] args)
          {
              int a = 5;
              int b = 0;
              try {
                  System.out.println(a / b); // throw Exception
              }
              catch (ArithmeticException e) {
                  // Exception handler
                  System.out.println(
                      "Divided by zero operation cannot possible");
              }
          }
      }
      ```
      
    * Conversão de tipos de dados inválidos
      ```
      Ocorreu uma exceão ao executar o método aumentarLetras()
      java.lang.Exception: java.lang.NullPointerException
      ```
      
    * Acessar uma posição inválida em um arranjo
      ```
      public class UnderAgeException extends Exception {
          private int _age;

          public UnderAgeException(String message, int age) {
                  super(message);
                  this._age = age;
          }

          // Use the getAge method to get the value that caused the exception.
          public int getAge() {
                  return _age;
          }
      }
      ```
      
    * Acessar uma String nula
      ```
      public static boolean cartaoExistente(CartaoDeCredito cartaoDeCredito, Usuario usuario){
         for (CartaoDeCredito cartao : usuario.getCartoes()) {
            if(cartaoDeCredito.getNumero().equals(cartao.getNumero())){
               return false;
            }
         }
      return true;
      }
      ```
      
  * Bloco para capturar uma exceção
    ```
    try
    {
      //trecho de código que pode vir a lançar uma exceção
    }
    catch(tipo_exceçao_1 e)
    {
      //ação a ser tomada
    }
    catch(tipo_exceçao_2 e)
    {
      //ação a ser tomada
    }
    catch(tipo_exceçao_n e)
    {
      //ação a ser tomada
    }
    ```
    
  * Bloco para capturar diferentes exceções 
    ```
    import java.util.InputMismatchException;
    import java.util.Scanner;

    public class Exemplo_PrintStrackTrace {

      public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        try {
          System.out.print("Digite a idade: ");
          int idade = sc.nextInt();

          System.out.println(idade);
        } catch (InputMismatchException e) {
          e.printStackTrace();
        }
      }
    }
    ```
    
  * Bloco finally
    ```
    try
    {
      //trecho de código que pode vir a lançar uma exceção
    }
    catch(tipo_exceçao_1 e)
    {
      //ação a ser tomada
    }
    catch(tipo_exceçao_2 e)
    {
      //ação a ser tomada
    }
    catch(tipo_exceçao _n e)
    {
      //ação a ser tomada
    }
    finally
    {
      //ação a ser tomada
    }
    ```
    
  * Lançar uma exceção
    ```
    class Regr{
    static void moeda() throws Exception{
    throw new Exception();
    }
    public static void main(String args[]){
    try{
    moeda();
    }
    catch(Exception e){
    throw  e;
    }
    }}
    ```

* [Métodos estáticos](11.md)
  * Estrutura de declaração de um método estático
    ```
    public class Teste_Metodo_Static {

     public static void main(String[] args) {
      double num1 = 8.5;
      double pi = Math.PI;

      System.out.println("Valor num1 = "+num1);
      System.out.println("Valor PI = "+pi);

      System.out.println("Soma dos valores = "+(num1+pi));

     }

    }
    ```
    
  * Nomes válidos e boas práticas
    - Use nomes específicos para cada variável, “valor”, “igual”, “dados” não são nomes validos para nenhum caso.

      Use nomes “significativos” para as variáveis. Através do nome da variável você deve ser capaz de saber o que ela contém.

      Não inicie nomes de variáveis com o_, obj_, m_, etc. Uma variável não precisa de prefixos indicando o estado da variável.

      Obedeça aos padrões definidos na empresa onde trabalha e defina nomes de variáveis consistentes com cada aplicação, por exemplo, “txtUserName”, “lblUserName”,         “cmbSchoolType”, caso contrário a falta de legibilidade irá ser prejudicada e o uso de ferramentas para “find/replace” será prejudicado.

      Obedeça aos padrões da linguagem de programação que está sendo utilizada, no caso do Java:
      :arrow: Use para nomes de classes: VelocityResponseWritter

      :arrow: Use para nomes da pacotes: com.company.project.ui

      :arrow: Use para nomes de variáveis: studentName

      :arrow: Não use “_” (underscore) em lugar algum exceto para constantes e valores de enums.
      
  * Parâmetros 
    ```
    public void incrementa (int num) {
        num++;
        System.out.println(“num : ” + num);
    }

    // veja agora

    int num = 10;

    incrementa (num); //Imprimirá 11

    System.out.println(”num : ” + num); //Imprimirá 10
    ```
    
  * Retorno
    ```
    class Metodo3{

     String nome = "João Silva";

     public String retornaNome()
     {
      return nome;
     }
    }

    public class Metodo_Com_Retorno {

     public static void main(String[] args) {

      Metodo3 m3 = new Metodo3();
      System.out.println(m3.retornaNome());

     }

    }
    ```
  
  * Utilização de métodos estáticos 
    * Disponíveis na mesma classe:
      ```
      public class Conta {

       private Double saldo;

       public void setSaldo(Double saldo) {
        this.saldo = saldo;
       }

       public Double getSaldo() {
        return saldo;
       }

       public void depositar(Double valor){
        saldo += valor;
       }

       public void verificaSaldo(){
        System.out.println("Valor do Saldo: "+getSaldo());
       }
      }
      
      
      public static void main(String[] args) {

       //INSTANCIA A CLASSE
       Conta conta = new Conta();

       //DEFINE UM VALOR DE SALDO
       conta.setSaldo(633.00);

       //DEFINE VALOR PARA DEPOSITAR
       conta.depositar(555.0);

       //RESGATA VALOR
       conta.verificaSaldo();

      }
      ```
      
    * Disponíveis em outra classe/arquivo:
      ```
      public class Teste_Metodo_Static {

       public static void main(String[] args) {
        double num1 = 8.5;
        double pi = Math.PI;

        System.out.println("Valor num1 = "+num1);
        System.out.println("Valor PI = "+pi);

        System.out.println("Soma dos valores = "+(num1+pi));

       }

      }
      
      -------------------------------------------------------------------
      
      class Soma{

       public static int resultado(int num1, int num2){
        return (num1 + num2);
       }
      }

      public class TestaSomaEstatica {

       public static void main(String[] args) {

        System.out.println(Soma.resultado(10,50));
       }
      }
      ```
      
  * Recursão 
    ```
    public class ImprimirPares {
      public static void main(String[] args) {
        System.out.println("Inicio do programa.");
        ImprimirPares ip = new ImprimirPares();
        ip.imprimir(5);
        System.out.println("Fim do programa.");
      }

      private void imprimir(int x) {
        int soma = 0;

        for(int cont = 0; cont < x; cont++) {
          if(cont % 2 == 0)
            soma = soma + cont;
        }

        System.out.println("Soma dos pares: " + soma);
      }
    }
    ```





--------------------------------------------------------------------
Continuara...






* 10. Tratamento de Exceções
  * Definição
  * Exceções comuns
    * Divisão por zero
    * Conversão de tipos de dados inválidos
    * Acessar uma posição inválida em um arranjo
    * Acessar uma String nula
  * Bloco para capturar uma exceção 
  * Bloco para capturar diferentes exceções 
  * Bloco finally
  * Lançar uma exceção
* 11. Métodos estáticos
  * Estrutura de declaração de um método estático
  * Nomes válidos e boas práticas 
  * Parâmetros 
  * Retorno
  * Utilização de métodos estáticos 
    * Disponíveis na mesma classe
    * Disponíveis em outra classe/arquivo. 
  * Recursão 
* 12. Classe
  * Definição:
    ```
    Uma classe é um elemento do código Java que utilizamos para representar objetos do mundo real. Dentro dela é comum declararmos atributos e métodos, que               representam, respectivamente, as características e comportamentos desse objeto.
    ```
    
    * Representação de classe e objeto na UML
      <br>
      ![image](https://user-images.githubusercontent.com/78597253/190504594-45e35fec-7552-4d15-92b3-dbc4011e9672.png)
      <br>

    * Diferença entre classe e objeto
      ```
      A diferença é que um classe é uma especificação. Um projeto Ex:
      
      Class Conta{
          int numero;
          String dono;
          double saldo;
      }
      
      Com esse projeto de conta não podemos acessar saldo nem ver quem é o dono nada, precisamos construir apartir desse projeto um objeto desse tipo.

      Apesar de declararmos que toda conta tem um saldo, um número e um dono no projeto, são nas instâncias desse projeto que realmente há espaço para armazenar esses       valores.

      Ao projeto da conta, isto é, a definição da conta, damos o nome de classe. Ao que podemos construir a partir desse projeto, as contas de verdade, damos o nome         de objetos.
      
      class Programa {
        public static void main(String[] args) {
          Conta minhaConta = new Conta();
        }
      }
      ```
      
  * Atributos
    ```
    public class Caes {

     public String nome;
     public int peso;
     public String corOlhos;
     public int quantPatas;

     public void falar(){
      //MÉTODO FALAR
     }

     public void andar(){
      //MÉTODO ANDAR
     }

     public void comer(){
      //MÉTODO COMER
     }

     public void dormir(){
      //MÉTODO DORMIR
     }
    }
    ```
    
  * Métodos
    ```
    public class Teste_Metodo_Static {

     public static void main(String[] args) {
      double num1 = 8.5;
      double pi = Math.PI;

      System.out.println("Valor num1 = "+num1);
      System.out.println("Valor PI = "+pi);

      System.out.println("Soma dos valores = "+(num1+pi));

     }

    }
    ```
    
  * Construtor
    ```
    // Create a Main class
    public class Main {
      int x;  // Create a class attribute

      // Create a class constructor for the Main class
      public Main() {
        x = 5;  // Set the initial value for the class attribute x
      }

      public static void main(String[] args) {
        Main myObj = new Main(); // Create an object of class Main (This will call the constructor)
        System.out.println(myObj.x); // Print the value of x
      }
    }
    ```
    
  * Objeto
    ```
    public class Main {
      int x = 5;

      public static void main(String[] args) {
        Main myObj1 = new Main();  // Object 1
        Main myObj2 = new Main();  // Object 2
        System.out.println(myObj1.x);
        System.out.println(myObj2.x);
      }
    }
    ```
    
  * Inicialização de um objeto 
    ```
    Referencia:
    
    class Aluno {  
     int id;  
     String nome;  
    }  
    class TesteAluno2 {  
     public static void  main(String args []) {  
      Aluno a1 = new Aluno();  
      a1.id = 101 ;  
      a1.nome = "Sonoo" ;  
      System.out.println(a1.id + "" + s1.nome); // imprimindo membros com um espaço em branco   
     }  
    }  
    ```
    
    ```
    Por metodo:
    
    class  Aluno {    
     int  id;    
     String nome;    
    }    
    class  TesteAluno3 {    
     public static void  main (String[] args) {      
      //Criando objetos    
      Aluno a1 = new  Aluno();    
      Aluno a2 = new  Aluno();    
      //Inicializando objetos    
      a1.id = 101 ;    
      a1.nome = "Sonoo";    
      a2.id = 102 ;    
      a2.nome = "Amit";    
      //Imprimindo dados    
      System.out.println(a1.id + "" + a1.nome);    
      System.out.println(a2.id + "" + a2.nome);    
     }    
    } 
    ```
    
    ```
    Por construtor:
    
    class  Funcionario {  
        int id;  
        String nome;  
        float salario;  
        void inserir(int  i, String n,  float  s) {  
            id = i;  
            nome = n;  
            salario = s;  
        }  
        void  exibir() {System.out.println (id + "" + nome + "" + salario);}  
    }  
    public class TesteFuncionario {   
                public static void  main (String [] args) {    
                            Funcionario f1 = new Funcionario();  
                            Funcionario f2 = new Funcionário();  
                            Funcionario f3 = new Funcionario();  
                            f1.inserir(101, "João", 45000);  
                            f2.inserir(102, "Antônio", 25000);  
                            f3.inserir(103, "Maria", 55000);  
                            f1.exibir();  
                            f2.exibir();  
                            f3.exibir();  
                }  
    }  
    ```
    
  * Utilização de um objeto
    ```
    class Aluno {  
     int id;  
     String nome;  
    }  
    
    
    class TesteAluno2 {  
     public static void  main(String args []) {  
      Aluno a1 = new Aluno();  
      a1.id = 101 ;  
      a1.nome = "Sonoo" ;  
      System.out.println(a1.id + "" + s1.nome); // imprimindo membros com um espaço em branco   
     }  
    }  
    
    ```

  * Comparação de objetos
    ```
    // Java Program to compare two objects

    // Importing java input output library
    import java.io.*;

    // Class 1
    class Pet {
     // attributes of class1
     String name;
     int age;
     String breed;

     // constructor of class 1
     Pet(String name, int age, String breed)
     {
      // Assignment of current attributes
      /// using this keyword with same
      this.name = name;
      this.age = age;
      this.breed = breed;
     }
    }

    /* Class 2 : where execution is shown
       for class 1 */
    public class GFG {

     // Main driver method
     public static void main(String args[])
     {

      // Objects of class1 (auxiliary class)
      // are assigned value */
      Pet dog1 = new Pet("Snow", 3, "German Shepherd");
      Pet cat = new Pet("Jack", 2, "Tabby");
      Pet dog2 = new Pet("Snow", 3, "German Shepherd");

      // Checking objects are equal and
      // printing output- true/false
      System.out.println(dog1.equals(dog2));
     }
    }
    ```
    
  * Método toString
    ```
    class Pet{

      String name;
      Integer age; 

      Pet(String n, Integer a){
        this.name=n;
        this.age=a;
      }
    //Over-riding the toString() function as a class function
      public String toString(){
        return "The name of the pet is " + this.name + ". The age of the pet is " + this.age;
      }
    }

    class HelloWorld {
        public static void main( String args[] ) {
          Pet p = new Pet("Jane",10);
          //Calling the class version of toString()
            System.out.println(p.toString());
          //Calling the original toString()
          System.out.println(Integer.toString(12));
        }
    }
    ```
    
  * Visibilidade de atributos e métodos
    ![image](https://user-images.githubusercontent.com/78597253/190509404-29017373-03e7-47ac-8c54-6da7508ceb5e.png)

    * Público
    * Privado 
      ![image](https://user-images.githubusercontent.com/78597253/190509778-01022349-1924-4333-bd75-5ca9ff1149ae.png)

  * Sobrecarga de métodos
    ```
    static int plusMethodInt(int x, int y) {
      return x + y;
    }

    static double plusMethodDouble(double x, double y) {
      return x + y;
    }

    public static void main(String[] args) {
      int myNum1 = plusMethodInt(8, 5);
      double myNum2 = plusMethodDouble(4.3, 6.26);
      System.out.println("int: " + myNum1);
      System.out.println("double: " + myNum2);
    }
    ```

  * Sobrecarga de construtores
    ```
    // Java program to illustrate role of this() in
    // Constructor Overloading
    class Box
    {
     double width, height, depth;
     int boxNo;

     // constructor used when all dimensions and
     // boxNo specified
     Box(double w, double h, double d, int num)
     {
      width = w;
      height = h;
      depth = d;
      boxNo = num;
     }

     // constructor used when no dimensions specified
     Box()
     {
      // an empty box
      width = height = depth = 0;
     }

     // constructor used when only boxNo specified
     Box(int num)
     {
      // this() is used for calling the default
      // constructor from parameterized constructor
      this();

      boxNo = num;
     }

     public static void main(String[] args)
     {
      // create box using only boxNo
      Box box1 = new Box(1);

      // getting initial width of box1
      System.out.println(box1.width);
     }
    }
    ```
    

    --------------------------------------------------------------------
    
* 13. Pacotes 
  * Definição
    ```
    Pacotes java são utilizados para organizar as classes da sua aplicação. Um programa pode, facilmente, ter mais de centenas de classes. Então é muito importante       que todos os seus componentes fiquem organizados. Podemos pensar nos pacotes como uma pasta do seu sistema de arquivos.
    ```
     * Representação de pacotes na UML
       ![image](https://user-images.githubusercontent.com/78597253/190510825-1ab92f29-15f5-43b6-98a9-6c28762bc083.png)

  * Definição de um pacote em uma classe
    ```
    import package.name.Class;   // Import a single class
    import package.name.*;   // Import the whole package
    
    import java.util.Scanner;
    
    import java.util.Scanner;

    class MyClass {
      public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in);
        System.out.println("Enter username");

        String userName = myObj.nextLine();
        System.out.println("Username is: " + userName);
      }
    }
    ```
    
  * Importando uma classe de um pacote diferente
    ```
    import com.my.stuff.main.Main;
    import com.my.stuff.second.*;
    
    package com.my.stuff.main

    import com.my.stuff.second.Second;   // THIS IS THE IMPORTANT LINE FOR YOUR QUESTION

    class Main {
       public static void main(String[] args) {
          Second second = new Second();
          second.x();  
       }
    }
    ```
    
  * Visibilidade de classes, atributos e métodos
    ```
       package br.visibilidade.outropacote;

       import br.visibilidade.Produto;

       /**
        * Classe utilizada para testar a visibilidade protected
        * do atributo e métodos da classe Produto a partir de outro
        * pacote.
        */
       public class TesteProdutoOutroPacote {
         public static void main(String[] args) {
           Produto prodCaneta = new Produto();
           prodCaneta.setNomeProduto("Caneta");
           System.out.println(prodCaneta.getNomeProduto());
         }
       }
    ```
     * Default/Pacote  
       ```
       public class FindEvenOdd {  
       public static void main(String args[])   
       {  
       int number=87;  
       //returns true if num is perfectly divisible by 2  
       if(number % 2 == 0)  
       System.out.println(number +" is even number.");  
       else  
       System.out.println(number +" is odd number.");  
       }  
       }  
       
       
       
       
       import java.io.PrintStream;  
       public class FindEvenOdd   
       {   
       public FindEvenOdd()   
       {  
       }  
       public static void main(String[] paramArrayOfString)   
       {   
       int i = 87;  
       if (i % 2 == 0)   
       {  
       System.out.println(i + " is even number.");  
       }   
       else   
       {  
       System.out.println(i + " is odd number.");  
       }  
       }  
       }  
       ```
       
  * Pacote default
    * Importar uma classe em um pacote default 
      ```
      public class FindEvenOdd  
      {  
      public static void main(String args[])   
      {  
      int number=87;  
      //returns true if num is perfectly divisible by 2  
      if(number % 2 == 0)  
      System.out.println(number +" is even number.");  
      else  
      System.out.println(number +" is odd number.");  
      }  
      }   
      
      
      
      import java.io.PrintStream;  
      public class FindEvenOdd   
      {   
      public FindEvenOdd()   
      {  
      }  
      public static void main(String[] paramArrayOfString)   
      {   
      int i = 87;  
      if (i % 2 == 0)   
      {  
      System.out.println(i + " is even number.");  
      }   
      else   
      {  
      System.out.println(i + " is odd number.");  
      }  
      }  
      }  
      ```
      
      --------------------------------------------------------------------
      
      
* Escopo de classe e objeto
  ```
  public class principal {
 
  public static void main(String[] args)
    {
        Planetas marte = new Planetas(3.0, 1.5, 6.419e23);

        marte.apelido = "Marte";

        System.out.println("Quantidade de planetas: " + Planetas.numeroDePlanetas);
        System.out.println("Nome do Planeta: " + marte.apelido);
        System.out.println("As outras variaveis da classe não podem ser alcançadas devido ao escopo");
        System.out.println("mas podem ser utlizadas dentro da classe");
    }
   }
  ```
  * Definição:
    ```
    Escopo refere-se à vida e acessibilidade de uma variável. Quão grande é o alcance depende de onde uma variável é declarada. Por exemplo, se uma variável é             declarada na parte superior de uma classe, ela será acessível a todos os métodos de classe. Se for declarada num método, em seguida, só pode ser utilizada em tal     método.

    O escopo de uma variável é a parte do programa que pode acessar uma variável. Quando você tenta acessar uma variável que não está no escopo, você normalmente tém     um erro do compilador
    ```
    
  * Palavra reservada static 
    ```
    public class Calculo {
    static Montagem m = new Montagem();

    public static void main(String args[])
    {
    Calculo cl = new Calculo();
    cl.printMessage(“Mensagem escrita em java”);
    m.mostraMontagem(“Frase de calculo escrita em montagem”);

     }
     private void printMessage(String msg)
      {
        System.out.println(msg);
       };
    }

    class Montagem {
    public Montagem()
    {

        }
       public static void mostraMontagem(String palavra)
         {
           System.out.println(palavra);
         }
    }
    ```
    
* Herança
  * Definição
    ```
    A herança é um princípio da POO que permite a criação de novas classes a partir de outras previamente criadas. Essas novas classes são chamadas de subclasses, ou     classes derivadas; e as classes já existentes, que deram origem às subclasses, são chamadas de superclasses, ou classes base.
    ```
    
     * Representação de herança na UML
       ![image](https://user-images.githubusercontent.com/78597253/190514570-f90558cd-4bcc-4a25-8517-2c739ea0dacb.png)

  * Criação de uma classe que realiza herança 
    ```
    public class Bicycle {
        
    // the Bicycle class has three fields
    public int cadence;
    public int gear;
    public int speed;
        
    // the Bicycle class has one constructor
    public Bicycle(int startCadence, int startSpeed, int startGear) {
        gear = startGear;
        cadence = startCadence;
        speed = startSpeed;
    }
        
    // the Bicycle class has four methods
    public void setCadence(int newValue) {
        cadence = newValue;
    }
        
    public void setGear(int newValue) {
        gear = newValue;
    }
        
    public void applyBrake(int decrement) {
        speed -= decrement;
    }
        
    public void speedUp(int increment) {
        speed += increment;
    }
    
    
    
    
    public class MountainBike extends Bicycle {
        
    // the MountainBike subclass adds one field
    public int seatHeight;

    // the MountainBike subclass has one constructor
    public MountainBike(int startHeight,
                        int startCadence,
                        int startSpeed,
                        int startGear) {
        super(startCadence, startSpeed, startGear);
        seatHeight = startHeight;
    }   
        
    // the MountainBike subclass adds one method
    public void setHeight(int newValue) {
        seatHeight = newValue;
    }   
    }
    ```  

  * Sobreescrita de métodos
    ```
    // A Simple Java program to demonstrate
    // Overriding and Access-Modifiers

    class Parent {
     // private methods are not overridden
     private void m1()
     {
      System.out.println("From parent m1()");
     }

     protected void m2()
     {
      System.out.println("From parent m2()");
     }
    }

    class Child extends Parent {
     // new m1() method
     // unique to Child class
     private void m1()
     {
      System.out.println("From child m1()");
     }

     // overriding method
     // with more accessibility
     @Override
     public void m2()
     {
      System.out.println("From child m2()");
     }
    }

    // Driver class
    class Main {
     public static void main(String[] args)
     {
      Parent obj1 = new Parent();
      obj1.m2();
      Parent obj2 = new Child();
      obj2.m2();
     }
    }
    ```
   
  * Polimorfismo
    ```
    interface GUIFactory
    public Menu createMenu();
    }

    class WinFactory implements GUIFactory {

    public Menu createMenu() {
    return new WinMenu();
    }
    }

    class LinuxFactory implements GUIFactory {
    public Menu createMenu() {
    return new LinuxMenu();
    }
    }
    
    
    
    
    interface Menu {
    public void paint();
    }

    class WinMenu implements Menu {
    public void paint() {
    System.out.println("Eu sou um WinMenu");
    }
    }

    class LinuxMenu implements Menu {
    public void paint() {
    System.out.println("Eu sou um LinuxMenu");
    }
    }
    
    
    
    class Aplicacao {
    public Aplicacao(GUIFactory factory) {
    Menu menu = factory.createMenu();
    menu.paint();
    }
    }

    class Principal {
    public static void main(String args[]) {
    chamar Application();
    //De preferencia leia de algum lugar e coloque a opção na variável
    int tipoDeMenu = 0;
    if (tipoDeMenu == 0)
    new Aplicacao(new WinFactory());
    else
    new Aplicacao(new LinuxFactory());
    }
    }
    ```
    
    * Conversão de tipos 
      ```
      import java.util.Scanner;
      public class NarrowingExample {
         public static void main(String args[]){
            Scanner sc = new Scanner(System.in);
            System.out.println("Enter an integer value: ");
            int i = sc.nextInt();
            char ch = (char) i;
            System.out.println("Character value of the given integer: "+ch);
         }
      }
      ```
      
  * Visibilidade de atributos e métodos
    ```
    public class Animal {
      public void eat() { /* Do something */ }
    }
    
    public class Dog extends Animal {
    }

    public class Dog extends Animal {
      public void bark() { /* Do something */ }
    }
    
    class Toy {} 

    class Animal{} 

    // Cat is an Animal, so Cat class extends Animal class.
    class Cat extends Animal { 
     // Cat has a Toy, so Cat has an instance of Toy as its member.
     private Toy toy; 
    }
    ```
     * Protegido
       ```
       class Person {
         protected String fname = "John";
         protected String lname = "Doe";
         protected String email = "john@doe.com";
         protected int age = 24;
       }

       class Student extends Person {
         private int graduationYear = 2018;
         public static void main(String[] args) {
           Student myObj = new Student();
           System.out.println("Name: " + myObj.fname + " " + myObj.lname);
           System.out.println("Email: " + myObj.email);
           System.out.println("Age: " + myObj.age);
           System.out.println("Graduation Year: " + myObj.graduationYear);
         }
       ```

  * Palavra reservada super 
    ```
    class Animal { // Superclass (parent)
      public void animalSound() {
        System.out.println("The animal makes a sound");
      }
    }

    class Dog extends Animal { // Subclass (child)
      public void animalSound() {
        super.animalSound(); // Call the superclass method
        System.out.println("The dog says: bow wow");
      }
    }

    public class Main {
      public static void main(String args[]) {
        Animal myDog = new Dog(); // Create a Dog object
        myDog.animalSound(); // Call the method on the Dog object
      }
    }
    ```
     * Encadeamento de construtor
       ```
        @SerializedName("new")
        private String New;
       public String getNew ()
        {
            return New;
        }
        public void setNew (String aNew)
        {
            New = aNew;
        }
       ```
     * Encadeamento de método
       ```
       class A {

        private int a;
        private float b;

        A() { System.out.println("Calling The Constructor"); }

        int setint(int a)
        {
         this.a = a;
         return this.a;
        }

        float setfloat(float b)
        {
         this.b = b;
         return this.b;
        }

        void display()
        {
         System.out.println("Display=" + a + " " + b);
        }
       }

       // Driver code
       public class Example {
        public static void main(String[] args)
        {
         // This will return an error as
         // display() method needs an object but
         // setint(10) is returning an int value
         // instead of an object reference
         new A().setint(10).display();
        }
       }
       ```
       
* Interface
  * Definição
    ```
    A interface é um recurso muito utilizado em Java, bem como na maioria das linguagens orientadas a objeto, para “obrigar” a um determinado grupo de classes a ter       métodos ou propriedades em comum para existir em um determinado contexto, contudo os métodos podem ser implementados em cada classe de uma maneira diferente.
    ```
     * Representação de interface na UML
       ![image](https://user-images.githubusercontent.com/78597253/190518875-7192118d-cdda-4057-9096-701dca20dda4.png)

  * Criação de uma classe que implementa uma interface
    ```
    public interface FiguraGeometrica
    {
     public String getNomeFigura();
     public int getArea();
     public int getPerimetro();
    }
    
    
    
    public class Quadrado implements FiguraGeometrica {

        private int lado;

        public int getLado() {
            return lado;
        }

        public void setLado(int lado) {
            this.lado = lado;
        }

        @Override
        public int getArea() {
            int area = 0;
            area = lado * lado;

            return area;
        }

        @Override
        public int getPerimetro() {
            int perimetro = 0;

            perimetro = lado * 4;
            return perimetro;
        }

        @Override
        public String getNomeFigura() {
            return "quadrado";
        }
    }
    
    
    
    public class Triangulo implements FiguraGeometrica {

        private int base;
        private int altura;
        private int ladoA;
        private int ladoB;
        private int ladoC;

        public int getAltura() {
            return altura;
        }

        public void setAltura(int altura) {
            this.altura = altura;
        }

        public int getBase() {
            return base;
        }

        public void setBase(int base) {
            this.base = base;
        }

        public int getLadoA() {
            return ladoA;
        }

        public void setLadoA(int ladoA) {
            this.ladoA = ladoA;
        }

        public int getLadoB() {
            return ladoB;
        }

        public void setLadoB(int ladoB) {
            this.ladoB = ladoB;
        }

        public int getLadoC() {
            return ladoC;
        }

        public void setLadoC(int ladoC) {
            this.ladoC = ladoC;
        }

        @Override
        public String getNomeFigura() {
            return "Triangulo";
        }

        @Override
        public int getArea() {
            int area = 0;
            area = (base * altura) / 2;
            return area;
        }

        @Override
        public int getPerimetro() {
            int perimetro = 0;
            perimetro = ladoA + ladoB + ladoC;

            return perimetro;
        }
    }
    
    
    
    
    ```
    
  * Sobreescrita de métodos
    ```
    public class Filme {
        public void alugarFilme(int dias){
              if ((dias > 0) && (dias <= 5)){
                  System.out.println("Aluguel feito.");
              }else{
                  System.out.println("Não é possível alugar um filme por menos de 0 dias ou mais de 5 dias.");
              }
        }
    }
    
    
    
    public class Filme24Horas extends Filme {
 
        @Override
        public void alugarFilme(int dias) {
            if ((dias > 0) && (dias <=1)){
                System.out.println("Aluguel feito.");
            }else{
                System.out.println("Filme 24 horas deve ser alugado por no máximo 1 dia.");
            }
        }
    }
    ```
    
  * Polimorfismo
    ```
    interface GUIFactory
    public Menu createMenu();
    }

    class WinFactory implements GUIFactory {

    public Menu createMenu() {
    return new WinMenu();
    }
    }

    class LinuxFactory implements GUIFactory {
    public Menu createMenu() {
    return new LinuxMenu();
    }
    }
    
    
    
    interface Menu {
    public void paint();
    }

    class WinMenu implements Menu {
    public void paint() {
    System.out.println("Eu sou um WinMenu");
    }
    }

    class LinuxMenu implements Menu {
    public void paint() {
    System.out.println("Eu sou um LinuxMenu");
    }
    }
    
    
    
    class Aplicacao {
    public Aplicacao(GUIFactory factory) {
    Menu menu = factory.createMenu();
    menu.paint();
    }
    }

    class Principal {
    public static void main(String args[]) {
    chamar Application();
    //De preferencia leia de algum lugar e coloque a opção na variável
    int tipoDeMenu = 0;
    if (tipoDeMenu == 0)
    new Aplicacao(new WinFactory());
    else
    new Aplicacao(new LinuxFactory());
    }
    }
    ```
    
    * Conversão de tipos 
      ```
      class Test {			
          public static void main(String[] args) {
              // Casting conversion (5.4) of a float literal to
              // type int. Without the cast operator, this would
              // be a compile-time error, because this is a
              // narrowing conversion (5.1.3):
              int i = (int)12.5f;
              // String conversion (5.4) of i's int value:
              System.out.println("(int)12.5f==" + i);
              // Assignment conversion (5.2) of i's value to type
              // float. This is a widening conversion (5.1.2):
              float f = i;
              // String conversion of f's float value:
              System.out.println("after float widening: " + f);
              // Numeric promotion (5.6) of i's value to type
              // float. This is a binary numeric promotion.
              // After promotion, the operation is float*float:
              System.out.print(f);
              f = f * i;
              // Two string conversions of i and f:
              System.out.println("*" + i + "==" + f);
              // Method invocation conversion (5.3) of f's value
              // to type double, needed because the method Math.sin
              // accepts only a double argument:
              double d = Math.sin(f);
              // Two string conversions of f and d:
              System.out.println("Math.sin(" + f + ")==" + d);
          }
      }
      ```
      
* Classe abstrada
  * Definição
     * Representação de classe abstrata na UML
  * Criação de uma classe que extende uma classe abstrata
  * Polimorfismo
    * Conversão de tipos 
* Coleções 
  * Definição
  * List e Arraylist 
    * Aplicações
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
  * Map e HashMap
    * Aplicações 
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
* Tipo Enumerado
  *  Definição
     * Representação de tipos enumerados na UML
* Representação de tempo
  * Classe Date
  * Classe Calendar
  * API Date/Time Java 8
    * LocalDate
    * LocalTime
    * LocalDateTime
    * Period
    * Duration
    * Formação de Date/Time 
* Modificador final
  * Definição
    * Representação de final no diagrama UML 
  * Modificador final em uma variável
    * Variável  de tipo primitivo
    * Objeto 
  * Modificador final em um atributo
    * Atributo primitivo
    * Objeto 
  * Modificador final em um método
  * Modificador final em uma classe
* Objeto imutável
  * Definição
  * Aplicações
  * Como criar um objeto imutável
  * Como modificar um objeto imutável 
* Tipos Genéricos
  * Definição
     * Representação de tipos genéricos na UML
  * Criação de classes com tipos genéricos
  * Inicialização de objetos com tipos genéricos  
* Testes Unitários
  * TDD
  * JUnit
    * Adicionar JUnit no projeto Java
  * Teste assertEquals
  * Teste assertTrue/assertFalse
  * Teste assertNull/assertNull
  * Teste assertArrayEquals  
  * Teste fail
  * Teste capturar uma exception
* JDBC
  * Definição
  * Driver de conexão 
  * Como adicionar o driver de conexão no projeto Java
  * Criação de uma conexão com o banco de dados
    * Classe DataManager
    * String de conexão
      * Banco SQLite
      * Banco MySql
      * Banco Postgre 
    * Classe Connection
  * Enviar instruções SQL
    * Classe Statement
    * Classe PreparedStatment   
  * Consultar registros no banco de dados
    * Classe ResultSet
    * Obter um registro
    * Obter uma coleção de registros
  * Bloco de instruções try-with-resources
  * Captura de exceções
    * Driver não encontrado
    * Conexão inválida
    * Tabela não encontrada
    * Registro não encontrado
    * Erro ao inserir/atualizar
    * Erro ao consultar
  * Design Patterns
    * Singleton Factory para criação de conexões   
      * Representação na UML
    * DAO para manipular dados de uma tabela   
      * Representação na UML

## Listas de Exercícios

[SCHEIBEL, Glaucio. Exercícios de Programação](https://github.com/glaucioscheibel/exercicios)

[Beecrowd](https://www.beecrowd.com.br/judge/pt/)

[Leetcode](https://leetcode.com)

[HackerRank](https://www.hackerrank.com)

[Exercism](https://exercism.org/tracks/java)



## Referências Bibliográficas

FURGERI, SÉRGIO. Java 8 Ensino Didático: Desenvolvimento e Implementação de Aplicações. Saraiva Educação SA, 2018.

Schildt, Herbert. Java para iniciantes. Bookman Editora, 2015.

Finegan, Edward, and Robert Liguori. OCA Java SE 8: Guia de Estudos para o Exame 1Z0-808. Bookman Editora, 2018.

Bloch, Joshua. Java Efetivo: 3a edição. Alta Books Editora, 2019.

Martin, Robert C. Código limpo: habilidades práticas do Agile software. Alta Books, 2019.

Fowler, Martin. UML Essencial: um breve guia para linguagem padrão. Bookman editora, 2014.


https://github.com/geronimo-santos/hamburgueria/blob/main/index.html
