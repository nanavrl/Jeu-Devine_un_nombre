

#--------------------------
#  Jeux Devine un Nombre
#--------------------------

from random import * # Import de la biblioteque

print ("Jeux : Deviner un Nombre entre 1 et 100, vous avez droit à 10 essais")

Nbre_Tape = 0
Nbre_Essais = 0
Nbre_A_Deviner = randint(1, 100)

while (Nbre_Tape != Nbre_A_Deviner and Nbre_Essais < 10) :

    Nbre_Tape = int( input("Taper un Nombre : "))
    Nbre_Essais = Nbre_Essais + 1
    
    if Nbre_Tape == 0:
        print("Erreur")

    elif (Nbre_Tape > Nbre_A_Deviner):
        print("Trop Grand")

    elif (Nbre_Tape < Nbre_A_Deviner):
        print("Trop Petit")

    elif (Nbre_Tape == Nbre_A_Deviner ):
        print("Bravo vous avez trouvé le nombre a deviner : ",Nbre_A_Deviner,"en", 10-Nbre_Essais,"coups")

    elif (Nbre_Essais > 10):
        print("!!! Perdu !!! vous avez atteint le nombre d'essais maximum, le nombre a deviner etait : ", Nbre_A_Deviner)







