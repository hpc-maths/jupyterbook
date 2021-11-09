# X - EDP II : Equations de transport et Burgers

Dans ce chapitre, nous focalisons notre attention sur des équations d’advection linéaire et non-linéaire, dans le même état d’esprit que pour le Chapitre 9. Nous focalisons notre attention dans un premier temps sur l’équation d’advection linéaire puis sur l’équation de Burgers (1948), introduite dans le cadre de la modélisation de la turbulence. Ces équations sont de type hyperbolique ; elles constituent des représentants simples de la classe d’équations aux dérivées partielles que l’on appelle systèmes de lois de conservation (system of conservation laws - voir les références dans le polycopié).

Le point clef de ce chapitre réside dans le fait que ces équations admettent des solutions aux sens classique mais aussi des solutions moins régulières au sens des distributions, qui peuvent comporter des singularités de type discontinuité (on pense à la dynamique des gaz – équations d’Euler et notion d’onde de choc – cf. illustrations du polycopié).

Nous n’insistons pas ici sur la partie théorique que l'on trouvera dans le cours pour les elèves intéressés pas la partie analyse fgonctionnelle, mais la notion de solution faible entropique permet de garantir l’unicité des solutions dans des espaces de solutions très différents de ce que nous avons pu voir au chapitre 9. Ces espaces de solutions incluent donc des solutions discontinues beaucoup moins régulières que celles étudiées précédemment.

Construire un schéma numérique est un alors un défi un peu plus ambitieux puisque les notions de consistance et d’ordre doivent être revue à la lumière des notions de conservation et de solution faible entropique.

Le but de ce notebook est d’expérimenter la résolution de l’équation d’advection et l’équation de Burgers dans des cas où l’on connait la solution exacte (en particulier le petit chapeau) et de montrer que l’on converge bien vers la solution faible pour l'équation d'advection avec le schéma décentrée amont (updwind) et vers la solution faible entropique pour Burgers avec un schéma de type Godunov. En particulier, même si l’on constate que la convergence et la notion d’ordre sont alors à revoir dans le cadre de solution faibles. 

Le but ici n’est pas de rentrer dans les détails des aspects théoriques abordés dans le polycopié mais d’expérimenter et de se rendre compte que le cadre des équations hyperboliques, dont les exemples proposés sont génériques, demande un autre cadre que celui introduit lors de la résolution de l’équation de la chaleur et de l’équation de Nagumo.


