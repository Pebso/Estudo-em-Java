# Estudo-em-Java
Estudos gerais em java. Orientação objeto, estruturas sequenciais e condicionais, etc... 


**EXERCICIOS ESTRUTURA CONDICIONAL**


1.Faça um programa que receba as duas notas de um aluno, calcule sua média, e que imprima a sua situação: 
>= 7 -> Aprovado
< 7 -> Reprovado


     package aula;
     import java.util.Scanner;


     public class Aula {

  
     public static void main(String[] args) {
     Scanner leia= new Scanner(System.in);

     double nota1, nota2, media;
     System.out.println("informe a nota das duas provas: ");
     nota1 = leia.nextDouble();
     nota2 = leia.nextDouble();
     media = nota1+nota2/2;
     if (media>=7){
         System.out.println("APROVADO");
     }
     else{
         System.out.println("REPROVADO");
     }
     }
     }


2.Faça um programa que receba 3 notas de um aluno, calcule e mostre uma mensagem de acordo com sua média:

     package aula;
     import java.util.Scanner;


     public class Aula {

  
     public static void main(String[] args) {
     Scanner leia= new Scanner(System.in);

     double nota1, nota2, nota3, media;
        System.out.print("Informe a nota da primeira prova: ");
        nota1 = leia.nextDouble();
        System.out.print("Informe a nota da segunda prova: ");
        nota2 = leia.nextDouble();
        System.out.print("Informe a nota da terceira prova: ");
        nota3 = leia.nextDouble();
        media = nota1+nota2+nota3/3;
        if(media>=0 & media<3){
            System.out.println("REPROVADO");
        }
            else if(media<7){
                System.out.println("EXAME");
            }
            else{
                System.out.println("APROVADO");
     }
     }
     }


