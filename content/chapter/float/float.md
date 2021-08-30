# I - Arithmétique flottante, conditionnement et stabilité

Le Chapitre 1 du cours introduit la représentation des nombres réels en machine et les arrondis associés, mais surtout les notions de conditionnement d’un problème et de stabilité au sens inverse. Ces notions permettent d’analyser les erreurs potentielles que l’on peut générer lorsque l’on implémente une méthode numérique sur ordinateur.

Le lecteur trouvera dans ce chapitre du JupyterBook des exemples permettant d’illustrer ce type de génération d’erreur, qu’elle mène à des pertes de chiffres significatifs ou à des erreurs plus dramatiques. Afin de pouvoir analyser l’influence des erreurs d’arrondi sur les résultats, il est pratique de pouvoir mener des calculs à précision fixée par l’utilisateur et on s’appuie sur le module mpmath qui est présenté dans le premier notebook.

Il permet de comprendre avec quelle précision on doit travailler pour obtenir un résultat précis sur la fonction de Rump et d’analyser les difficultés que l’on rencontre (un exemple proposé en PC permettra d’identifier qu’il s’agit en fait d’un problème mathématique très mal conditionné). 

Le fait de travailler avec une représentation finie des nombres en machine conduit à la perte de certaines propriétés mathématiques et à des « règles » d’implémentation de certaines suites d’opération comme on le voit dans le troisième notebook dédié à la perte de l’associativité de l’addition.

Un domaine classique de l’analyse numérique est celui de la résolution de systèmes linéaires qui fera l’objet du chapitre 4 et pour lequel on définira la notion de conditionnement d’une matrice. En attendant, un quatrième notebook permet de comprendre l’influence de la structure de la matrice sur le conditionnement du problème et d’en avoir une illustration graphique. Cette interprétation permet de bien montrer que le conditionnement est une propriété intrinsèque du problème que l’on cherche à résoudre et n’a rien à voir avec une quelconque méthode numérique de résolution. 

Dans un cinquième notebook, nous reprenons l’illustration de l’influence du conditionnement sur l’évaluation d’une fonction scalaire au moyen de diverses méthodes de calcul. Le lecteur constatera que le choix de l’algorithme d’évaluation a un impact sur la qualité du résultat quand on travaille avec un problème mal conditionné. 

Pour finir, dans un sixième notebook, nous considérons un problème bien conditionné et montrons que l’utilisation d’un algorithme instable au sens backward peut mener à une perte de précision, éventuellement catastrophique.

Ces notebooks doivent permettre d’expérimenter et de mieux comprendre les notions de base de conditionnement et de stabilité et leur influence sur la qualité d’une évaluation numérique d’un problème mathématique du fait des limites imposées par la représentation des nombres réels en machine.



