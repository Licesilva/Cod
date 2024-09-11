```python
import random

def jogo_adivinhacao():
    print("Bem-vindo ao jogo de adivinhação!")
    numero_secreto = random.randint(1, 100)
    tentativas = 0
    acertou = False

    while not acertou:
        try:
            palpite = int(input("Adivinhe um número entre 1 e 100: "))
            tentativas += 1
            
            if palpite < 1 or palpite > 100:
                print("Por favor, escolha um número entre 1 e 100.")
            elif palpite < numero_secreto:
                print("Muito baixo! Tente novamente.")
            elif palpite > numero_secreto:
                 módulo `random`**: Para gerar um número aleatório.
