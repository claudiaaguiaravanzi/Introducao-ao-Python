

AULA 1: INTRODUÇÃO AO GOOGLE COLAB


print("I Primeira competição de programação da Start")


ano="II"

print(ano, "Competição de Programação de Estática")

print(f"{ano} Competição de Programação da Start")

AULA 2: CALCULANDO PONTOS

**Contexto:** 

Uma escola está promovendo uma campanha de incentivo à leitura, em que cada estudante recebe pontos ao concluir livros. Esses pontos podem ser trocados por diferentes premios da escola. As categorias de livros têm valores de pontos diferentes:

* Livro de ficção: 10 pontos
* Livro de não-ficção: 8 pontos
* Livro infantil: 6 pontos

**Problema:**

Rodrigo leu um livro de cada categoria. Agora ele quer saber quantos pontos acumulou com sua leitura.

Nosso objetivo é criar um programa em Python que:

* Armazene a pontuação de cada categoria de livro em uma variável.
* Calcule o total de pontos acumulados por Rodrigo.
* Mostre na tela o total de pontos acumulados por Rodrigo.

livro_ficcao = 10
livro_nficcao = 8
livro_infantil = 6

pontos_rodrigo = livro_ficcao + livro_nficcao + livro_infantil

print(f"Os pontos totais do Rodrigo são: {pontos_rodrigo}")

AULA 3: DISTRIBUINDO ÍTENS

Divisão do tesouro: https://olimpiada.ic.unicamp.br/passadas/OBI2020/fase1/programacao-b/

A turma do 2º ano encontrou um envelope cheio de figurinhas. Para garantir uma divisão justa, todos concordaram com a sugestão de João, o dono do envelope:

Cada amigo, exceto João, deve receber exatamente o mesmo número de figurinhas. João deve receber o dobro da quantidade que cada amigo recebe. Pode ser que o fato de João ser o dono do envelope tenha ajudado a convencer os amigos, mas também contribuiu o fato de que, do jeito proposto, a divisão era exata, sem sobrar nem faltar figurinhas.

**Problema:**

Crie um programa que determine a quantidade de figurinhas que João recebeu, dado o número total de figurinhas no envelope e o número de amigos de João.

**Entrada:**

* A primeira linha contém um número inteiro `total_figurinhas`, que representa o número de figurinhas no envelope.
* A segunda linha contém um número inteiro `numero_amigos`, que representa a quantidade de amigos de João (excluindo o próprio João).

total_figurinhas = int(input("Digite o total de figurinhas: "))
numero_amigos = int(input("Digite o número de amigos: "))

figurinhas_amigos = total_figurinhas // (numero_amigos + 2)
figurinhas_joao = 2 * figurinhas_amigos

print(f"João recebeu {figurinhas_joao} figurinhas.")

AULA 4: USANDO CONDICIONAIS

Bondinho - link: https://olimpiada.ic.unicamp.br/pratique/pj/2017/f1/bondinho/


A turma de um colégio está organizando uma excursão para a serra e, para chegar ao pico da montanha, todos os alunos e monitores devem usar um bondinho. No entanto, a cabine do bondinho tem uma capacidade máxima de 50 pessoas por viagem.

Você precisa criar um programa que verifique se todos os alunos e monitores podem ser transportados em apenas uma viagem.

**Entrada**

* Um número inteiro `numero_alunos`, representando a quantidade de alunos na excursão.
* Um número inteiro `numero_monitores`, representando a quantidade de monitores na excursão.

numero_alunos = int(input("Digite a quantidade de alunos: "))
numero_monitores = int(input("Digite a quantidade de monitores: "))
resposta_positiva = "Pode ir"
resposta_negativa = "Não pode ir"

if numero_alunos + numero_monitores <= 50:
  print(resposta_positiva)
else:
  print(resposta_negativa)

**DESAFIO**
Agora, imagine que infelizmente o bondinho que carrega 50 pessoas está em manutenção e agora todo mundo vai precisar usar um bondinho menos sofisticado e ele só pode levar 30 pessoas. Além disso, 8 professores do colégio também vão participar da excursão. Como fazemos para garantir que o número total de pessoas no bondinho (alunos, monitores e professores) não ultrapasse a capacidade máxima de 30 pessoas?

Seu desafio é escrever um programa que verifique se é possível ou não levar todos em apenas uma viagem.

# Solicita o número de alunos e monitores
numero_alunos = int(input("Digite a quantidade de alunos: "))
numero_monitores = int(input("Digite a quantidade de monitores: "))

# Número fixo de professores
numero_professores = 8

# Capacidade máxima do novo bondinho
capacidade_maxima = 30

# Mensagens de resposta
resposta_positiva = "Pode ir"
resposta_negativa = "Não pode ir"

# Soma total de pessoas
total_pessoas = numero_alunos + numero_monitores + numero_professores

# Verifica se o total é menor ou igual à capacidade
if total_pessoas <= capacidade_maxima:
    print(resposta_positiva)
else:
    print(resposta_negativa)
