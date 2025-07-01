1. Qual o resultado dos dois prints se o usuário digitar altura = 1.00 e peso = 100?

def imc(altura, peso):
    imc = peso / (altura ** 2)
    return imc

x = imc(2.00, 100)
print(x)
altura = float(input('Informe a altura: '))
peso = float(input('Informe o peso: '))
y = imc(altura, peso)
print(y)
Resposta:

x = 25.0, pois 100 / (2.0²) = 100 / 4 = 25.0
y = 100.0, pois 100 / (1.0²) = 100 / 1 = 100.0

Por quê?
A função imc retorna o cálculo de peso dividido pela altura ao quadrado. O valor de x é fixo e o de y depende da entrada do usuário.

2. Média, mediana e moda da lista medidas = [0, 0, 15, 4, 6]
Resposta:

Média: (0 + 0 + 15 + 4 + 6) / 5 = 25 / 5 = 5

Mediana: lista ordenada = [0, 0, 4, 6, 15] → valor do meio = 4

Moda: o número que mais aparece = 0

Por quê?
Moda é o número mais frequente. Mediana é o valor do meio em uma lista ordenada.

3. O que aparece se n1 = 2 e n2 = 4?
   
def media_impar_par(n1, n2):
    media = (n1 + n2) / 2
    if media % 2 == 0:
        print("A média é", media, "e é par")
    else:
        print("A média é", media, "e é ímpar")
Resposta:

Média = (2+4)/2 = 3.0 → 3.0 % 2 = 1 → Ímpar

Por quê?
O operador % retorna o resto da divisão. 3 % 2 = 1 → número ímpar.

4. Qual o resultado final?

frutas = ['maçã', 'banana', 'pêra', 'morango', 'laranja']
frutas.append('ameixa')      # ['maçã', 'banana', 'pêra', 'morango', 'laranja', 'ameixa']
frutas.insert(2, 'uva')      # ['maçã', 'banana', 'uva', 'pêra', 'morango', 'laranja', 'ameixa']
frutas.pop()                 # remove 'ameixa'
frutas.pop(1)                # remove 'banana'
frutas[1] = 'melancia'       # troca 'uva' por 'melancia'
print(frutas[2])             # imprime 'pêra'
Resposta: 'pêra'

Por quê?
Depois das operações, a lista fica:
['maçã', 'melancia', 'pêra', 'morango', 'laranja']

5. Dada a lista medidas = [3, 2, 8, 9, 6, 15, 20, 28, 25, 21]
Comandos:

max(medidas) → 28
min(medidas) → 2
sum(medidas) → 137

Por quê?

max() encontra o maior valor
min() encontra o menor
sum() soma todos os elementos

6. O que será impresso?

cont = 1
while cont <= 5:
    cont += 1
    print(cont)
Resposta: 2 3 4 5 6

Por quê?
O print está após o cont += 1, então ele começa imprimindo 2 até 6 (inclusive).

7. Resultado com break
python
Copiar
Editar
for n in range(1, 6):
    if n == 5:
        break
    print(n)
Resposta: 1 2 3 4

Por quê?
Quando n é igual a 5, o break encerra o laço e não imprime o 5.

8. Cálculo IMC com peso = 100 e altura = 2
python
Copiar
Editar
imc = peso / (altura * altura) → 100 / (2 * 2) = 100 / 4 = 25
Resposta: Sobrepeso

Por quê?
A tabela do IMC diz que 25 ≤ IMC ≤ 29.9 → Sobrepeso.

9. Código TERMINATOR

entrada = input("Digite 'entrar' ou 'sair': ")
...
print("TERMINATOR")
Resposta correta:
A palavra "TERMINATOR" sempre será impressa

Por quê?
Esse print está fora das estruturas condicionais, então será executado sempre.

10. Código com continue

for n in range(1, 6):
    if n == 3:
        continue
    print(n)
Resposta: 1 2 4 5

Por quê?
O continue pula a iteração atual (n == 3), então o
