# Commentaires

>Ne commentez pas le mauvais code, récrivez-le.

>Rien ne peut être plus utile qu’un commentaire bien placé. Rien ne peut encombrer un module autant que des commentaires dogmatiques sans importance. Rien ne peut être plus préjudiciable qu’un ancien commentaire obsolète qui propage mensonges et désinformation.

>Les commentaires sont bien employés lorsqu’ils pallient notre incapacité à exprimer nos intentions par le code. Notez que j’emploie le mot incapacité, car les commentaires masquent toujours nos échecs.

>Par conséquent, lorsque vous éprouvez le besoin d’écrire un commentaire, réfléchissez et essayez de trouver une solution pour exprimer vos intentions avec du code.

>La vérité doit se trouver uniquement dans le code. Seul le code peut indiquer réellement ce qu’il fait. Il représente la seule source d’informations absolument justes. Par conséquent, bien que les commentaires puissent parfois être nécessaires, il est indispensable d’œuvrer à leur extinction.

**Ne pas compenser le mauvais code par des commentaires**

>Très souvent, le mauvais code semble justifier les commentaires.

>Un code clair et expressif avec peu de commentaires est bien supérieur à un code encombré et complexe avec de nombreux commentaires. Au lieu de passer du temps à écrire les commentaires qui expliquent le désordre créé, il est préférable de le passer à nettoyer ce fouillis.

**S’expliquer dans le code**

>En général, il ne faut pas plus de quelques secondes de réflexion pour expliquer la majorité des intentions dans le code. Dans la plupart des cas, il suffit simplement de créer une fonction qui exprime la même chose que le commentaire imaginé.

**Bons commentaires**

>Certains commentaires sont indispensables ou bénéfiques. Nous allons en examiner quelques-uns qui valent pleinement les quelques octets qu’ils occupent. Cependant, n’oubliez pas que le meilleur commentaire est celui que vous pouvez éviter d’écrire.

*Commentaires légaux*

>Les conventions de codage de notre entreprise nous obligent parfois à écrire certains commentaires pour des raisons légales.

*Commentaires informatifs*

>Il est parfois utile de fournir des informations de base à l’aide d’un commentaire.

>Si ce type de commentaires se révèle parfois utile, il est préférable, si possible, d’employer le nom de la fonction pour transmettre des informations.

*Expliquer les intentions*

>Un commentaire ne se limite pas toujours à donner des informations utiles concernant l’implémentation, mais explique les raisons d’une décision.

*Clarifier*

>Il est souvent utile de convertir la signification obscure d’un argument ou d’une valeur de retour en quelque chose de parfaitement lisible. En général, il est préférable de trouver une solution pour qu’un argument ou une valeur de retour clarifie de lui-même sa signification. Cependant, lorsqu’ils font partie de la bibliothèque standard ou d’un code que nous ne pouvons pas modifier, il faut alors se tourner vers un commentaire de clarification.

>Il existe, bien entendu, un risque non négligeable qu’un commentaire de clarification soit erroné.

>Par conséquent, avant d’écrire ce genre de commentaires, recherchez une meilleure solution et vérifiez bien qu’ils sont corrects.

*Avertir des conséquences*

>Dans certains cas, il ne sera pas inutile d’avertir les autres programmeurs quant aux conséquences possibles.

*Commentaires TODO*

>Les commentaires //TODO, qui permettent de laisser des notes du type "À faire", sont
parfois pleinement justifiés.

>Ces commentaires correspondent à des travaux qui, selon le programmeur, devront être réalisés, mais qu’il est impossible de faire actuellement pour une raison ou pour une autre.

>Quelle que soit la raison d’être d’un commentaire TODO, elle ne doit pas justifier la présence d’un mauvais code dans le système.

>La plupart des bons IDE actuels disposent d’une fonction qui permet de localiser tous les commentaires TODO. Par conséquent, il est peu probable qu’ils soient perdus. Néanmoins, votre code ne doit pas être jonché de tels commentaires, et vous devez les parcourir régulièrement pour les éliminer au fur et à mesure.

*Amplifier*

>Un commentaire peut servir à amplifier l’importance d’un point qui, sinon, pourrait paraître sans conséquence.

*Documentation Javadoc dans les API publiques*

>Si vous développez une API publique, vous allez certainement rédiger la documentation Javadoc correspondante. Cependant, n’oubliez pas les autres conseils de ce chapitre. Comme n’importe quel autre commentaire, cette documentation peut être mensongère, mal placée et malhonnête.

**Mauvais commentaires**

>La majorité des commentaires entre dans cette catégorie. Ils servent généralement de béquilles ou d’excuses à du mauvais code, ou bien ils justifient des choix insuffisants, comme si le programmeur se parlait à lui-même.

*Marmonner*

>Si vous ajoutez un commentaire simplement parce que vous pensez que c’est nécessaire ou que le processus l’exige, il s’agit ni plus ni moins d’une bidouille. Si vous décidez d’écrire un commentaire, vous devez passer suffisamment de temps pour vous assurer qu’il soit parfaitement rédigé.

>Un commentaire qui nous oblige à consulter d’autres modules pour comprendre sa signification est un commentaire qui ne parvient pas à communiquer et qui ne vaut pas les quelques octets qu’il consomme.

*Commentaires redondants*

