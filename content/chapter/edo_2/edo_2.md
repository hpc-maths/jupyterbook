# VIII - EDO II : Méthodes de Runge-Kutta

Après avoir introduit dans le cadre de méthodes “simples” d’ordre 1 les concepts fondamentaux que l’on retrouve dans beaucoup d’études d’analyse numérique (définitions de stabilité, définitions d’erreur locale de troncature et d’erreur globale, convergence, ordre, notion de raideur), nous allons aborder dans ce cours de manière plus générale l’analyse des méthodes à un pas d’ordre élevé. 

L’idée est d’être plus précis à coût calcul constant ou plus performant en termes de calcul à précision fixée. Nous allons donc reprendre les notions abordées au chapitre précédent et les approfondir dans le cadre de la présentation et l’analyse des méthodes de Runge-Kutta. En particulier, nous avons étudié dans le cours les diverses notions de stabilité pour ces méthodes et les notions de consistance et ordre. 

Dans un premier temps, nous reprenons l’équation de Curtiss et Hirschfelder, qui constitue un très bon modèle jouet permettant de jouer avec la raideur du système et d’illustrer la notion de stabilité linéaire ou stabilité absolue. En particulier, nous considérons les méthodes explicites en lien avec la raideur et le diagramme de stabilité afin de voir l’impact de la raideur et de l’ordre sur les résultats. 

Nous vérifions aussi l’ordre des méthodes implicites de type Radau 3 et 5, ce qui nous permet de montrer l’influence de la montée en ordre sur les performances de la méthode : pour un niveau d’erreur donné, une méthode d’ordre plus élevé est plus efficace.

Nous aborderons ensuite la notion de pas de temps adaptatif basé sur un estimateur d’erreur local, très utile en pratique pour les problèmes raides ; ce type d’approche est présent dans de nombreuses bibliothèques. Nous traitons alors du système d’équations de Belousov et Zhabotinsky (réactions chimiques oscillantes) et montrons l’efficacité de l’estimateur d’erreur local, l’impact de la raideur et la qualité de l’approche de type pas de temps adaptatif sur l’erreur globale.

Pour finir, l’ensemble des méthodes sont testées sur le problème très non-linéaire de l’explosion thermique. Cette équation scalaire implique des valeurs propres réelles positives de très large amplitude dans un régime initial de type explosion puis des valeurs propres réelles négatives de très grande amplitude menant à une très forte raideur en fin d’intégration. Nous illustrons le fait que pour ce type de problème, la « bonne » stratégie consiste à utiliser une méthode implicite à pas de temps adaptatif d’ordre élevé, type Radau 5.


Les notebooks présentés en amphi sont disponibles [ici](https://moodle.polytechnique.fr/pluginfile.php/325583/mod_folder/content/0/MAP412_Notebooks_Cours8.zip?forcedownload=1).
