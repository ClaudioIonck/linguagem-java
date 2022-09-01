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
       public class MyClass{
       public  void meuMetodo(/*argumentos*/){
       }
       }
       
      - Main:
       public class MyClass{
       public static void main(String[] args){
       }
       }
       
  * Estilo de código
      - Chamada de metodo:
       someMethod(longExpression1, longExpression2, longExpression3,
        longExpression4, longExpression5);

       var = someMethod1(longExpression1,
                       someMethod2(longExpression2,
                               longExpression3));
                               
      - Metodos aritmeticos:
       longName1 = longName2 * (longName3 + longName4 - longName5)
           + 4 * longname6; // PREFER

       longName1 = longName2 * (longName3 + longName4
                              - longName5) + 4 * longname6; // AVOID
                              
      - Netodos ternarios:
       alpha = (aLongBooleanExpression) ? beta : gamma;

       alpha = (aLongBooleanExpression) ? beta
           : gamma;

       alpha = (aLongBooleanExpression)
           ? beta
           : gamma;
           
      - Comentarios:
       /*
       *Aqui está um bloco de comentário...
       */
       
      - Declarações:
       int level; // indentation level
       int size;  // size of table
       
      - Classes e interfaces:
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
       
  * Versões
    * Java 1.8
      Funcionalidades do Java 8:
           Aqui há um breve resumo das melhorias incluídas na release 8 do Java:
           Métodos de Expressão Lambda e Extensão Virtual
           O destaque do Java SE 8 é a implementação de expressões Lambda e funcionalidades de suporte para a linguagem de programação e plataforma Java.
           API de Data e Hora
           Essa nova API permitirá que os desenvolvedores tratem data e hora de maneira mais natural, clara e fácil de entender.
           Nashhorn JavaScript Engine
           Uma nova implementação leve de alto desempenho do motor JavaScript foi integrada ao JDk e está disponível para aplicações Java por meio das APIs existentes.
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

          JEP 400: UTF-8 por padrão – Define UTF-8 como o conjunto de caracteres padrão das APIs Java padrão. Com essa alteração, as APIs que dependem do conjunto de  caracteres padrão se comportarão de forma consistente em todas as implementações, sistemas operacionais, localidades e configurações.
          JEP 408: Simple Web Server – Uma ferramenta de linha de comando e API para iniciar um servidor web mínimo que serve apenas arquivos estáticos. Esta ferramenta será útil para prototipagem, codificação ad-hoc e propósitos de teste, particularmente em contextos educacionais.
          JEP 416: Reimplementar Core Reflection com Method Handles – Reimplementa java.lang.reflect.Method, Constructor e Field sobre os handles de método java.lang.invoke. Ao tornar o método manipula o mecanismo subjacente para reflexão, ele reduz o custo de manutenção e desenvolvimento das APIs java.lang.reflect e java.lang.invoke.
          JEP 418: Resolução de endereço de Internet SPI – Define uma interface de provedor de serviço (SPI) para resolução de nome e endereço de host, para que java.net.InetAddress possa usar resolvedores diferentes do resolvedor integrado da plataforma.

          Ferramentas

          JEP 413: Trechos de código JEP na documentação da API Java – Introduz a tag @snippet para o Doclet padrão do JavaDoc para simplificar a inclusão de código-fonte de exemplo na documentação da API.

          Visualização e incubadoras para versões posteriores do JDK

          JEP 417: Vector API (Terceira Incubadora) – Fornece uma API para desenvolvedores alavancarem de forma confiável arquiteturas de CPU que fornecem extensões vetoriais escaláveis. Isso levará a um desempenho superior em comparação com cálculos equivalentes em processadores não estendidos.
          JEP 419: Função Estrangeira e API de Memória (Segunda Incubadora) – Permite que programas Java interoperem com código e dados fora do tempo de execução Java. Ao invocar eficientemente funções externas (ou seja, código fora da JVM) e ao acessar com segurança a memória externa (ou seja, memória não gerenciada pela JVM), a API permite que programas Java chamem bibliotecas nativas e processem dados nativos sem a fragilidade e as armadilhas de JNI.
          JEP 420: Correspondência de padrões para switch (segunda visualização) – Aprimora a linguagem de programação Java com correspondência de padrões para expressões e instruções de switch, juntamente com extensões para a linguagem de padrões. Estender a correspondência de padrões para switch permite que uma expressão seja testada em vários padrões, cada um com uma ação específica, para que consultas complexas orientadas a dados possam ser expressas de forma concisa e segura.

          Programas Java à prova de futuro

          JEP 421: Finalização obsoleta para remoção – A finalização permanece habilitada por padrão por enquanto, mas pode ser desabilitada para facilitar o teste. Em uma versão futura, ela será desabilitada por padrão e, em uma versão posterior, será removida. Os mantenedores de bibliotecas e aplicativos que dependem da finalização devem considerar a migração para outras técnicas de gerenciamento de recursos, como a instrução try-with-resources e limpadores .

          Suporte a clientes Java

          O Oracle Java SE Subscription é uma oferta previsível de pagamento conforme o uso, oferece aos clientes o melhor suporte da categoria, direito ao GraalVM Enterprise, acesso ao Java Management Service e flexibilidade para atualizar no ritmo de seus negócios. Isso ajuda as organizações de TI a gerenciar a complexidade, conter custos e mitigar os riscos de segurança.
          
    * Java 19 
      Funcionalidades do Java 19:
          
      Uma prévia dos genéricos universais, da Valhalla. Entregues por meio de três JEPs, os genéricos universais unificariam o tratamento de tipos de referência e primitivos no código genérico, permitindo que as variáveis ​​de tipo Java abrangessem os dois tipos de tipos.Uma visualização de objetos de valor, também um aprimoramento do Valhalla, fornecendo 
      instâncias de classe que possuem apenas campos de instância final e não possuem identidade de objeto. Classes de valor sem identidade seriam declaradas.
      Uma visualização de padrões de registro, para desconstruir valores de registro. Isso faz parte do Projeto Amber.
      Fixação de região para o coletor de lixo G1, para reduzir a latência implementando a fixação de região para G1 para que a coleta de lixo não precise ser desabilitada durante regiões 
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

      strictfp: usado em frente a um método ou classe para indicar que os números de ponto flutuante seguirão as regras de ponto flutuante em todas as expressões

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
        
      - Criando um projeto: https://www.alura.com.br/conteudo/intellij-idea-truques-para-aumentar-sua-produtividade-em-projetos-java?gclid=CjwKCAjwsMGYBhAEEiwAGUXJae_4Anz228D8giU5A9ycNmlfFKhayDRzH117ct6ODugObtKQKieMWxoCXbcQAvD_BwE
        
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
  * Nome do arquivo e Extensão
  * Nome da classe
  * Método main
  * Escrever dados no console
  * Indentação de código
  * Delimitação de uma instrução
  * Delimitação de bloco de instruções
  * Compilação e Execução via linha de comando
