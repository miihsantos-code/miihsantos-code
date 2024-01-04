
# Importar a biblioteca random
import random

# Definir uma lista de adjetivos
adj = ["belo", "triste", "feliz", "bravo", "gentil", "forte", "doce", "amargo"]

# Definir uma lista de substantivos
sub = ["amor", "flor", "céu", "mar", "sol", "lua", "sonho", "dor"]

# Definir uma lista de verbos
ver = ["cantar", "chorar", "rir", "gritar", "sorrir", "lutar", "beijar", "sofrer"]

# Definir uma função que gera um verso de quatro sílabas
def verso():
  # Escolher um adjetivo, um substantivo e um verbo aleatoriamente
  a = random.choice(adj)
  s = random.choice(sub)
  v = random.choice(ver)
  # Retornar o verso com a primeira letra maiúscula
  return f"{a.capitalize()} {s}\nQue sabe {v}"

# Definir uma função que gera um poema de quatro versos
def poema():
  # Gerar quatro versos e juntá-los com uma quebra de linha
  v1 = verso()
  v2 = verso()
  v3 = verso()
  v4 = verso()
  return f"{v1}\n\n{v2}\n\n{v3}\n\n{v4}"

# Imprimir o poema gerado
print(poema())