# 🧮 Calculadora de IMC em C

Programa desenvolvido em C para calcular o Índice de Massa Corporal (IMC) com base na altura e peso informados pelo usuário.

---

## 💻 Como funciona

O usuário informa:
- Altura
- Peso

O programa calcula o IMC e retorna a classificação:

- Abaixo do peso
- Peso normal
- Acima do peso
- Obesidade

---

## 🧠 Conceitos utilizados

- Variáveis
- Entrada e saída de dados (scanf / printf)
- Operadores matemáticos
- Estruturas condicionais (if)

---

## 🚀 Como executar

Compile o código:

#include <stdio.h>

int main () {


    float altura;
    float peso;
    float imc;

    printf("Digite sua altura\n");
    scanf(" %f", &altura);

    printf("Digite seu peso\n");
    scanf(" %f", &peso);

    imc = peso / (altura * altura);

    if ( imc < 18.5){
    printf("Voce esta abaixo do peso!\n");
    }
    if ( imc >= 18.5 && imc < 25){
    printf("Voce esta com o peso normal!\n");
    }
    if ( imc >= 25 && imc < 30){
    printf("Voce esta acima do peso!\n");
    }
    if ( imc >= 30){
    printf("Voce esta obeso!");
    }
    return 0;

}
