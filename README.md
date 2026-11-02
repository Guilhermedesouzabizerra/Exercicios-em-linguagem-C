# Exercicios-em-linguagem-C

1.

#include <stdio.h>



int main() {

  int numero;



  printf("Digite um numero inteiro: ");

  scanf("%d", &numero);



  printf("Numero digitado: %d\n", numero);



  if (numero % 2 == 0) {

    printf("O numero e par.\n");

  }



  if (numero % 2 != 0) {

    printf("O numero e impar.\n");

  }



  return 0;

}

2.



#include <stdio.h>



int main() {

  int numero;



  printf("Digite um numero inteiro: ");

  scanf("%d", &numero);



  printf("Numero digitado: %d\n", numero);



  if (numero >= 100 && numero <= 200) {

    printf("O numero esta entre 100 e 200.\n");

  } else {

    printf("O numero nao esta entre 100 e 200.\n");

  }



  return 0;

}



3.



#include <stdio.h>



int main() {

  float nota1, nota2, nota3, media;



  printf("Digite a primeira nota: ");

  scanf("%f", &nota1);



  printf("Digite a segunda nota: ");

  scanf("%f", &nota2);



  printf("Digite a terceira nota: ");

  scanf("%f", &nota3);



  media = (nota1 + nota2 + nota3) / 3;



  printf("Media do estudante: %.2f\n", media);



  if (media >= 6.0) {

    printf("Aluno aprovado.\n");

  } else if (media >= 4.0) {

    printf("Aluno de recuperacao.\n");

  } else {

    printf("Aluno reprovado.\n");

  }



  return 0;

}



questão 4



#include <stdio.h>



int main() {

  int opcao;



  printf("Digite um numero de 1 a 3: ");

  scanf("%d", &opcao);



  /*

    1 - Regiao Sul

    2 - Regiao Norte

    3 - Regiao Centro-Oeste

  */



  switch (opcao) {

    case 1:

      printf("Regiao Sul\n");

      break;



    case 2:

      printf("Regiao Norte\n");

      break;



    case 3:

      printf("Regiao Centro-Oeste\n");

      break;



    default:

      printf("Opcao invalida.\n");

  }



  return 0;

}


5.



#include <stdio.h>



int main() {

  char opcao;



  printf("Digite S, N ou C: ");

  scanf(" %c", &opcao);



  switch (opcao) {

    case 'S':

    case 's':

      printf("Regiao Sul\n");

      break;



    case 'N':

    case 'n':

      printf("Regiao Norte\n");

      break;



    case 'C':

    case 'c':

      printf("Regiao Centro-Oeste\n");

      break;



    default:

      printf("Opcao invalida.\n");

  }



  return 0;

}


6.



#include <stdio.h>



int main() {

  float temperatura;



  printf("Digite a temperatura do equipamento: ");

  scanf("%f", &temperatura);



  if (temperatura > 80) {

    printf("ALERTA: temperatura elevada!\n");

  }



  return 0;

}


7.



#include <stdio.h>



int main() {

  float valor, desconto, valorFinal;



  printf("Digite o valor da compra: R$ ");

  scanf("%f", &valor);



  valorFinal = valor;



  if (valor >= 200) {

    desconto = valor * 0.10;

    valorFinal = valor - desconto;



    printf("Cliente tem direito a 10%% de desconto.\n");

    printf("Desconto: R$ %.2f\n", desconto);

  } else {

    printf("Cliente nao tem direito ao desconto.\n");

  }



  printf("Valor final a pagar: R$ %.2f\n", valorFinal);



  return 0;

}


8.



#include <stdio.h>



int main() {

  int idade;



  printf("Digite a idade: ");

  scanf("%d", &idade);



  if (idade < 0) {

    printf("Idade invalida.\n");

  } else if (idade <= 11) {

    printf("Categoria: Crianca\n");

    printf("Ingresso: Gratuito\n");

  } else if (idade <= 17) {

    printf("Categoria: Adolescente\n");

    printf("Ingresso: R$ 15,00\n");

  } else if (idade <= 59) {

    printf("Categoria: Adulto\n");

    printf("Ingresso: R$ 30,00\n");

  } else {

    printf("Categoria: Idoso\n");

    printf("Ingresso: R$ 15,00\n");

  }



  return 0;

}


9.



#include <stdio.h>



int main() {

  float numero1, numero2, resultado;

  int operacao;



  printf("Digite o primeiro numero: ");

  scanf("%f", &numero1);



  printf("Digite o segundo numero: ");

  scanf("%f", &numero2);



  printf("\n1 - Soma\n");

  printf("2 - Subtracao\n");

  printf("3 - Multiplicacao\n");

  printf("4 - Divisao\n");



  printf("Escolha a operacao: ");

  scanf("%d", &operacao);



  switch (operacao) {

    case 1:

      resultado = numero1 + numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 2:

      resultado = numero1 - numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 3:

      resultado = numero1 * numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 4:

      if (numero2 == 0) {

        printf("A divisao por zero nao pode ser realizada.\n");

      } else {

        resultado = numero1 / numero2;

        printf("Resultado: %.2f\n", resultado);

      }

      break;



    default:

      printf("Operacao inexistente.\n");

  }



  return 0;

}


 10.



#include <stdio.h>



int main() {

  float numero1, numero2, resultado;

  char operacao;



  printf("Digite o primeiro numero: ");

  scanf("%f", &numero1);



  printf("Digite o segundo numero: ");

  scanf("%f", &numero2);



  printf("\nS - Soma\n");

  printf("U - Subtracao\n");

  printf("M - Multiplicacao\n");

  printf("D - Divisao\n");



  printf("Escolha a operacao: ");

  scanf(" %c", &operacao);



  switch (operacao) {

    case 'S':

    case 's':

      resultado = numero1 + numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 'U':

    case 'u':

      resultado = numero1 - numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 'M':

    case 'm':

      resultado = numero1 * numero2;

      printf("Resultado: %.2f\n", resultado);

      break;



    case 'D':

    case 'd':

      if (numero2 == 0) {

        printf("A divisao por zero nao pode ser realizada.\n");

      } else {

        resultado = numero1 / numero2;

        printf("Resultado: %.2f\n", resultado);

      }

      break;



    default:

      printf("Operacao inexistente.\n");

  }



  return 0;

}

