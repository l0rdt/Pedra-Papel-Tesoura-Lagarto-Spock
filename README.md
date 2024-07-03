# Pedra-Papel-Tesoura-Lagarto-Spock 

Versão digital do JoKenPô visto em The Big Bang Theory.
Originalmente desenvolvido no Colab



from random import randint
from time import sleep

print("""-------- É hora de jogar --------
Pedra Papel Tesoura Lagarto Spock
---------------------------------""")
sleep(1)

print("""Escolha:

[1] PEDRA
[2] PAPEL
[3] TESOURA
[4] LAGARTO
[5] SPOCK""")

print("-=-"*10)
sleep(2)
vc = int(input('Digite o número do que você jogará: '))

pc = randint(1,5)

print('___'*12)
sleep(1)

print("""
PEDRA
    PAPEL
        TESOURA
            LAGARTO
                SPOCK:
__________________________________""")
sleep(1)

if vc == 1:
  print("Você jogou PEDRA")
elif vc == 2:
  print("Você jogou PAPEL")
elif vc == 3:
  print("Você jogou TESOURA")
elif vc == 4:
  print("Você jogou LAGARTO")
elif vc == 5:
  print("Você jogou SPOCK")

if pc == 1:
  print("Eu joguei PEDRA")
elif pc == 2:
  print("Eu joguei PAPEL")
elif pc == 3:
  print("Eu joguei TESOURA")
elif pc == 4:
  print("Eu joguei LAGARTO")
elif pc == 5:
  print("Eu joguei SPOCK")

print("-=-"*10)
sleep(1)

if vc == pc :
  print("Deu Empate: Vamos Jogar de Novo!!!")
elif vc == 1 and pc == 3 or vc == 1 and pc == 4 or vc==2 and pc==1 or vc==2 and pc==1 or vc==3 and pc==2 or vc==3 and pc==4 or vc==4 and pc==5 or vc==4 and pc==2 or vc==5 and pc==3 or vc==5 and pc==1:
  print("Você Ganhou!!!")
elif pc == 1 and vc == 3 or pc == 1 and vc == 4 or pc==2 and vc==1 or pc==2 and vc==1 or pc==3 and vc==2 or pc==3 and vc==4 or pc==4 and vc==5 or pc==4 and vc==2 or pc==5 and vc==3 or pc==5 and vc==1:
  print("Eu Ganhei!!!")
