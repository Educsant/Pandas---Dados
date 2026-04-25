# Listas em Python

# Lista com números inteiros
num_inteiros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Lista com tipos mistos
valores_mistos = [1, 2, "Var", 5, "Pedro"]

# Lista contendo outras listas
lista_lista = [num_inteiros, valores_mistos, []]


# Acessando elementos pelo índice

# Índice 3 = quarto elemento
tres = num_inteiros[3]

# Índices negativos contam de trás para frente
nine = num_inteiros[-2]

print("Penúltimo elemento:", nine)


# Fatiamento de listas

# lista[inicio:fim]
tres_dez = num_inteiros[3:]
print(tres_dez)

# Do índice 5 até antes do índice 8
cinco_oito = num_inteiros[5:8]
print(cinco_oito)

# Últimos cinco elementos
dez_cinco = num_inteiros[-5:]
print(dez_cinco)


# Operador IN - Verifica se um valor existe na lista

print("Var" in valores_mistos)

Resultado: True
