# Isaac.py
# Aqui eu faço título simples
print("=== Calculadora Simples ===")

# Pega o 1º número, float para uso de decimais
# Veja que eu dou um nome a ela "num1"
num1 = float(input("Digite o primeiro número: "))

# Pega a operação com cada sinal
operacao = input("Operação (+, -, *, /): ")

# Pega o 2º número ainda float
num2 = float(input("Digite o segundo número: "))

# Calcula baseado na operação (if/elif)
# Veja que eu começo pela adição, e de acordo com os elifs vou colocando os outros sinais, dps crio outro if e else onde evita uma divisão usando 0

if operacao == '+':
    resultado = num1 + num2
elif operacao == '-':
    resultado = num1 - num2
elif operacao == '*':
    resultado = num1 * num2
elif operacao == '/':
    if num2 != 0: 
        resultado = num1 / num2
    else:
        resultado = "Erro: Divisão por zero!"
else:
    resultado = "Operação inválida!"

# Mostra o resultado, Imprimindo ele!
print(f"Resultado: {resultado}")
input("Pressione Enter pra sair...")  
