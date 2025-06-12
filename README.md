# pythoniniciante
Apenas alguns projetos feito na linguagem de programação python fazendo pesquisas principalmente no chat gpt, porém sem ele dar o resultado final.

Calculadora Simples

while True:
    valor1 = float(input('Digite o Primeiro Valor: '))
    sinal = (input('Digite um sinal (+ - * /): '))
    valor2 = float(input('Digite o Segundo Valor: '))

    if sinal == "+":
        resultado = valor1 + valor2
    elif sinal == "-":
         resultado = valor1 - valor2
    elif sinal == "*":
         resultado = valor1 * valor2
    elif sinal == "/":
         if valor2 != 0:
              resultado = valor1 / valor2
         else:
          print("Erro: divisão por zero, tente novamente.")
          continue

    else:
         print("Operador inválido, tente novamente.")
         continue
    
    print("Resultado: ", resultado)

    continuar = input('Deseja fazer outro cálculo? (s/n): ').lower()
    if continuar == 'n':
         print('Encerrando, até!')
         break
