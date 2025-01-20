# devoirpython
#exo1
n=int(input("veuillez entrer un nombre à 3 chiffres"))
def prem(n):
    for i in range(2, int(n**0.5) + 1):  
        if n % i == 0:
            return False
    return True
nbrprem = [x for x in range(0, n) if prem(x)]

print("Les nombres premiers entre 0 et votre nombre sont :", nbrprem)
def pair(n): 
     if n%2==0:
         return True
nbrpair= [y for y in range(0, n) if pair(y)]
print("Les nombres pairs entre 0 et votre nombre sont :", nbrpair)

somme=sum(nbrprem+nbrpair)
print(" voici la somme des deux listes" ,somme)


#exo2
def lire_fichier():
    meteo={}

#exo3
class compte_bancaire:
    ndcompte=665656202023
    solde=0
def depot():
    d=input(int("veuillez faire un dépôt"))
    solde=d+solde
def retrait():
   montant=int(input("combien voulez-vous retirer?"))
   solde=solde-montant
   if solde<montant:
    print("votre solde est inssuffisant")
    return retrait
def afficher_solde():
    solde=solde
    print(solde)
     
choix=str(input("que voulez vous faire entre un depot et afficher votre solde?"))
if choix=="depot":
    print("combien voulez-vous deposer?")
return depot

elif choix=="afficher":
            print(solde)
    return solde
            
else:
            print("choix valide svp")


    
