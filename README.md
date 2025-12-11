# project1
It Is first Project for Try open source 
#benrabah ikram, biochimie appliquée, 6/12/2025 
#bakhti riheb
#Aina marwa 
#senous chaimae 
#sebdik imene 
#Belaidi salim bilal 

#Dans cette étape nous avons saisi les différentes séquences d’ADN dans une liste Python
# méthode permet de stocker les données de manière structurée et de les manipuler facilement par la suite
#Une saisie manuelle garantit également l’exactitude des données avant le début des analyses.

import pandas as pd

#Nous avons utilisé la bibliothèque Pandas afin de créer un DataFrame contenant les séquences.
#Cette structure tabulaire est idéale pour l’analyse de données : elle permet d’ajouter des colonnes, d’effectuer des calculs, et de filtrer les informations rapidement
#Convertir les séquences en tableau constitue une étape essentielle avant toute analyse bioinformatiq

#Données: séquences ADN,longueur ,pourcentage de GC 
data ={
    "Séquences":["ATGCGTACGTA","GCTAGCTAGGCC","ATGCGCGTAAGT","TACGATCGTA","ATGAAAGGCTT","CGTACGTAGC","TTAACCGGAT"],
    "longueur":[11,12,12,10,11,10,10],
    "pourcentage GC":[50,66.67,58.33,40,45.45,60,50]
    }
#création d un DataFrame (tableau pandas )
df=pd.DataFrame(data)
print("**************création et affichage ****************")

#affichage du tableau
print("tableau des séquences ADN:")
print(df,"\n\n")





#opération sur tableau :
print("**************opération **************")
#1.) Sélectionner la colonne "longueur"
Longuer=df["longueur"]
print(Longuer)

