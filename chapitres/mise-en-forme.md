# Mise en forme

>Si quelqu’un soulève le voile, nous voulons qu’il soit impressionné par l’élégance, la cohérence et l’attention portée aux détails dans ce qu’il voit. Nous voulons qu’il soit frappé par l’ordre. Nous voulons qu’il s’étonne lorsqu’il parcourt les modules. Nous voulons qu’il perçoive le travail de professionnels.

>Vous devez faire attention à ce que votre code soit parfaitement présenté. Vous devez choisir un ensemble de règles simples qui guident cette mise en forme et les appliquer systématiquement.

**Objectif de la mise en forme**

>Soyons extrêmement clairs. Le formatage du code est important. Il est trop important pour être ignoré et trop important pour être traité religieusement. La mise en forme du code se place au niveau de la communication et la communication est le premier commandement du développeur professionnel.

>Le style de codage et la lisibilité établissent un précédent qui continue à affecter la facilité de maintenance et d’extension du code bien après que la version d’origine a évolué de manière méconnaissable. Votre style et votre discipline survivent, même si ce n’est pas le cas de votre code.

**Mise en forme verticale**

>Tout d’abord, il est possible de construire des systèmes importants (environ 50 000 lignes pour FitNesse) avec des fichiers contenant généralement 200 lignes, et une taille maximale de 500 lignes. Même si cela ne doit pas constituer une règle absolue, cette approche est très souhaitable. Les fichiers courts sont généralement plus faciles à comprendre que les fichiers longs.

*Métaphore du journal*

>Nous voudrions qu’un fichier source ressemble à un article de journal. Le nom doit être simple, mais explicatif. Ce nom doit nous permettre de déterminer si nous examinons le bon module. Les parties initiales du fichier source doivent fournir les concepts de haut niveau et les algorithmes. Le niveau de détail doit augmenter au fur et à mesure que nous descendons vers le bas du fichier source, pour arriver à la fin où se trouvent les fonctions et les détails de plus bas niveau.

*Espacement vertical des concepts*

>Le code se lit essentiellement de gauche à droite et de haut en bas. Chaque ligne représente une expression ou une clause, et chaque groupe de lignes représente une idée. Ces idées doivent être séparées les unes des autres par des lignes vides.

>Des lignes vides séparent la déclaration du paquetage, l’importation et chaque fonction. Cette règle extrêmement simple a un effet majeur sur l’organisation visuelle du code. Chaque ligne vide est un indice visuel qui identifie un nouveau concept distinct.

*Concentration verticale*

>Si un espacement sépare des concepts, une concentration verticale implique une association étroite. Par conséquent, les lignes de code étroitement liées doivent apparaître verticalement concentrées.

*Distance verticale*

>Avez-vous déjà tourné en rond dans une classe, en passant d’une fonction à la suivante, en faisant défiler le fichier source vers le haut et vers le bas, en tentant de deviner le lien entre les fonctions, pour finir totalement perdu dans un nid de confusion ? Avez-vous déjà remonté la chaîne d’héritage de la définition d’une fonction ou d’une variable ?

>Les concepts étroitement liés doivent être verticalement proches les uns des autres . Bien évidemment, cette règle ne concerne pas les concepts qui se trouvent dans des fichiers séparés. Toutefois, les concepts étroitement liés ne devraient pas se trouver dans des fichiers différents, à moins qu’il n’existe une très bonne raison à cela. C’est l’une des raisons pour lesquelles les variables protégées doivent être évitées.

>Nous voulons éviter que le lecteur ne saute de part en part dans nos fichiers sources et nos classes.

*Déclarations de variables*

>Les variables doivent être déclarées au plus près de leur utilisation. Puisque nos fonctions sont très courtes, les variables locales doivent apparaître au début de chaque fonction.

>Les variables de contrôle des boucles doivent généralement être déclarées à l’intérieur de l’instruction de boucle.

*Variables d’instance*

>A contrario, les variables d’instance doivent être déclarées au début de la classe. Cela ne doit pas augmenter la distance verticale de ces variables, car, dans une classe bien conçue, elles sont employées dans plusieurs voire dans toutes les méthodes de la classe.

*Fonctions dépendantes*

>Lorsqu’une fonction en appelle une autre, les deux doivent être verticalement proches et l’appelant doit se trouver au-dessus de l’appelé, si possible. De cette manière, le flux du programme est naturel. Si cette convention est fidèlement suivie, le lecteur saura que les définitions des fonctions se trouvent peu après leur utilisation.

>Il était préférable de passer la constante depuis l’endroit où la connaître a un sens vers l’endroit où elle est employée réellement.