3.  Faça um programa para resolver equação de segundo grau (ax² + bx + c = 0).


     package estruturassequenciais;
     import java.util.Scanner;
     public class EstruturasSequenciais {

     /**
     * @param args the command line arguments
     */
     public static void main(String[] args) {
       
        Scanner leia = new Scanner(System.in);
        double A,B,C,DELTA,X1,X2;
       System.out.println("Informe o coeficiente A");
       A = leia.nextDouble();
       System.out.println("Informe o coeficiente B");
       B = leia.nextDouble();
       System.out.println("Informe o coeficiente C");
       C = leia.nextDouble();
       DELTA = ((B*B)-(4*A*C));
       if(DELTA >=0){
           X1 = ((-B + (Math.sqrt(DELTA))) / (2*A));
           X2 = ((-B - (Math.sqrt(DELTA))) / (2*A));
           System.out.println("As raizes são" + X1+ "e" +X2);
       }
       else{
           System.out.println("Não existem raizes reais");
       }
           
       
           
       
       }

4.4. Construa um programa para determinar se o indivíduo está com um peso favorável. Essa situação é determinada através do IMC (Índice de Massa
Corpórea), que é definida como sendo a relação entre o peso (PESO – em kg) e o quadrado da Altura (ALTURA – em m) do indivíduo. Ou seja,
IMC= PESO/ALTURA2

     package estruturassequenciais;
     import java.util.Scanner;
     public class EstruturasSequenciais {

     /**
     * @param args the command line arguments
     */
     public static void main(String[] args) {
       
        Scanner leia = new Scanner(System.in);

        double peso, altura, imc, altura2;

        System.out.println("Digite seu peso em kg: ");
        peso = leia.nextDouble();
        System.out.println("Digite sua altura em m: ");
        altura = leia.nextDouble();
        altura2 = altura * altura;
        imc = peso / altura2;
        System.out.println("Seu IMC é de: " + imc);
        if (imc < 20) {
            System.out.println("Abaixo do peso");
        } else if (imc > 20 && imc <= 25) {
            System.out.println("Peso Normal");
        } else if (imc > 25 && imc <= 30) {
            System.out.println("Sobre Peso");
        } else if (imc > 30 && imc <= 40) {
            System.out.println("Obeso");
        } else {
            System.out.println("Obeso Morbido");
     }
     }
     }

5.(SEM FAZER)



6. (SEM FAZER)

7.(SEM FAZER)

8.(SEM FAZER)

9.Um determinado hotel cobra R$ 500,00 a diária e mais uma taxa de serviços. Faça um programa que leia o número de diárias e calcule o total a ser pago pelo cliente, sabendo-se que a taxa de serviços é de: 
R$ 15,00 por dia, se número de diárias < 15 
R$ 10,00 por dia, se número de diárias = 15 
R$ 5,00 por dia, se número de diárias > 15

     package estruturassequenciais;
     import java.util.Scanner;
     public class EstruturasSequenciais {

     /**
      * @param args the command line arguments
      */
     public static void main(String[] args) {
     Scanner leia = new Scanner(System.in);
        int diaria, dias, tax, tax2, tax3, dia2, dia3;
        
        System.out.println("Quantos dias pretende ficar? ");
        dias = leia.nextInt(); 
        tax = dias *15;
        tax2 = dias*10;
        tax3 = dias*5;
        diaria = dias*500+tax;
        dia2 = dias*500+tax2;
        dia3 = dias*500+tax3;
        if (dias>0 & dias <15){
            System.out.println("A estadia é de R$ " + diaria);
        }          
        else if(dias==15){
            System.out.println("A estadia é de R$ " + dia2);
            
        }
        else if(dias>15){
            System.out.println("A estadia é de R$ " + dia3);
            
        }
        else{
            
        }
        }
        }


10.Uma academia de musculação possui a seguinte tabela para cobrança da mensalidade de seus clientes:
HOMENS: até 15 anos 60,00 16 a 18 anos 75,00 19 a 30 anos 90,00 31 a 40 anos 85,00 Acima de 40 anos 80,00.
MULHERES até 18 anos 60,00 19 a 25 anos 90,00 26 a 40 anos 85,00 Acima de 40 anos 80,00.
Faça um programa que leia a idade e sexo do cliente, e imprima o valor da mensalidade que o mesmo deve pagar.



     package javaapplication11;
     import java.util.Scanner;
     /**
      *
     * @author aluno
       */
     public class JavaApplication11 {

      /**
     * @param args the command line arguments
     */
      public static void main(String[] args) {
     Scanner leia = new Scanner(System.in);
     int idade;
     String sexo;
     System.out.println("idade");
     idade= leia.nextInt();
     System.out.println("Sexo f/m");
     sexo = leia.next();
     if(idade<=15&&(sexo.equals("m")||sexo.equals("M"))){
         System.out.print("Mensalidade de R$60,00");
        
     }
     else
         if(idade<=18&&(sexo.equals("f")||sexo.equals("F"))){
             System.out.print("Mensalidade de R$60,00");
         }
     else
             if(idade==16 || idade<=18&&(sexo.equals("m")||sexo.equals("M"))){
                 System.out.println("Mensalidade de R$75,00");
             }
     else
                 if(idade==19||idade<=25&&(sexo.equals("f")||sexo.equals("F"))){
                     System.out.println("Mensalidade de R$90,00");
                 }
     else
                     if(idade==19||idade<=30&&(sexo.equals("m")||sexo.equals("M"))){
                         System.out.println("Mensalidade de R$90,00");
                     }
     else
                         if(idade==26||idade<=40&&(sexo.equals("f")||sexo.equals("F"))){
                             System.out.println("Mensalidade de R$85,00");
                         }
     else
                             if(idade==31||idade<=40&&(sexo.equals("m")||sexo.equals("M"))){
                                 System.out.println("Mensalidade de R$85,00");
                             }
                             else{
                                 System.out.println("Mensalidade de R$ 80,00");
                             }
         }
    
     }

11.  Um hotel possui a seguinte tabela para cobrança da diária de seus clientes: Apto Simples Número de diárias < 10 100,00 Número de diárias entre 10 e 15 90,00 Número de diárias > 15 80,00
Apto Duplo Número de diárias < 10 140,00 Número de diárias entre 10 e 15 120,00 Número de diárias > 15 100,00
Faça um programa que leia a tipo de apartamento e a quantidade de dias em que um hóspede esteve no hotel, e calcule o total a ser pago pelo mesmo.





         package javaapplication11;
         import java.util.Scanner;
         /**
         *
           * @author aluno
           */
         public class JavaApplication11 {

         /**
          * @param args the command line arguments
         */
          public static void main(String[] args) {
          int dias,simples100,simples90,simples80,duplo140,duplo120,duplo100;
          double estadia100, estadia140;     
          String simples, duplo;     
          Scanner leia = new Scanner(System.in);
          System.out.println("Selecione: apto simples ou duplo:");
          System.out.println("Simples? S/N");
          simples = leia.next();
          System.out.println("Duplo? S/N");
          duplo = leia.next();
          System.out.println("Quantos dias o hospede ficou?");
          dias = leia.nextInt();
          simples100 = dias *100;
          simples90 = dias *90;
          simples80 = dias *80;
          duplo140 = dias *140;
          duplo120 = dias *120;
          duplo100 = dias *100;

          if(dias<10&&(simples.equals("s")||simples.equals("S"))){
          System.out.println("Diarias no valor de " + simples100);
    
          }
          else 
          if(dias==10||dias<=15&&(simples.equals("s")||simples.equals("S"))){
             System.out.println("Diarias no valor de " +simples90);
          }
          else
             if(dias>15&&(simples.equals("s")||simples.equals("S"))){
                 System.out.println("Diarias no valor de " +simples80);
          }
          else
                 if(dias<10&&(duplo.equals("s")||duplo.equals("S"))){
           System.out.println("Diarias no valor de " +duplo140);
           }
           else
                     if(dias==10||dias<=15&&(duplo.equals("s")||duplo.equals("S"))){
                         System.out.println("Diarias no valor de " +duplo120);
                }
            else
                         if(dias>15&&(duplo.equals("s")||duplo.equals("S"))){
                             System.out.println("Diarias no valor de " +duplo100);
                    }
                    else{
                        
                    }
                        

             }
             }
            # Estrutura Sequencial

    1 Leia três números inteiros e imprima a média aritmética entre esses números.
       int A, B, C, ABC, med;
       
           new Scanner(System.in).nextLine();
           A = Integer.parseInt(new Scanner(System.in).nextLine());
           B = Integer.parseInt(new Scanner(System.in).nextLine());
           C = Integer.parseInt(new Scanner(System.in).nextLine());
           ABC = 3;
           med = (A + B + C) / ABC;
           System.out.println("MEDIA =" + med);

    2 Faça um programa que receba o ano de nascimento de uma pessoa, o ano atual e imprima:
        1. A idade da pessoa no ano atual
        2. A idade que a pessoa terá em 2050
        
           int ano, anoatual, idade, id, veio;
           new Scanner(System.in).nextLine();
           System.out.println("digite o seu ano de nascimento");
           ano = Integer.parseInt(new Scanner(System.in).nextLine());
           System.out.println("digite o ano atual");
           anoatual = Integer.parseInt(new Scanner(System.in).nextLine());
           idade = anoatual - ano;
           veio = 2050;
           id = veio - ano;
           System.out.println("sua idade é " + idade);
           System.out.println("sua idade em 2050 será " + id);

    3 Faça um programa que receba a cotação do dólar em reais, e um valor que o usuário possui em dólares. Imprima este valor em reais.
       
           import java.util.Scanner;
           public class Main
           {
	    public static void main(String[] args) {
		System.out.println("Conversor Dolar/Real");
		// variaveis
           double real, dolar, convert;

           Scanner leia = new Scanner(System.in);

           real = 5.18;

           System.out.println("Digite quanto possui em dólar");
           dolar = leia.nextDouble();
           convert = dolar*real;
           System.out.println("Convertendo seu Dolar em Real, você tem" + convert );

		
           	}
           }

    4  Faça um programa que calcule e mostre a área de um losango AREA = (DIAGONAL MAIOR * DIAGONAL MENOR)/2

            import java.util.Scanner;
            public class Main
            {
	    public static void main(String[] args) {
		System.out.println("Meça a area de um losango");
		
            double area, diagmaior, diagmenor;
            Scanner leia = new Scanner(System.in);
            System.out.println("Tamanho da diagonal maior");
            diagmaior = leia.nextDouble();
                      System.out.println("Tamanho da diagonal menor");
                      diagmenor = leia.nextDouble();
            area = diagmaior * diagmenor/ 2;
            System.out.println("A area total é de " + area );
           	}
            }
    5 Faça um programa que receba uma temperatura em Celsius, calcule e mostre essa temperatura em Fahrenheit (F = (C*1,8) + 32)
package estruturassequenciais;


           import java.util.Scanner;
           public class EstruturasSequenciais {

               /**
                * @param args the command line arguments
                */
               public static void main(String[] args) {
       
                   Scanner leia = new Scanner(System.in);
                  double C, Faren;
                  System.out.println("Qual a temperatura em Celsius?");
                  C = leia.nextDouble();
                  Faren = (C*1.8) +32;
                  System.out.println("Convertendo Cº em Fº ficariam: " + Faren);
               }
    
           }


    6 Faça um programa que solicite ao usuário que informe os coeficientes a, b e c de uma equação de segundo grau, e que imprima as raízes desta equação (considere que os valores informados sempre retornarão raízes reais para a equação).
    
    
           package estruturassequenciais;
           import java.util.Scanner;
           public class EstruturasSequenciais {

                                                /**
                                      * @param args the command line arguments
                           */
               public static void main(String[] args) {
       
                  Scanner leia = new Scanner(System.in);
                   double A,B,C,DELTA,X1,X2;
                  System.out.println("Informe o coeficiente A");
                  A = leia.nextDouble();
                  System.out.println("Informe o coeficiente B");
                  B = leia.nextDouble();
                  System.out.println("Informe o coeficiente C");
                  C = leia.nextDouble();
                  DELTA = ((B*B)-(4*A*C));
                  if(DELTA >=0){
                      X1 = ((-B + (Math.sqrt(DELTA))) / (2*A));
                      X2 = ((-B - (Math.sqrt(DELTA))) / (2*A));
                      System.out.println("As raizes são" + X1+ "e" +X2);
                  }
                  else{
                      System.out.println("Não existem raizes reais");
                  }
           
       
           
       
                          }
    
                                 }




   
                       

# EXEMPLO ESTRUTURA REPETIÇAO FOR

        public static void main(String[] args) {
       
        Scanner leia = new Scanner(System.in);  
        int vet [] = new int[5];
        double notas;
        int i;      
        // pra ler sempre vai ser de 0 ate o tamanho do vetor, e o ++ eu uso para incrementar.
        // leitura de dados:
        for(i=0; i< vet.length; i++){
        vet[i] = i;
        System.out.print("informe as notas: ");
        vet[i] = leia.nextInt();
       
       
       
       
        }System.out.println("as notas informadas foram:");
        // saida de dados:
        // pra eu ter um espaço entre cada inf do vetor uso o "  "
        // o legth vai preencher ate o tamanho do meu vetor, podendo assim eu alterar o tamanho do vetor sem ter que trabalhar toda a estrutura de codigo
        for(i=0; i<vet.length; i++){
           
         System.out.println(vet[i]+ " ");
          
         }


# Treinando um pouco de repetição simples for, com multiplicação de vetores 

         import java.util.Scanner;
         public class Main
         {
	 public static void main(String[] args) {
	 Scanner	input = new Scanner(System.in);
		int vet[] = new int[1];
		int vet2[] = new int[1];
		int vet3[] = new int[1];
		
		int i;
		for (i =0; i<vet.length; i++){
		    vet[i] = i;
		    System.out.println("informe o primeiro numero");
		    vet[i] = input.nextInt();
		    
		}for (i =0; i<vet.length; i++){
		    vet2[i]=i;
		    System.out.println("informe um segundo numero");
		    vet2[i] = input.nextInt();
		}for (i =0; i<vet.length;i++){
		    vet3[i]= vet[i] * vet2[i];
		    System.out.println("a multiplicação dos numeros informados é  " + vet3[i] + " ");
		}
		
		
	  }
          }

