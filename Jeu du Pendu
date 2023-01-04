import random

mots = []
with open("Mots.txt") as fl:
    for l in fl:
        mots.append(l.rstrip("\n"))

mot = random.choice(mots)

#mot = input("Choisis un mot:") #Chosir le mot
essai = 9       #Nombre d'essai
affichage = ""
bonnes_lettres = ""

for l in mot:
  affichage = affichage + " _ "



while essai > 0:
    
    print("Guess it:", affichage)
    proposition = input("Choisis une lettre:")
    

    if proposition in mot:
        print("Tu es sur la bonne voie")
        bonnes_lettres = bonnes_lettres + proposition
    else:
        
        essai = essai - 1
        print("Raté ! Il te reste:",essai,"essais")

    affichage=""
    for l in mot:
        if l in bonnes_lettres:
            affichage += l + " "
        else:
            affichage += " _ "
            
    if "_" not in affichage:
        print("Vous avez gagné le gros lot")
        print("le mot à trouver était:", mot)
        break
