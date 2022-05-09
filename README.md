# revision_sql

Vous disposez de trois listes, la liste **game_data.csv** contient une liste de jeux vidéos avec le nombre de copie vendu pour chaque jeux, la liste est rangée du jeux le plus vendu aux jeux le moins vendu. La deuxième liste (**game_platform.csv**) contient une liste de console de jeux, et la troisième liste (**game_genre**) contient une liste des différents genres.

## Mise en place
- Télécharger les trois fichiers
- Installer mysql
- Se connecter à mysql en root
- Créer une BDD nommée **video_games**
- Céer un utilisateur nommé **mario** ayant tout les droit sur la BDD **video_games** et se connecter en tant que **mario**
- Créer une table **games** (qui contiendra les données du fichier **game_data.csv**), une table **consoles** qui contiendra les données du fichier **game_platform.csv** et une table genres avec contenant les données de **game_genres**
- Importer les données des fichiers dans leurs tables respectives

## Exercice
1. Combien y a-t-il d'enregistrement dans la table **games** ? 
2. Comment s'apelle le centième jeux le plus vendu ?
3. Au total combien d'exemplaires du premier jeux ont été vendus ?
4. En quel année est sortis le plus vieux jeux de la liste ? (attention 0 n'est pas une année acceptable)
5. Trouver un jeu qui contient les mots **mortal** et **sub** dans son titre.
6. Afficher le rang ainsi que le nom de tous les jeux sortis sur Atari 2600 (**utiliser JOIN**), combien de ligne ont été affichées ?
7. Afficher le rang, le nom, le nom de la platforme et le nom du genre des 10 premiers jeux de la liste (**utiliser JOIN**)
8. Afficher les 50 premiers jeux avec le nom des platformes à la place de leurs id, l'une des lignes n'a pas de nom, sur quel console est ce "jeux" ?
9. Créer une vue qui affichera le rang, le nom du jeux, l'année et le nom de la platforme de tous les jeux sortis entre 1990 et 2000, appeler la vue, combien d'enregistrement sont renvoyés ?
10. Créer un utilisateur **luigi** qui aura uniquement le droits d'apeller la vue
