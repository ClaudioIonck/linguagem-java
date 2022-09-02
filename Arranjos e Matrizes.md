* [Arranjos e Matrizes](Arranjos e Matrizes.md)
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
