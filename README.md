# Projet programmation S1

Ce projet permet de calculer les dépenses énergétiques journalières d'un utilisateur en prenant en compte l'activité physique réalisée, ainsi que des données personnelles comme le poids, l'âge, le sexe et la taille. L'objectif est d'estimer les calories brûlées à la fois pendant l'activité physique et lors des fonctions basales de l'organisme, grâce à la méthode du métabolisme de base (BMR).

## Fonctionnement du code :

1. **Dataset des Activités Physiques :**
   Le projet utilise un dataset où chaque activité physique est associée à une valeur MET (Metabolic Equivalent of Task). Cette valeur permet de comparer l'intensité des différentes activités physiques et d'estimer la dépense énergétique.

2. **Entrée des données par l'utilisateur :**
   L'utilisateur est invité à saisir les informations suivantes :
   - L'activité physique réalisée.
   - La durée de l'activité en minutes.
   - Son poids en kilogrammes.
   - Son âge.
   - Son sexe (Homme/Femme).
   - Sa taille (pour le calcul du BMR).

3. **Calcul des calories brûlées :**
   En fonction des données saisies, le programme recherche l'activité dans le dataset, applique un calcul basé sur la valeur MET, et ajuste le résultat selon le sexe et l'âge de l'utilisateur. Les calories brûlées pendant l'activité sont calculées par la formule suivante :  Calories brûlées = MET × Poids × (Durée / 60) × Facteur sexe × Facteur âge
   
4. **Calcul du métabolisme de base (BMR) :**
Le BMR est estimé à l'aide de la formule de Harris-Benedict, qui prend en compte le poids, la taille, l'âge et le sexe. Ce calcul donne une estimation des calories brûlées au repos, ce qui permet d'évaluer les besoins énergétiques de l'utilisateur en dehors des activités physiques.

5. **Calcul des dépenses énergétiques totales :**
La dépense calorique totale de la journée est obtenue en additionnant les calories brûlées lors de l'activité physique et celles brûlées au repos (BMR).

## Exemple d'utilisation :

L'utilisateur entre son activité (par exemple, "Course à pied de type marathon"), la durée, son poids, son âge, son sexe et sa taille. Le programme affiche alors :
- Les calories brûlées pendant l'activité.
- La dépense énergétique totale incluant le BMR.


