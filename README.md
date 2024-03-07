# projet-pelletier

Nous cherchons à analyser les facteurs qui ont influencé les probabilités de survie des différents passagers, lors du naufrage du titanic. Pour ce faire, nous avons un jeu de données comportant diverses variables sur les caractéristiques des passagers (age, prix du ticket, cabine, sexe etc.) ainsi qu’une variable indiquant la survie ou non du passager.
Avant de pouvoir analyser le jeu de données et d’en tirer des inférences, nous devons le nettoyer, et effectuer diverses étapes de processing préliminaires à l’analyse.
D’abord, nous faisons une première visualisation du jeu de données. Nous commençons à nous familiariser avec les variables, leur type, et leurs valeurs.
Ensuite, nous continuons la préanalyse du jeu de données en produisant des statistiques descriptives pour les variables le permettant (les variables numériques).
Un majeur problème dans l’analyse des données risque d’être la présence de valeurs manquantes. Ainsi, nous allons visualiser celles-ci. 
La variable ‘Embarked’ n’a que 2 observations manquantes. Au vu du faible nombre d’observations, nous choisissons d’éliminer les 2 lignes correspondantes. 
La variable ‘Cabin’ a plus de la moitié de ses observations maquantes. Nous choisissons d’éliminer la variable du jeu de données.
La variable ‘age’ a un nombre significatif d’observations manquantes. Nous allons utiliser une méthode d’imputation des valeurs manquantes.

Nous remarquons que presque la moitié des variables du jeu de donnée sont catégorielles. Afin de pouvoir utiliser ces variables pour une modélisation ultérieure, nous ne pouvons les garder en l’état. 
Pour permettre une modélisation avec des variables catégorielles, divers procédés existent. Pour la variable ‘Sexe’ nous allons transformer Masculin/Féminin en une variable binaire.
Pour la variable embarked, nous allons procéder à un encodage dit de label. Il assignera une valeur numérique différente à chaque port d’embarcation.
De plus, nous supposons que la variable name aura un effet sur la probabilité de survie d’un individu. En particulier, la particule du nom ('Mrs', 'Miss', 'Master' etc.)  nous parait intéressante. Est-ce qu’un titre de noblesse augmentera la probabilité de survie ? Pour étudier ceci nous procédons à un encodage à chaud.
 


Une fois notre jeu de données prêt à l’exploitation, nous pouvons nous intéresser aux données.
Pour avoir un premier aperçu, nous pouvons produire une table de statistiques descriptives pour chacune des variables numériques.
Nous pouvons aussi produire des tables de fréquences pour les variables catégorielles. 
Une fois ces premières statistiques produites nous pouvons chercher à visualiser la distribution des différents variables numériques grâce à des histogrammes.
Une fois que nous nous sommes familiarisés avec les différentes variables, nous pouvons chercher à déceler les liens qu’elles ont entre elles. Ainsi, nous étudierons d’une part la distribution de certaines variables conditionnellement à d’autres variables, et deuxièmement la distribution des probabilités de survie selon les différentes variables. 
Une fois que nous avons établi la forme de la relation entre les variables et la survie, nous allons nous intéresser à l’intensité de la relation ainsi qu’à la significativité statistique de la relation. 
