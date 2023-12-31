# Des boites empilables et paramétrables

Ces boites sont conçus pour être empilables et surtout modifiable en dimensions. 
Le fichier ".f3D" permet de modifier les cotes de cette boite. 

![assemblage_empile.png](images/Assemblage_empile.png)
![assemblage_cote-cote.png](images/assemblage_cote-cote.png)


## 1. Fabrication
### 1.1 Matériel
**Rassembler le matériel suivant : **

|Dénomination|Notes|Quantité|Fournisseur|
|------|------|--|-----|
|Planche de bois contreplaqué 5mm|Planche de 1200mm * 600mm pour chaque fichier de découpe|1|Magasin de bricolage|
|Colle à bois||1|Magasin de bricolage|

**Outils nécessaire :**
 - Découpeuse laser (plateau minimum 300*400mm)
 - Logiciel Inkscape
 - Sert-joint

### 1.2 Fichiers de découpes
Les fichiers de découpes se trouvent dans l'archive au chemin "laser-cuts/boites/"
On y trouve différents dossiers contenenant les fichiers de découpes classés par dimensions de boites. 
Par exemple la boite de hauteur 120mm et avec du bois de 5 mm se trouvera dans le dossier "h120_ep5".

Toutes les boites ont une largeur de 420mm et de profondeur de 290mm. Si vous souhaitez réaliser une boite de taille différente, il est possible de modifier les dimensions en se référent à la partie 2 de cette présente documentation. 

Les numéros de pièces ci-dessous seront mentionnés lors de l'assemblage. 

![nomenclature_pieces.png](images/nomenclature_pieces.png)
![nomenclature_pieces2.png](images/nomenclature_pieces2.png)
![nomenclature_pieces3.png](images/nomenclature_pieces3.png)


### 1.3 Fabrication
 - Coller les charnières (8A et 8B) sur le coté du couvercle (5). 
![avcollage_couvercle.jpg](images/avcollage_couvercle.jpg)
![collage_couvercle.jpg](images/collage_couvercle.jpg)

- Disposer le fond (6) et les 4 cloisons internes comme ceci (2A, 2B, 3A et 3B). 
![avcollage_fond.jpg](images/avcollage_fond.jpg)

- Encoller puis coller les cloisons internes en veillant à disposer de la colles sur toutes les surfaces en contact. 
![collage_int.jpg](images/collage_int.jpg)

- Avant de serrer le tout au moyen de sert-joints, coller les parois externes (1A, 1B, 7A, 7B). 
- Disposer les parois externes comme ceci (Attention à bien veiller à ce que les paroix externes soient disposé symétriquement): 
![avcollage_ext.jpg](images/avcollage_ext.jpg)

- Avant d'encoller, assembler à sec et marquer au crayon à papier les zones qu'il ne faudra pas encoller. 
![marque_1.jpg](images/marque_1.jpg)
![marque_2.jpg](images/marque_2.jpg)

- Encoller les 4 faces une par une puis coller les cloisons extérieur.
![pdcollage_ext.jpg](images/pdcollage_ext.jpg)
![collage_ext.jpg](images/collage_ext.jpg)

- Avant de poser les sert-joints, écarter les deux côtés pour insérer le couvercle.
- Serrer le tout avec des sert-joint et/ou des pinces. 
![serrage_1.jpg](images/serrage_1.jpg)
![serrage_2.jpg](images/serrage_2.jpg)

 - Coller la baguette (4) à l'arrière du couvercle. Elle sert à ratrapper le jour laisser par la système de charnière.  

## 2. Modifier les côtes
Le modèle 3D est paramétrique, c'est à dire que toutes les dimensions du dessin sont calculés selon un ensemble de paramètres que l'on peut modifier (à la manière d'un tableur).

### 2.1 Prérequis
 - Bénéficier d'une licence fusion 360. [Autodesk propose une licence gratuite à dégradé pour usage personnel](https://www.autodesk.com/ca-fr/products/fusion-360/personal).
 - Retrouver le fichier ".f3d" déposé dans l'archive git au chemin : "3Dfiles/modifiable_fusion360"
 
### 2.2 Paramètres
Dans les fichiers 3d des boites d'amorce, il est possible d'agir sur : 

|Nom|Précisions|Notes|
|--|---------|------------|
|**Ep_bois**|Épaisseur des planches qui constitueront la boite|5mm recommandés mais il est possible d'utiliser du mdf et au quel cas ce sera plutôt 6mm|
|**Ep_fond**|Epaisseur de la planche du fond de la boite|Parfois pour contenir des objets lourds il peut-être utile de faire un fond plus épais comme 10mm par exemple.|
|**Pbx**|Profondeur extérieur de la boite||
|**Lbx**|Largeur extérieur de la boite||
|**Hbx**|Hauteur extérieur de la boite||

**Attention** : Pour rester empilable, 2 boites doivent avoir les mêmes dimensions? Seule la hauteur **Hbx** peut varier. 


### 2.3 Modifier les paramètres

 - Dans fusion 360, importer le fichier précédemment téléchargé. 
 - **Ouvrir la table des paramètres**: Dans le menu "Solide" dans le menu déroulant des outils "modifier", cliquer sur "modifier les paramètres"
![chercher tebleau des paramètres](images/recherche_tab_parametres.png)

 - On obtient alors le tableau des paramètres. Toutes les cotes qui ont permis de déterminer les dimansions de cette boite, dépendent de ces 5 valeurs.
 - Pour modifier un paramètre, double-cliquer sur la valeur puis la modifier. Attention ! Ces valeurs sont en millimètre. 
 - Ne pas oublier que pour que des boites puissent s'empiler, leurs paramètres doivent être les même. Seul les hauteurs (Hbx) peuvent varier?
![Tableau des paramètres](images/tab_parametres.png)

 - Ici on a simplement modifié la hauteur à 200mm. 
![Hauteur 200mm](images/hauteur-differente.png)

 - Pour importer les surfaces au format ".svg", il faut uiliser [un pluggin de fusion, "shaper"](https://support.shapertools.com/hc/fr-fr/articles/115002735814-Export-de-fichiers-SVG-depuis-Fusion-360) . Que  l'on retrouve après installation dans le menu "Utilitaires".
![Utilitaire svg](images/slice_svg.png)




