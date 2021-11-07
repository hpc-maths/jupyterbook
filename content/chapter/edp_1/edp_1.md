# IX - EDP I : Équations de la chaleur et de Nagumo

Dans ce chapitre, nous focalisons notre attention sur l’équation de la chaleur, une équation scalaire linéaire, dans un premier temps et abordons ensuite son pendant non-linéaire en ajoutant un terme source non-linéaire pour obtenir une équation de réaction-diffusion dite de Nagumo, qui admet des solutions de type ondes progressives.

Dans la lignée des deux chapitres précédents, nous pouvons commencer la résolution des équations aux dérivées partielles de type équation de la chaleur (équation parabolique) en semi-discrétisant l’équation en espace par une méthode de différences finies d’ordre deux centrée et en gardant le temps comme une variable continue. Le système obtenu est un système d’équations différentielles ordinaires de large taille et qui rentre donc dans le cadre des chapitres précédents. Nous considérons un ensemble de méthodes numériques en temps d’ordre un et deux, explicites et implicites pour résoudre cette équation et faisons le lien entre solution fondamentale exacte, solution quasi-exacte pour une discrétisation spatial fixée et solution numérique de l’EDP sur un intervalle de temps et d’espace. Les ordres de convergence obtenus par la théorie sont retrouvés expérimentalement.

La notion de raideur du système d’EDO obtenu est analysée graphiquement (théoriquement dans le cours) sur la base du spectre de l’opérateur de Laplace continue et de sa discrétisation spatiale par différences finies. On retrouve le conditionnement de la matrice de discrétisation du Laplacien en $1/\Delta x^2$ en lien direct avec la raideur modérée sur système.

Il est alors intéressant de considérer la notion de convergence au sens des EDPs, au-delà de son pendant en version EDO, et d’analyse la convergence en termes des pas d’espace et de temps, dans la lignée de la théorie de Lax et Richtmyer. Il y a ici quelques subtilités suivant comment on lie le pas d’espace et de temps, en particulier lorsque l’on a la latitude de les choisir indépendamment dans le cadre de méthodes implicites. 

Nous terminons par une résolution avec diverses méthodes numériques de l’équation de Nagumo (Splitting, IMEX). Il s’agit d’un cas d’école de résolution d’une équation non-linéaire et permet de saisir l’étendues des techniques possibles pour aborder ce type d’équation.

Les notebooks présentés en amphi sont disponibles [ici](https://moodle.polytechnique.fr/pluginfile.php/325586/mod_folder/content/0/MAP412_Amphi9_Notebooks.zip?forcedownload=1).
