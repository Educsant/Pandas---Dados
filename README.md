# Python - Data Science do Zero

# =====================================================
# EXCEÇÕES EM PYTHON - TRATANDO ERROS
# =====================================================

# Exceção = erro que pode acontecer durante a execução.
# Em vez do programa parar, podemos tratar o erro.


# -----------------------------------------------------
# EXEMPLO: DIVISÃO
# -----------------------------------------------------

def div(a, b):

    try:
        # Tenta executar este bloco
        resultado = a / b

        print(f"Resultado da divisão de {a} / {b} = {resultado}")

    except ZeroDivisionError:
        # Executa se tentar dividir por zero
        print("Impossível dividir por 0")



# =====================================================
# LISTAS EM PYTHON - EXEMPLOS EXPLICADOS
# =====================================================

# Lista = estrutura usada para armazenar vários valores.
# Pode guardar números, textos e até outras listas.


# -----------------------------------------------------
# 1. CRIANDO LISTAS
# -----------------------------------------------------

# Lista apenas com números inteiros
num_inteiros = [1,2,3,4,5,6,7,8,9,10]

# Lista com tipos mistos (número + texto)
valores_mistos = [1,2,"Var",5,"Pedro"]

# Lista contendo outras listas dentro dela
lista_lista = [num_inteiros, valores_mistos, []]


# -----------------------------------------------------
# 2. TAMANHO DA LISTA
# -----------------------------------------------------

# len() retorna quantos elementos existem na lista
tamanho_lista = len(lista_lista)

print("Quantidade de listas dentro de lista_lista:", tamanho_lista)

# Resultado: 3
# Porque existem 3 itens:
# [num_inteiros], [valores_mistos], []


# -----------------------------------------------------
# 3. SOMA DOS VALORES
# -----------------------------------------------------

# sum() soma todos os números da lista
soma_lista = sum(num_inteiros)

print("Soma dos números:", soma_lista)

# Resultado: 55


# -----------------------------------------------------
# 4. ACESSANDO ELEMENTOS PELO ÍNDICE
# -----------------------------------------------------

# Toda lista começa no índice 0

# posição:  0 1 2 3 4 ...
# valores: [1,2,3,4,5...]

# Índice 3 = quarto elemento
tres = num_inteiros[3]

print("Elemento índice 3:", tres)

# Resultado: 4


# Índices negativos contam de trás para frente

# -1 = último
# -2 = penúltimo
# -3 = antepenúltimo

nine = num_inteiros[-2]

print("Penúltimo elemento:", nine)

# Resultado: 9


# -----------------------------------------------------
# 5. FATIAMENTO DE LISTAS (SLICE)
# -----------------------------------------------------

# Sintaxe:
# lista[inicio:fim]

# Começa no índice informado
# Para antes do índice final


# Do índice 3 até o final
tres_dez = num_inteiros[3:]

print("Do índice 3 até o final:", tres_dez)

# Resultado:
# [4,5,6,7,8,9,10]


# Do índice 5 até antes do 8
cinco_oito = num_inteiros[5:8]

print("Índice 5 até 7:", cinco_oito)

# Resultado:
# [6,7,8]


# Últimos 5 elementos
dez_cinco = num_inteiros[-5:]

print("Últimos cinco elementos:", dez_cinco)

# Resultado:
# [6,7,8,9,10]


# -----------------------------------------------------
# 6. OPERADOR IN
# -----------------------------------------------------

# Verifica se existe determinado valor na lista

print("Var" in valores_mistos)

# Resultado:
# True


print("Lucas" in valores_mistos)

# Resultado:
# False
