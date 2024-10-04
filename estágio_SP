#1. Cálculo do valor da variável SOMA
INDICE = 13
SOMA = 0
K = 0

while K < INDICE:
    K = K + 1
    SOMA = SOMA + K

print(SOMA)

#2. Verificar se um número pertence à sequência de Fibonacci

def fibonacci(n):
    a, b = 0, 1
    fib_sequence = []
    while a <= n:
        fib_sequence.append(a)
        a, b = b, a + b
    return fib_sequence

def pertence_fibonacci(num):
    fib_seq = fibonacci(num)
    return num in fib_seq

# Entrada do usuário
numero = int(input("Informe um número: "))
if pertence_fibonacci(numero):
    print(f"O número {numero} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero} não pertence à sequência de Fibonacci.")

#3. Análise de faturamento diário

import json

# Exemplo de dados em JSON
dados_faturamento = '''
{
    "faturamento_diario": [10000, 15000, 0, 20000, 25000, 30000, 0, 40000, 50000, 45000, 60000, 0, 70000]
}
'''

dados = json.loads(dados_faturamento)
faturamento_diario = dados["faturamento_diario"]

# Remover dias sem faturamento
dias_com_faturamento = [valor for valor in faturamento_diario if valor > 0]

menor_faturamento = min(dias_com_faturamento)
maior_faturamento = max(dias_com_faturamento)
media_mensal = sum(dias_com_faturamento) / len(dias_com_faturamento)

dias_acima_da_media = sum(1 for valor in dias_com_faturamento if valor > media_mensal)

print(f'Menor faturamento: R$ {menor_faturamento:.2f}')
print(f'Maior faturamento: R$ {maior_faturamento:.2f}')
print(f'Dias acima da média: {dias_acima_da_media}')


#4. Cálculo do percentual de faturamento por estado

# Valores de faturamento
faturamento = {
    "SP": 67836.43,
    "RJ": 36678.66,
    "MG": 29229.88,
    "ES": 27165.48,
    "Outros": 19849.53
}

total_faturamento = sum(faturamento.values())

percentuais = {estado: (valor / total_faturamento) * 100 for estado, valor in faturamento.items()}

for estado, percentual in percentuais.items():
    print(f'Percentual de {estado}: {percentual:.2f}%')

#5. Inverter os caracteres de uma string

def inverter_string(s):
    string_invertida = ""
    for char in s:
        string_invertida = char + string_invertida
    return string_invertida

# Entrada do usuário
entrada = input("Informe uma string: ")
resultado = inverter_string(entrada)
print(f'String invertida: {resultado}')


