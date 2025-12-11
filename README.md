# project1
It Is first Project for Try open source 
#benrabah ikram, biochimie appliquée, 6/12/2025 
#bakhti riheb 
#Aina marwa 
#senous chaimae 
#sebdik imene 
#Belaidi salim bilal 

#Dans cette étape nous avons saisi les différentes séquences d'ADN dans un liste python  
#méthode permet de stocker les données de maniére structurée et de les manipuler facilement par la suite  
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
#1)création d un DataFrame (tableau pandas )
df=pd.DataFrame(data)
print("*************création et affichage *************")

#affichage du tableau
print("tableau des séquences ADN:")
print(df,"\n\n")

#2)opération sur tableau :
print("**************opération **************")
#1.) Sélectionner la colonne "longeur"
Longeur=df["longueur"]
print(Longeur)





#2.)Filtrer les longueur supérieur à 10 
print("************* Filtrage des longueur*************")
#filtrer les longueur supérieur à 10 
filtered_df = df[df["longueur"] > 10 ]
print(filtered_df,"\n\n")

#3.)Calculer la moyenne du pourcentage de GC
print("************* Calcul de la moyenne *************")
# Calculer la moyenne du pourcentage de GC
average_gc = df["pourcentage GC"].mean()
print(f"pourcentage moyen de GC : {average_gc:.3f}%")
print(df,"\n\n")