* [Tipos de Dados e operadores](03.md)
  * Tipos de Dados
  * Declarações de variáveis
  * Nomes válidos para variáveis e boas práticas 
  * Atribuição de valores
  * Operadores
    * Operadores aritméticos
    * Operadores booleanos
  * Conversão de tipos de dados
* [Saída de Dados](04.md)
  * Método System.out.println
  * Método System.out.print
  * Exibir o valor de uma variável
  * Exibir o valor de um decimal  
* Classe Math
  * Definição
  * Principais operações 
* String
  * Concatenação de String
  * Principais operações sobre String
  * Comparação de String
  * Diferença entre String e caracter
* Entrada de Dados
  * Classe Scanner
    * Obter um valor inteiro
    * Obter um valor decimal
    * Obter um valor de texto 
* Fluxo de Controle
  * Estruturas de Decisões
    * if-else-then
    * switch
  * Estruturas de Repetições
    * for
    * while
    * do-while 
    * Comandos break e continue
* Arranjos e Matrizes
  * Definição matemática
  * Declaração de arranjos
  * Declaração de matrizes
  * Percorrer arranjos
  * Percorrer matrizes
    * Linha a linha
    * Coluna a coluna
    * Em diagonal 
  * Utilizar arranjos e matrizes como parâmetros de métodos 
  * Utilizar arranjos e matrizes como retorno de métodos 
* Tratamento de Exceções
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
* Métodos estáticos
  * Estrutura de declaração de um método estático
  * Nomes válidos e boas práticas 
  * Parâmetros 
  * Retorno
  * Utilização de métodos estáticos 
    * Disponíveis na mesma classe
    * Disponíveis em outra classe/arquivo. 
  * Recursão 
* Classe
  * Definição
    * Representação de classe e objeto na UML
    * Diferença entre classe e objeto
  * Atributos
  * Métodos
  * Construtor 
  * Objeto
  * Inicialização de um objeto 
  * Utilização de um objeto
  * Comparação de objetos
  * Método toString
  * Visibilidade de atributos e métodos
    * Público
    * Privado 
  * Sobrecarga de métodos
  * Sobrecarga de construtores
* Pacotes 
  * Definição
     * Representação de pacotes na UML
  * Definição de um pacote em uma classe
  * Importando uma classe de um pacote diferente
  * Visibilidade de classes, atributos e métodos
     * Default/Pacote  
  * Pacote default
    * Importar uma classe em um pacote default 
* Escopo de classe e objeto
  * Definição 
  * Palavra reservada static 
* Herança
  * Definição
     * Representação de herança na UML
  * Criação de uma classe que realiza herança 
  * Sobreescrita de métodos
  * Polimorfismo
    * Conversão de tipos 
  * Visibilidade de atributos e métodos
     * Protegido
  * Palavra reservada super 
     * Encadeamento de construtor 
     * Encadeamento de método
* Interface
  * Definição
     * Representação de interface na UML
  * Criação de uma classe que implementa uma interface
  * Sobreescrita de métodos
  * Polimorfismo
    * Conversão de tipos 
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