*Affinité conceptuelle*

>Certaines parties du code veulent se trouver à côté de certaines autres. Elles présentent une affinité conceptuelle. Plus cette affinité est grande, moins la distance verticale qui les sépare est importante.

>Nous l’avons vu, cette affinité peut se fonder sur une dépendance directe, comme l’appel d’une fonction par une autre, ou une fonction qui utilise une variable. Mais il existe également d’autres causes d’affinité. Par exemple, elle peut être due à un groupe de fonctions qui réalisent une opération semblable.

*Rangement vertical*

>En général, nous préférons que les dépendances d’appel de fonctions se fassent vers le bas. Autrement dit, une fonction appelée doit se trouver en dessous d’une fonction qui l’appelle. Cela crée un agréable flux descendant dans le module du code source, en allant des fonctions de haut niveau vers les fonctions de bas niveau.

>Comme dans les articles d’un journal, nous nous attendons à trouver tout d’abord les concepts les plus importants, exprimés avec le minimum de détails superflus possible. Les détails de bas niveau sont supposés arriver en dernier. Cela nous permet de passer rapidement sur les fichiers sources, en retenant l’essentiel des quelques premières fonctions, sans avoir à nous plonger dans les détails.

**Mise en forme horizontale**

>Quelle doit être la largeur d’une ligne ?

>En conclusion, nous devons nous efforcer à écrire des lignes courtes. L’ancienne limite de 80 caractères, fixée par Hollerith, est un tantinet arbitraire et je ne suis pas opposé aux lignes qui dépassent 100 caractères, voire 120. Les largeurs plus importantes indiquent probablement un manque de soin.

*Espacement horizontal et densité*

>Nous employons un espacement horizontal pour associer des éléments étroitement liés et dissocier ceux qui le sont plus faiblement.

>Les opérateurs d’affectation sont entourés d’espaces horizontales pour les accentuer. Ces instructions sont constituées de deux éléments principaux et distincts : le côté gauche et le côté droit. Les espaces permettent de révéler cette séparation.

>En revanche, je ne place aucune espace entre les noms de fonctions et la parenthèse ouvrante. En effet, la fonction et ses arguments sont étroitement liés et ne doivent pas paraître séparés. À l’intérieur des parenthèses d’appel de la fonction, je sépare les arguments afin d’accentuer la virgule et de montrer que les arguments sont distincts.

*Alignement horizontal*

>Je préfère les déclarations et les affectations non alignées, comme dans le code ci-après, car elles révèlent une faiblesse importante. Si je dois aligner de longues listes, le problème se trouve dans la longueur des listes, non dans l’absence d’alignement. La longueur de la liste des déclarations dans FitNesseExpediter indique que cette classe devrait être divisée.

*Indentation*

>Les instructions qui se trouvent au niveau du fichier, comme la plupart des déclarations de classe, ne sont
pas indentées. Les méthodes d’une classe sont indentées d’un niveau vers la droite par rapport à la classe. Les implémentations de ces méthodes sont indentées d’un niveau vers la droite par rapport aux déclarations des méthodes. Les blocs sont indentés d’un niveau vers la droite par rapport à leur bloc conteneur. Et ainsi de suite.

*Rompre l’indentation*

>Il est parfois tentant de passer outre la règle d’indentation pour les instructions if, les boucles while ou les fonctions courtes. S’il m’est arrivé de succomber à cette tentation, j’ai pratiquement toujours fait marche arrière et remis en place l’indentation.

*Portées fictives*

>Parfois, le corps d’une instruction while ou for est fictif, comme dans le code ci-après. Je n’aime pas ce genre de structures et j’essaie de les éviter. Lorsque cela m’est impossible, je fais en sorte que le corps fictif soit correctement indenté et entouré d’accolades.

**Règles d’une équipe**

>Les développeurs de l’équipe doivent se mettre d’accord sur un même style de formatage, puis chaque membre doit le respecter. Un logiciel doit employer un style cohérent. Il ne faut pas que l’on ait l’impression qu’il a été écrit par un ensemble d’individus en désaccord.

>Vous ne devez pas oublier qu’un bon système logiciel est constitué d’un ensemble de documents dont la lecture est agréable. Ils doivent avoir un style cohérent et fluide. Le lecteur doit être certain que la mise en forme rencontrée dans un fichier source aura la même signification dans les autres. Il ne faut pas compliquer inutilement le code source en employant des styles individuels différents.

**Règles de mise en forme de l’Oncle Bob**

>Les règles que j’emploie sont très simples et sont illustrées par le Listing 5.6. Vous pouvez considérer cet exemple comme un document de standardisation d’un bon codage.
