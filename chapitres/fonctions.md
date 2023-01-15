# Fonctions

**Faire court**

>La première règle est d’écrire des fonctions courtes. La deuxième règle est qu’elles doivent être encore plus courtes que cela.

>Les fonctions doivent rarement dépasser 20 lignes.

>Dans celui-ci, chaque fonction occupait entre deux et quatre lignes. Chacune était d’une évidence transparente. Chacune avait son scénario. Et chacune amenait à la suivante de manière irréfutable. Vos fonctions doivent avoir cette taille !

*Blocs et indentation*

>Pour parvenir à une telle taille, les blocs des instructions if, des instructions else, des instructions while, etc. ne doivent occuper qu’une seule ligne. Il est fort probable que cette ligne sera un appel de fonction.

>Le niveau d’indentation d’une fonction ne doit donc pas être supérieur à un ou deux.

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

>Idéalement, le nombre d’arguments d’une fonction devrait être égal à zéro (niladique). Ensuite viennent les fonctions à un argument (monadique, ou unaire), puis à deux arguments (diadique). Les fonctions à trois arguments (triadique) doivent être évitées autant que possible.

*Formes unaires classiques*

>Il existe deux raisons très classiques de passer un seul argument à une fonction. Dans le premier cas, vous posez une question à propos de cet argument. Dans le deuxième cas, l’argument est manipulé, pour le transformer en autre chose et le retourner.

>L’événement est une forme moins fréquente, mais toutefois très utile, de fonction à un seul argument. Il existe dans ce cas un argument d’entrée et aucun argument de sortie. Le programme global est conçu de manière à interpréter l’appel de fonction comme un événement et à utiliser l’argument pour modifier l’état du système. Cette forme doit être employée avec prudence. Le lecteur doit voir très clairement qu’il s’agit d’un événement. Choisissez soigneusement les noms et les contextes.

*Arguments indicateurs*

>Les arguments indicateurs sont laids. Passer une valeur booléenne à une fonction est véritablement une pratique épouvantable. Cela complique immédiatement la signature de la méthode, en proclamant que cette fonction fait plusieurs choses. Elle réalise une chose lorsque l’indicateur vaut true et une autre lorsqu’il vaut false !

*Fonctions diadiques*

>Une fonction à deux arguments est plus difficile à comprendre qu’une fonction unaire. Par exemple, writeField(name) est plus simple à comprendre que writeField (outputStream, name). Même si le sens de ces deux fonctions est clair, la première n’accroche pas l’œil car sa signification transparaît immédiatement, tandis que la seconde nécessite une petite pause afin d’ignorer le premier paramètre.

>Il existe cependant des cas où les deux arguments sont appropriés. Par exemple, Point p = new Point(0,0) est parfaitement raisonnable. Les coordonnées cartésiennes prennent naturellement deux arguments. Nous serions plutôt surpris de voir new Point(0). Toutefois, les deux arguments sont, dans ce cas, des éléments ordonnés d’une même valeur !

>Les diades ne sont pas diaboliques et vous devrez certainement en écrire. Cependant, vous devez savoir qu’elles ont un prix et que vous devez exploiter tous les mécanismes disponibles pour les convertir en fonctions unaires.

*Fonctions triadiques*

>Les fonctions qui prennent trois arguments sont encore plus complexes à comprendre que les fonctions diadiques. Les problèmes d’ordre, de pause et d’ignorance sont multipliés. Je vous conseille d’y réfléchir à deux fois avant de créer une fonction triadique.

*Objets en argument*

>Lorsqu’une fonction semble avoir besoin de plus de deux ou trois arguments, il est probable que certains d’entre eux feraient mieux d’être enveloppés dans leur propre classe.

>Vous pourriez croire que la réduction du nombre d’arguments en créant des objets est une forme de tromperie, mais ce n’est pas le cas. Lorsque des groupes de variables sont passés ensemble, à l’instar de x et y dans l’exemple précédent, il est fort probable qu’ils fassent partie d’un concept qui mérite son propre nom.

*Listes d’arguments*

>Il arrive parfois que nous devions passer un nombre variable d’arguments à une fonction. Si les arguments variables sont tous traités de manière identique, ils sont alors équivalents à un seul argument de type List.

*Verbes et mots-clés*

>Le choix de noms appropriés pour les fonctions permet de faire un long chemin vers l’explication des objectifs de la fonction et vers l’ordre et les objectifs des arguments. Dans le cas d’une forme unaire, la fonction et l’argument doivent représenter un couple verbe/nom parfaitement associé.

**Éviter les effets secondaires**

>Les effets secondaires sont des mensonges. Votre fonction promet de faire une chose, alors qu’elle fait également d’autres choses cachées. Parfois, elle apportera des modifications inattendues aux variables de sa propre classe. Parfois, elle les apportera aux paramètres passés à la fonction ou aux variables globales du système. Ces deux cas sont retors et des mensonges préjudiciables qui conduisent souvent à des couplages temporels étranges et à des dépendances d’ordre.

>Les couplages temporels sont déroutants, en particulier lorsqu’ils sont la conséquence d’un effet secondaire. Si vous devez créer un couplage temporel, indiquez-le clairement dans le nom de la fonction.

