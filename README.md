# EBAC-JOANA-AGHATA-GITHUB

Trabalho da aluna Joana Aghata do GitHub.
#CALCULADORA PYTHON
# Script de calculadora simples em Python

# Função para realizar a operação
def calcular(num1, num2, op):
    if op == '+':
        return num1 + num2
    elif op == '-':
        return num1 - num2
    elif op == '*':
        return num1 * num2
    elif op == '/':
        return num1 / num2
    else:
        return "Operação inválida"

# Solicita a entrada do usuário
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
op = input("Escolha a operação: +, -, *, /: ")

# Realiza a operação e exibe o resultado
resultado = calcular(num1, num2, op)
print("Resultado: ", resultado)

#CALCULADORA BASH

#!/bin/bash
echo "Digite o primeiro nÃºmero:"
read num1
echo "Digite o segundo nÃºmero:"
read num2
echo "Escolha a operaÃ§Ã£o: +, -, *, /"
read op

case $op in
  +) result=$((num1 + num2)) ;;
  -) result=$((num1 - num2)) ;;
  \*) result=$((num1 * num2)) ;;
  /) result=$((num1 / num2)) ;;
  *) echo "OperaÃ§Ã£o invÃ¡lida" ;;
esac

echo "Resultado: $result"
