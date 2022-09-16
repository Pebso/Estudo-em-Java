# Estudo-em-Java
Estudos gerais em java. Orientação objeto, estruturas sequenciais e condicionais, etc... 



package atividades.em.java;


 
  @author pedro
 
import java.util.Scanner;
public class AtividadesEmJava {

    
           @param args the command line arguments
     
           public static void main(String[] args) {
        
                *******EXERCICIO*****
        Faça um programa que leia um número e informe se o mesmo é par ou ímpar.
        (aplicação de if e else)
        Scanner leia = new Scanner(System.in);
        double num1, num2;
      System.out.println("Entre com dois números");
        num1 = leia.nextDouble();
        num2 = leia.nextDouble();
        if(num1>num2){
            System.out.println("O maior é" + num1);
            System.out.println("O menor é" + num2);
        }
        else if (num2>num1){
            System.out.println("O maior é " +num2);
            System.out.println("O menor é " +num1);
        }
        else{
            System.out.println("Os numeros são iguals");
        }
        }
        }
  --
         **EXERCICIOS**
        DIFERENÇA ENTRE NUMEROS

        
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
--
        PROVAS APROVADO REPROVADO 3 VARIAVEIS
        
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
        Faça um programa que leia um número e informe se o mesmo é par ou ímpar.
        System.out.println("Digite um número: ");
        int numero = leia.nextInt();
        if(numero%2==0){
            System.out.println("O numero é par");
        }
        else{
            System.out.println("O numero é ímpar");
            }
    
--**EXERCICIO**
        Faça um programa que leia os três lados de um triângulo e imprima o tipo de triângulo:
Equilátero: os três lados são iguais
Isósceles: 2 lados são iguais
Qualquer: caso contrário.
--
        System.out.println("Digite os lados do triangulo: ");
        double l1,l2,l3;
        l1 = leia.nextDouble();
        l2 = leia.nextDouble();
        l3 = leia.nextDouble();
        if(l1==l2&&l2==l3){
            System.out.println("Equilátero");
        }
        else if(l1==l2||l1==l3||l2==l3){
            System.out.println("Isosceles");
        }
        else{
            System.out.println("Qualquer");
        }
      
     
        
--       **EXERCICIO**
        4. Construa um programa para determinar se o indivíduo está com um peso favorável. Essa situação é determinada através do IMC (Índice de Massa
Corpórea), que é definida como sendo a relação entre o peso (PESO – em kg) e o quadrado da Altura (ALTURA – em m) do indivíduo. Ou seja,
IMC= PESO/ALTURA2
--
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
        
        
        
 --        
        **EXERCICIO**
        Um determinado hotel cobra R$ 500,00 a diária e mais uma taxa de serviços. Faça um programa que leia o número de diárias e calcule o total a ser pago pelo cliente, sabendo-se que a taxa de serviços é de: 


        R$ 15,00 por dia, se número de diárias < 15 
        R$ 10,00 por dia, se número de diárias = 15 
        R$ 5,00 por dia, se número de diárias > 15
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
        
        
        
 -- 
 ***EXERCICIO***

 10. Uma academia de musculação possui a seguinte tabela para cobrança da mensalidade de seus clientes:

  **HOMENS:**
até 15 anos 60,00
16 a 18 anos 75,00
19 a 30 anos 90,00
31 a 40 anos 85,00
Acima de 40 anos 80,00.

**MULHERES**
até 18 anos 60,00
19 a 25 anos 90,00
26 a 40 anos 85,00
Acima de 40 anos 80,00.

***Faça um programa que leia a idade e sexo do cliente, e imprima o valor da mensalidade que o mesmo deve pagar.***
      
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
