README - Description of the different code : 

new_data.txt (Noe)
 -> fichier contenant 11556 sequences dont 50% de genes et 50% de orfs
 -> 79 orfs sont aussi des genes (faux negatifs) ou tres proches (> 90%)
 -> pour un gene de taille X, on a mis dans le fichier un orf de taille X (si possible)

another_try.txt (Noe)
 -> contient 223 genes/orfs de longueur = 300, notés avec '...,gene'
 -> contient 223 séquences random de longueur = 300 et notées avec '...,noise'

 => Tres mauvaises predictions des orfs/genes surement car difficultes liees aux non differences de taille

test_jupyter.ipynb (Noe)
 -> traitement du fichier texte contenant les donnees (data.txt ou new_data.txt par exemple)
 -> modele keras (idem a celui d'Alexis)
 -> entrainement du modele par batch de donnees (evite de saturer la RAM en traitant tout d'un coup)
 -> evalutation de la precision du modele
 -> verification des sorties
 -> differents tests realises (code brouillon a la fin : graphes, listes, prints, ...)

test_jupyter_orf_or_not (Noe)
 -> variante de 'test_jupyter'
 -> sépartation d'orfs et de séquences random
 -> utilise le fichier 'another_try.txt'
 => PREDICTION INVERSE IMPLEMENTEE


 
