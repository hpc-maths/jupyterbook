# VII - EDO I : Théorie et bases numériques

S’appuyant sur le cours qui propose une vision claire de la notion de solution pour un système d’équations différentielles ordinaires bien posé mathématiquement au sens de Hadamard (la fonction $f$ est continue et localement Lipschitz), la première partie des notebooks proposés est une « visite » de plusieurs systèmes dynamiques. Ces exemples mêlent systèmes conservatifs et dissipatifs et proviennent de la dynamique des populations, de la mécanique céleste, de la dynamique chimique non-linéaire ou encore de la modélisation du climat. Ils présentent diverses dynamiques : point critique attractif de la dynamique, cycle limite, solution périodique, système chaotique…

Une fois la variété des systèmes dynamiques établie, ainsi que de leur comportement, nous observons les deux schémas d’Euler explicite et Euler implicite étudiés dans le cours sur plusieurs de ces systèmes. Le but est ici de bien comprendre les diverses notions de stabilité, la notion de convergence et la notion de raideur et son impact sur la résolution numérique.

Pour cette dernière, l’étude du système de Hirschfelder et Curtiss est éclairante et permet de comprendre pourquoi les méthodes explicites ont du mal avec les systèmes raides, alors que la méthode implicite, même si aussi peu précise car d’ordre un, a de très bonnes propriétés de stabilité absolue : le schéma d’Euler implicite est même A-Stable.

Une seconde application des deux méthodes numériques sur des systèmes conservatifs issus de la mécanique céleste permet de bien illustrer le manque de précision lié à l’ordre limité des deux méthodes ainsi que l’incapacité des méthodes à préserver l’invariant du système.

Pour finir, nous nous concentrons sur le problème de l’explosion thermique qui combine une forte raideur avec une dynamique explosive impliquant une valeur propre de partie réelle positive et très élevée. Ce problème illustre les difficultés que l’on rencontre avec chacune des deux méthodes, que ce soit en termes de stabilité aux perturbations avec la méthode implicite dans la zone explosive ou la stabilité absolue avec la méthode explicite dans la zone de fin de réaction impliquant une valeur propre à très forte partie réelle négative et donc une très forte raideur.

