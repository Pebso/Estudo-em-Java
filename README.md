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

# EXEMPLO ESTRUTURA REPETIÇAO FOR

   public static void main(String[] args) {
       int vet [] = new int[5];
        Scanner leia = new Scanner(System.in);      
       int contador;      
     
       for(contador=0; contador<5; contador++){
       vet[contador] = contador;
       System.out.print("informe as notas: ");
       vet[contador] = leia.nextInt();
       }System.out.println("as notas informadas foram:");
       
       
       for(contador=0; contador<5; contador++){
         System.out.print(vet[contador] + ",");