*Arguments de sortie*

>Les arguments sont naturellement interprétés comme les entrées d’une fonction. Si vous programmez depuis plusieurs années, je suis sûr que vous y avez regardé à deux fois lorsqu’un argument était en réalité une sortie à la place d’une entrée.

>Tout ce qui vous oblige à vérifier la signature de la fonction équivaut à une hésitation. Il s’agit d’une coupure cognitive qui doit être évitée.

>En général, les arguments de sortie sont à proscrire. Si votre fonction doit modifier l’état de quelque chose, faites en sorte que ce soit l’état de l’objet auquel elle appartient.

**Séparer commandes et demandes**

>Les fonctions doivent soit faire quelque chose, soit répondre à quelque chose, non les deux. Une fonction doit modifier l’état d’un objet ou retourner des informations concernant cet objet. En faisant les deux, elle amène une confusion.

**Préférer les exceptions au retour de codes d’erreur**

>Le retour de codes d’erreur à partir de fonctions de commande est une violation subtile de la séparation des commandes et des demandes. Elle incite à employer des commandes comme des expressions dans les prédicats des instructions if.

>Lorsqu’un code d’erreur est retourné, nous obligeons l’appelant à traiter immédiatement l’erreur. En revanche, si nous utilisons des exceptions au lieu de retourner des codes d’erreur, le traitement de l’erreur peut alors être séparé du code principal et simplifié.

*Extraire les blocs try/catch*

>Les blocs try/catch sont intrinsèquement laids. Ils perturbent la structure du code et mélangent le traitement des erreurs au code normal. Il est donc préférable d’extraire le corps des blocs try et catch pour les placer dans leurs propres fonctions.

*Traiter les erreurs est une chose*

>Les fonctions doivent faire une chose. Le traitement des erreurs est une chose. Par conséquent, une fonction qui traite les erreurs ne doit rien faire d’autre. Cela implique que si le mot-clé try est présent dans une fonction, il doit être le tout premier mot de cette fonction et il ne doit rien n’y avoir après les blocs catch/finally.

*L’aimant à dépendances Error.java*

>Lorsque des codes d’erreur sont retournés, cela implique généralement qu’une classe ou une énumération définit tous les codes reconnus. Ces classes sont de véritables aimants à dépendances ; de nombreuses autres classes doivent les importer et les employer.

**Ne vous répétez pas**

>La redondance pose problème car elle fait grossir le code et exige des modifications en plusieurs endroits si l’algorithme vient à évoluer. Elle représente également plusieurs sources d’erreur par omission.

>Dans un logiciel, la redondance peut constituer la source du mal. Plusieurs principes et pratiques ont été imaginés dans le seul but de la contrôler ou de l’éliminer.

**Programmation structurée**

>Certains programmeurs suivent les règles de programmation structurée d’Edsger Dijkstra. Dijkstra stipule que chaque fonction, et chaque bloc dans une fonction, doit posséder une entrée et une sortie. Pour respecter ces règles, il ne doit y avoir qu’une seule instruction return dans une fonction, aucune instruction break ou continue dans une boucle et jamais, au grand jamais, d’instruction goto.

>Même si nous sommes bien disposés envers les objectifs et les disciplines de la programmation structurée, ces règles ont peu d’intérêt lorsque les fonctions sont très courtes. Elles ne valent que dans les fonctions très longues.

>Par conséquent, si vos fonctions restent courtes, les multiples instructions return, break ou continue occasionnelles ne seront pas vraiment un problème. Elles peuvent même parfois être plus expressives que la règle une seule entrée et une seule sortie.

**Écrire les fonctions de la sorte**

>Lorsque j’écris des fonctions, elles sont initialement longues et complexes. Elles contiennent de nombreuses instructions et boucles imbriquées. Leur liste d’arguments est longue, leurs noms sont arbitraires et elles contiennent du code redondant. Mais je dispose également d’une suite de tests unitaires qui couvrent chacune de ces lignes de code grossières.

>Ensuite, je triture et remanie ce code, en décomposant les fonctions, en modifiant des noms et en éliminant la redondance. Je réduis les méthodes et les réordonne. Parfois, j’éclate même des classes entières, tout en faisant en sorte que les tests réussissent.

**Conclusion**

>Tous les systèmes sont construits à partir d’un langage propre à un domaine et conçu par le programmeur pour décrire ce système. Les fonctions représentent les verbes de ce langage, les classes en sont les groupes nominaux.

>Les programmeurs experts voient les systèmes comme des histoires à raconter, non comme des programmes à écrire. Ils se servent des possibilités du langage de programmation choisi pour construire un langage plus riche et plus expressif, qui peut être employé pour raconter cette histoire.

>Ce chapitre s’est focalisé sur la bonne écriture des fonctions. Si vous suivez les règles établies, vos fonctions seront courtes, bien nommées et parfaitement organisées. Mais n’oubliez jamais que le véritable objectif est de raconter l’histoire du système et que les fonctions écrites doivent s’unir proprement en un langage clair et précis pour vous aider dans votre propos.