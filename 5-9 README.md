

Aula 5: Aprofundando condicionais 

**Flíper:** https://olimpiada.ic.unicamp.br/pratique/pj/2014/f1/fliper/


Flíper é um jogo em que uma bolinha de metal cai por um labirinto até chegar à parte de baixo. O jogador ganha pontos dependendo do caminho que a bolinha percorre. Ele pode controlar o trajeto da bolinha movendo algumas portinhas no labirinto. Cada portinha pode estar em duas posições: 0 (virada para a esquerda) ou 1 (virada para a direita).

No flíper mostrado na imagem, há duas portinhas. A portinha P está na posição 1 (virada para a direita) e a portinha R está na posição 0 (virada para a esquerda). Isso faz com que a bolinha caia no caminho B.

O programa que você deve escrever precisa, dado o valor das posições de P e R, informar por qual dos três caminhos (A, B ou C) a bolinha vai cair.

**Entrada**

As entradas correspondem a um valor inteiro P (0 ou 1) e um valor inteiro R (0 ou 1) que indicam as posições das portinhas do flíper.




![python jogo flipper.png] (https://drive.google.com/file/d/1GNDYWYhCPryKTrdfR5LGzdp6X6X2eGYA/view?usp=drive_link)

p = int(input("Digite a posição da porta (0 ou 1):"))
r = int(input("Digite a posição da porta (0 ou 1):"))

if p==0 and r==0:
  print("C")
elif p==0 and r==1:
    print("C")
elif p==1 and r==1:
  print("A")
else:
  print("B")

AULA 8: DESAFIO

Bem-vindo ao Caça-Palavras Python!

O seu desafio é encontrar as palavras relacionadas à linguagem Python escondidas na grade de letras.

Regras do jogo:

1.  Observe a grade de letras exibida na tela.
2.  As palavras podem estar em qualquer linha, mas sempre na horizontal.
3.  As palavras estão escondidas horizontalmente. 
4.  Após encontrar uma palavra, você pode marcar ou apenas memorizar.
5.  O objetivo é achar todas as palavras da lista que está logo abaixo da grade.


Divirta-se e teste seu conhecimento sobre Python enquanto se diverte com o caça-palavras!

import random

# Lista de palavras simples sobre Python
palavras = ["FOR", "IF", "ELSE", "LISTA", "FUNCAO"]

# Tamanho da grade
tamanho = 5

# Criar grade com letras aleatórias
grade = [[random.choice("ABCDEFGHIJKLMNOPQRSTUVWXYZ") for _ in range(tamanho)] for _ in range(tamanho)]

# Colocar palavras horizontalmente
for i, palavra in enumerate(palavras):
    if i < tamanho:  # para não ultrapassar o tamanho da grade
        for j, letra in enumerate(palavra):
            if j < tamanho:
                grade[i][j] = letra

# Mostrar grade
print("=== CAÇA-PALAVRAS PYTHON ===")
for linha in grade:
    print(" ".join(linha))

# Mostrar lista de palavras
print("\nPalavras para encontrar:")
print(", ".join(palavras))