>Il ne donne pas plus d’informations que le code. Il ne justifie pas le code ni ne fournit d’intentions ou de raisons. Il n’est pas plus facile à lire que le code. Il est moins précis que le code et tente de faire accepter au lecteur ce manque de précision, à défaut d’une bonne compréhension. Nous pourrions le comparer à un vendeur de voitures d’occasion enthousiaste qui vous assure qu’il est inutile de regarder sous le capot.

*Commentaires trompeurs*

>Malgré toutes ses bonnes intentions, un programmeur peut parfois inclure dans ses commentaires une déclaration qui n’est pas suffisamment précise pour être juste.

*Commentaires obligés*

>La règle stipulant que chaque fonction doit disposer d’une documentation Javadoc est totalement stupide, tout comme celle obligeant à commenter chaque variable. Les commentaires de ce type ne font qu’encombrer le code, propager des mensonges et conduire à une confusion et à une désorganisation générales.

*Commentaires de journalisation*

>Les développeurs ajoutent parfois un commentaire au début de chaque module lorsqu’ils le modifient. Ces commentaires s’accumulent pour former une sorte de journal de toutes les modifications apportées. J’ai déjà rencontré certains modules contenant des dizaines de pages de ces journaux de modifications.

>Il y a bien longtemps, nous avions une bonne raison de créer et de maintenir ces journaux au début de chaque module. Les systèmes de contrôle du code source n’existaient pas pour le faire à notre place. Aujourd’hui, ces longs journaux ne font qu’encombrer et obscurcir les modules. Ils doivent être totalement supprimés.

*Commentaires parasites*

>Certains commentaires ne sont rien d’autre que du bruit. Ils répètent simplement l’évident et n’apportent aucune nouvelle information.

>Ces commentaires sont tellement parasites que nous apprenons à les ignorer. Lorsque nous lisons le code, nos yeux sautent simplement par-dessus. À un moment donné, les commentaires commencent à mentir car le code associé évolue.

>Vous devez remplacer la tentation de créer du bruit par la détermination à nettoyer votre code. Vous serez ainsi un meilleur programmeur, plus heureux.

*Bruit effrayant*

>La documentation Javadoc peut également représenter du bruit.

>Il s’agit simplement de commentaires parasites redondants écrits par la seule volonté déplacée de fournir une documentation.

*Ne pas remplacer une fonction ou une variable par un commentaire*

>L’auteur du code d’origine a pu tout d’abord écrire le commentaire (peu probable), puis le code qui correspond au commentaire. Cependant, il aurait dû ensuite remanier le code, comme je l’ai fait, afin de pouvoir supprimer le commentaire.

*Marqueurs de position*

>Certains programmeurs ont l’habitude de marquer les emplacements précis dans un fichier source.

>Certaines fois, il peut être sensé de réunir certaines fonctions sous ce type de bannière.

>Réfléchissez. Les bannières sont repérables et évidentes lorsqu’elles se font rares. Vous devez donc les employer en très petite quantité et uniquement lorsque leur intérêt est significatif. Lorsqu’elles sont omniprésentes, elles tombent dans la catégorie du bruit ambiant et sont ignorées.

*Commentaires d’accolade fermante*

>Les programmeurs ajoutent parfois des commentaires spéciaux après les accolades fermantes. Si cela peut avoir un sens dans les longues fonctions contenant des structures profondément imbriquées, ces commentaires ne font que participer au désordre général dans le cas des petites fonctions encapsulées que nous recommandons. Si vous constatez que des accolades fermantes doivent être marquées, essayez plutôt de raccourcir vos fonctions.

*Attributions et signatures*

>Les systèmes de gestion du code source parviennent très bien à mémoriser qui a ajouté quoi et quand. Il est inutile de polluer le code avec ce type de légende.

*Mettre du code en commentaire*

>Peu de pratiques sont aussi détestables que la mise en commentaire d’un bout de code. Ne le faites jamais !

>Ceux qui rencontrent du code mis en commentaire n’ont pas le courage de le supprimer. Ils pensent qu’il existe une raison à sa présence et qu’il est trop important pour être supprimé. Le code en commentaire finit par s’accumuler, comme du dépôt au fond d’une bouteille de mauvais vin.

*Commentaires HTML*

>Le contenu HTML dans les commentaires est une abomination, comme vous pouvez le constater en lisant le code ci-après.

*Information non locale*

>Si vous devez écrire un commentaire, assurez-vous qu’il concerne du code proche. Ne donnez pas des informations globales dans un commentaire local.

*Trop d’informations*

>Il ne faut pas placer des discussions historiques intéressantes ou des détails non pertinents dans les commentaires.

*Lien non évident*

>Le lien entre un commentaire et le code qu’il décrit doit être évident. Si vous vous donnez du mal à écrire un commentaire, vous aimeriez au moins que le lecteur soit en mesure de le consulter avec le code afin de comprendre son propos.

*En-têtes de fonctions*

>Les fonctions courtes n’ont pas besoin d’une longue description. Il est généralement préférable de bien choisir le nom d’une fonction courte qui fait une seule chose que d’ajouter un commentaire en en-tête.

*Documentation Javadoc dans du code non public*

>Si la documentation Javadoc est très utile pour des API publiques, elle est à condamner pour le code privé.