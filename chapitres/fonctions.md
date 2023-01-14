# Fonctions

**Faire court**

>La première règle est d’écrire des fonctions courtes. La deuxième règle est qu’elles doivent être encore plus courtes que cela.

>Les fonctions doivent rarement dépasser 20 lignes.

>Dans celui-ci, chaque fonction occupait entre deux et quatre lignes. Chacune était d’une évidence transparente. Chacune avait son scénario. Et chacune amenait à la suivante de manière irréfutable. Vos fonctions doivent avoir cette taille !

*Blocs et indentation*

>Pour parvenir à une telle taille, les blocs des instructions if, des instructions else, des instructions while, etc. ne doivent occuper qu’une seule ligne. Il est fort probable que cette ligne sera un appel de fonction.

>imbriquées. Le niveau d’indentation d’une fonction ne doit donc pas être supérieur à un ou deux.

**Faire une seule chose**

>UNE FONCTION DOIT FAIRE UNE SEULE CHOSE. ELLE DOIT LA FAIRE BIEN ET NE FAIRE QU’ELLE.

>Toutefois, que signifie précisément "une chose" ?

>Lorsqu’une fonction met en œuvre des étapes qui se trouvent à un seul niveau sous son nom, alors, la fonction réalise une seule chose.

>Par conséquent, une autre manière de savoir si une fonction fait "plusieurs choses" consiste à déterminer s’il est possible d’en extraire une autre fonction dont le nom n’est pas simplement une reformulation de son implémentation.

*Sections à l’intérieur des fonctions*

>Une fonction qui ne fait qu’une seule chose ne peut pas être décomposée en sections.

**Un niveau d’abstraction par fonction**

>Pour être certain que chaque fonction ne fait qu’une seule chose, nous devons vérifier que les instructions qu’elle contient se trouvent toutes au même niveau d’abstraction.

>Mélanger les niveaux d’abstraction au sein d’une même fonction est toujours déroutant. Le lecteur ne sera pas toujours en mesure de déterminer si une expression est un concept essentiel ou un détail.

*Lire le code de haut en bas : la règle de décroissance*

>Nous voulons que le code puisse se lire du début à la fin comme un récit. Nous voulons que chaque fonction soit suivie des fonctions de niveau d’abstraction inférieure, afin que nous puissions lire le programme en descendant d’un niveau d’abstraction à la fois alors que nous parcourons la liste des fonctions vers le bas.

**Instruction switch**

>Il est difficile d’écrire des instructions switch courtes. Même une instruction switch qui ne comprend que deux cas est plus longue que la taille adéquate d’un bloc ou d’une fonction.

>Il est également difficile d’obtenir une instruction switch qui ne fait qu’une seule chose. Par essence, une instruction switch effectue N choses.

>Voici ma règle générale concernant les instructions switch : elles peuvent être tolérées uniquement lorsqu’elles apparaissent une seule fois, sont employées pour créer des objets polymorphes et sont cachées derrière une relation d’héritage, de manière que le reste du système ne puisse pas les voir.

**Choisir des noms descriptifs**

>Plus une fonction est courte et ciblée, plus il est facile de choisir un nom descriptif.

>N’ayez pas peur de créer un nom long. Un nom long descriptif vaut mieux qu’un nom court énigmatique complété d’un long commentaire descriptif.

>N’ayez pas peur de passer du temps à choisir les noms. Vous devez essayer plusieurs noms différents et lire le code correspondant à chacun.

>En choisissant des noms descriptifs, vous clarifiez la conception du module dans votre esprit et il sera ainsi plus facile à améliorer. Il arrive très souvent que la recherche d’un bon nom conduise à une restructuration bénéfique du code.

>Restez cohérent dans le choix des noms. Employez les mêmes phrases, groupes nominaux et verbes dans les noms de fonctions de vos modules.

**Arguments d’une fonction**

*Formes unaires classiques*

*Arguments indicateurs*

*Fonctions diadiques*

*Fonctions triadiques*

*Objets en argument*

*Listes d’arguments*

*Verbes et mots-clés*

**Éviter les effets secondaires**

*Arguments de sortie*

**Séparer commandes et demandes**

**Préférer les exceptions au retour de codes d’erreur**

*Traiter les erreurs est une chose*

*L’aimant à dépendances Error.java*

**Ne vous répétez pas**

**Programmation structurée**

**Écrire les fonctions de la sorte**

**Conclusion**