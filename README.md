# EBAC-JOANA-AGHATA-GITHUB

Trabalho da aluna Joana Aghata do GitHub.
# CALCULADORA simples PYTHON


    #Função para realizar a operação
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

    #Solicita a entrada do usuário
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))
    op = input("Escolha a operação: +, -, *, /: ")
    #Realiza a operação e exibe o resultado
    resultado = calcular(num1, num2, op)
    print("Resultado: ", resultado)

# CALCULADORA simples BASH

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

# EXPLICAÇÃO codificação PYTHON

"""

Script de Calculadora Simples

Este script é uma calculadora simples que realiza operações matemáticas básicas (+, -, *, /) com dois números fornecidos pelo usuário.

Funções:
    - calcular: Realiza a operação matemática baseada na escolha do usuário.
    - input: Solicita a entrada dos números e da operação pelo usuário.
    - print: Exibe o resultado da operação ou uma mensagem de erro se a operação for inválida.
    
"""

    #Função para realizar a operação
    def calcular(num1, num2, op):

    """
    
    Realiza uma operação matemática entre dois números.

    Parâmetros:
    num1 (float): O primeiro número.
    num2 (float): O segundo número.
    op (str): A operação a ser realizada (+, -, *, /).

    Retorna:
    float ou str: O resultado da operação ou uma mensagem de erro se a operação for inválida.
    """
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

    #Solicita a entrada do usuário
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))
    op = input("Escolha a operação: +, -, *, /: ")

    #Realiza a operação e exibe o resultado
    resultado = calcular(num1, num2, op)
    print("Resultado: ", resultado)

Função calcular: realiza a operação matemática baseada nos parâmetros fornecidos (num1, num2, op). Verifica qual operação foi escolhida (+, -, *, /) e retorna o resultado correspondente. Se a operação for inválida, a função retorna uma mensagem de erro "Operação inválida".

Solicitação de Entradas: o script solicita ao usuário que insira dois números (num1 e num2) e escolha a operação (op).

Exibição do Resultado: o resultado da operação é calculado pela função calcular e exibido ao usuário.

"""
# EXPLICAÇÃO codificação BASH

    #!/bin/bash
    # Script de Calculadora Simples

    # Solicita a entrada do primeiro número
    echo "Digite o primeiro número:"
    read num1

    #Solicita a entrada do segundo número
    echo "Digite o segundo número:"
    read num2

    #Solicita a operação desejada
    echo "Escolha a operação: +, -, *, /"
    read op

    #Realiza a operação com base na escolha do usuário
    case $op in
      +) result=$((num1 + num2)) ;;  # Soma
      -) result=$((num1 - num2)) ;;  # Subtração
      \*) result=$((num1 * num2)) ;; # Multiplicação
      /) result=$((num1 / num2)) ;;  # Divisão
      *) echo "Operação inválida" ;; # Operação Inválida
    esac

    #Exibe o resultado da operação
    echo "Resultado: $result"

Solicitação de Entradas: o script solicita ao usuário que insira dois números (num1 e num2) e escolha a operação (op).

Estrutura de Condicional case: dependendo da operação escolhida, o script realiza a operação correspondente e armazena o resultado na variável result.

Soma: result=$((num1 + num2))

Subtração: result=$((num1 - num2))

Multiplicação: result=$((num1 * num2))

Divisão: result=$((num1 / num2))

Operação Inválida: exibe uma mensagem de erro "Operação inválida".

Exibição do Resultado: o resultado da operação é exibido ao usuário.
