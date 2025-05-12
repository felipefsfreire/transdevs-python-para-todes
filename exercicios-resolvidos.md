# Exercícios Resolvidos - Python Básico

## Introdução e Olá Mundo

### Exercício 1: Escreva um programa que mostre "Olá, mundo!" na tela.
```py
print("Olá, mundo!")  # Saída simples usando a função print()
```

## Variáveis, Operações, Funções

### Exercício 2: Peça ao usuário que digite o nome e mostre uma mensagem de boas-vindas.
```py
nome = input("Digite seu nome: ")
print(f"Bem-vindo(a), {nome}!")
```

### Exercício 3: Solicite dois números e exiba a soma.
```py
a = int(input("Digite o primeiro número: "))
b = int(input("Digite o segundo número: "))
print("A soma é:", a + b)
```

### Exercício 4: Calcule a média entre 4 notas.
```py
notas = []
for i in range(4):
    nota = float(input(f"Digite a nota {i+1}: "))
    notas.append(nota)
media = sum(notas) / len(notas)
print(f"Média final: {media:.2f}")
```

### Exercício 5: Converta Celsius para Fahrenheit.
```py
celsius = float(input("Informe a temperatura em Celsius: "))
fahrenheit = celsius * 9/5 + 32
print(f"{celsius}C é igual a {fahrenheit}F")
```
### Exercício 6: Verifique se um número é par ou ímpar.

```py
n = int(input("Digite um número: "))
if n % 2 == 0:
    print("O número é par.")
else:
    print("O número é ímpar.")
```

## Listas, Tuplas, Dicionários

### Exercício 7: Armazene 5 nomes em uma lista e imprima-os em ordem.
```py
nomes = []
for i in range(5):
    nomes.append(input("Digite um nome: "))
nomes.sort()
print("Nomes em ordem alfabética:", nomes)
```

### Exercício 8: Crie uma tupla com os dias da semana e mostre o último.
```py
dias = ("Segunda", "Terça", "Quarta", "Quinta", "Sexta", "Sábado", "Domingo")
print("O último dia é:", dias[-1])
```

### Exercício 9: Dicionário com nome e idade.
```py
pessoa = {"nome": "Ana", "idade": 25}
print(f"{pessoa['nome']} tem {pessoa['idade']} anos.")
```

### Exercício 10: Lista de números e soma dos pares.
```py
numeros = [1, 2, 3, 4, 5, 6]
soma_pares = sum(n for n in numeros if n % 2 == 0)
print("Soma dos pares:", soma_pares)
```

## Condicionais e Loops

### Exercício 11: Verificar maior de idade.
```py
idade = int(input("Qual sua idade? "))
if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

### Exercício 12: Tabuada de um número
```py
n = int(input("Digite um número: "))
for i in range(1, 11):
    print(f"{n} x {i} = {n*i}")
```

### Exercício 13: Adivinhe o número
```py
import random
secreto = random.randint(1, 10)
chute = int(input("Adivinhe o número de 1 a 10: "))
if chute == secreto:
    print("Acertou!")
else:
    print(f"Errou! O certo era {secreto}.")
```

### Exercício 14: Contagem regressiva de 10 a 0
```py
for i in range(10, -1, -1):
    print(i)
```

### Exercício 15: Somar até digitar 0
```py
soma = 0
while True:
    n = int(input("Digite um número (0 para sair): "))
    if n == 0:
        break
    soma += n
print("Soma total:", soma)
```

## Funções

### Exercício 16: Função que retorna o quadrado de um número
```py
def quadrado(n):
    return n ** 2
print(quadrado(5))  # Saída: 25
```

### Exercício 17: Função que recebe nome e idade e imprime mensagem
```py
def saudacao(nome, idade):
    print(f"Olá {nome}, você tem {idade} anos!")
saudacao("João", 30)
```

### Exercício 18: Função que soma elementos de uma lista
```py
def soma_lista(lista):
    return sum(lista)
print(soma_lista([1, 2, 3]))  # Saída: 6
```

### Exercício 19: Função que verifica se número é primo
```py
def eh_primo(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
print(eh_primo(7))  # Saída: True
```

### Exercício 20: Função que retorna fatorial de um número
```py
def fatorial(n):
    resultado = 1
    for i in range(2, n+1):
        resultado *= i
    return resultado
print(fatorial(5))  # Saída: 120
```py
