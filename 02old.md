# Hello World

## Estrutura mínima de um código Java

```java
public class Main{

   public static void main(String args[]){
      System.out.println("Hello World");
   }

}
```

## Nome do arquivo e Extensão

O arquivo com código java deve ter o nome com a inicial em maiúscula. Por exemplo ```Main.java```.
A extensão de um arquivo com código Java deve ser sempre ```.java```.

## Nome da classe

Uma classe java deve ser nomeada com o mesmo nome do arquivo. 
Por exemplo se o arquivo se chama ```Main.java```,  a classe pública dentre deste arquivo deve se chamar ```Main```.
Caso o nome da classe e do arquivo forem diferentes, um erro de execução/compilação será gerado.

Os nomes das classes Java segue o padrão **camelCase**. Por exemplo: Pessoa, Endereco, ArrayList, ItemDaNotaFiscal.

## Método main

O método ```public static void main(String args[])``` é definido como o ponto inicial de execução de um programa Java. O método deve ter exatamente esta assinatura. Qualquer alteração, o método não será reconhecido como o ponto inicial de execução do programa.

## Escrever dados no console

Um programa Java pode utilizar o console para exibir informações ao usuário. Para este fim, o método [```System.out.println```](https://docs.oracle.com/en/java/javase/18/docs/api/java.base/java/lang/System.html#out) pode ser utilizado. O método recebe por parâmetro uma String a ser exibida no console.

## Indentação de código

A indentação de código é a prática de adicionar espaços extras nos blocos de códigos. Esta prática visa aumentar a legibilidade do código e identificar os blocos de instruções. Um nível de indentação pode ser feito com 4 caracteres de espaços ou uma tabulação. Exemplo:

```java
public static void main(String args[]){
   // este comentário e o println estão dentro do bloco do método.
   // Por isso contém uma indentação em relação a definição do método
   System.out.println("Hello World");
}
```


## Delimitação de uma instrução

Uma instrução típicamente ocupa uma linha do arquivo, sendo finalizado pelo caracter ```;``` (ponto e vírgula). Na linguagem Java, todas as instruções obrigatoriamente devem ser finalizadas pelo ```;```. Caso a instrução não for finalizada, um erro de compilação irá ser gerado. Exemplo:

```java
System.out.println("Hello World");
```

## Delimitação de bloco de instruções

Os blocos de instruções são delimitados pelos caracteres ```{``` e ```}```. Todos os blocos abertos devem ser fechados.  Caso um bloco de instrução não for fechado, um erro de compilação irá ser gerado. Exemplo:

```java 
public class Main{  // abre o bloco de instruções da classe Main

   public static void main(String args[]){  // abre o bloco de instruções do método main
      System.out.println("Hello World");
   }  // finaliza o bloco de instruções do método main

} // finaliza o bloco de instruções da classe Main
```

## Comentários

Comentários são trechos de textos que são ignorados pelo compilador. Pode ser utilizado pelo programador para apresentar informações extras sobre o trecho de código.
Exemplo:


```java 
public class Main{  

   // Comentário de uma linha
   
   /**
     Comentário 
     de 
     múltiplas linhas
   **/

} 
```



## Compilação e Execução via linha de comando

Um código java é compilado através do aplicativo ```javac``` fornecido pela JDK.
Para compilar um código java, deve-se utilizar o terminal no mesmo diretório do código fonte. O nome do arquivo java a ser compilado deve ser passado para o programa Javac.

```bash
javac Main.java
```

Se a compilação for um sucesso, nenhuma mensagem será apresentada no console e um arquivo com o mesmo nome e com a extensão ```.class``` será gerado no diretório.. Caso contrário, o java irá informar erro de compilação e o problema encontrado.

Para executar o programa Java, deve ser executado o comando ```java``` e informar o arquivo que deseja executar. Exemplo:

```bash
java Main
```

Se tudo estiver correto, o programa será executado.



