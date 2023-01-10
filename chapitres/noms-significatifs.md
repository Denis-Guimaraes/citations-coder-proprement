# Noms significatifs

**Choisir des noms révélateurs des intentions**

>Le nom d'une variable, d'une fonction ou d'une classe doit répondre à certaines grandes questions : la raison de son existence, son rôle et son utilisation. Si un nom exige un commentaire, c'est qu'il ne répond pas à ces questions.

**Éviter la désinformation**

>Il faut éviter des mots dont le sens établi varie du sens voulu. Par exemple, hp, aix, sco ne sont pas des noms appropriés car il s'agit de noms de plates-formes ou de systèmes Unix.

>Vous devez également faire attention à ne pas choisir des noms trop proches.

**Faire des distinctions significatives**

>Ne pas remplacer des noms de manière arbitraire pour satisfaire le compilateur ou interpréteur.

>Il ne suffit pas d'ajouter des numéros ou des mots parasites, bien que cela puisse satisfaire le compilateur. Si des noms doivent être différents, alors, ils doivent également représenter des choses différentes.

>Imaginons qu'il existe une class Product. Si vous en créez une autre nommée ProductInfo ou productData, vous avez choisi des noms différents sans qu'ils représentent quelque chose de différent. Info et Data sont des mots parasites vagues, tout comme les articles a, an et the.

**Choisir des noms prononçables**

>Si nous ne pouvons pas les prononcer, nous ne pouvons pas en discuter sans paraître idiots. La programmation étant une activité sociale, cet aspect est important.

**Choisir des noms compatibles avec une recherche**

>Les noms d'une seule lettre et les constantes numériques présentent un problème particulier en cela qu'il sont des éléments difficiles à localiser dans le corps d'un texte.

>Si il est facile de chercher MAX_CLASSES_PER_STUDENT, il n'en va pas de même pour le chiffre 7.

>Les noms d'une seule lettre ne doivent être utilisé que pour les variables locales à l'intérieur de méthodes courtes. La longueur d'un nom doit correspondre à la taille de sa portée [n5].

**Éviter la codification**

>Le codage des informations de type ou de portée dans les noms ne fait qu'augmenter le travail de décodage.

>Les noms codifiés sont rarement prononçables et sont sujets aux erreurs de saisie.

>Aujourd’hui la notion hongroise et les autres formes de codification ne constituent que des obstacles. Elles complexifient la modification du nom ou du type d'une variable, d'une fonction ou d'une classe. Elles rendent le code plus difficile à lire. Elles peuvent même conduire le système de codification à tromper le lecteur.

Pour la citation suivante, actuellement je pense que le contraire est mieux, je changerais peut-être d'avis dans le futur.

>Je veux simplement qu'ils sachent qu'il existe un ShapeFactory. Par conséquent, si je dois codifier l'interface ou l'implémentation, j'opte pour l'implémentation. Il est préférable de la nommer ShapeFactoryImp, voir l'horrible CShapeFactory, que de codifier l'interface.

**Éviter les associations mentales**

>Le lecteur ne doit pas avoir à convertir mentalement vos noms en noms qu'il connaît déjà. Ce problème survient généralement lorsque les termes choisis ne font pas partie du domaine du problème ou de la solution.

**Noms classes**

>Pour les classes et les objets, nous devons choisir des noms ou des groupes nominaux comme Customer, WikiPage, Account ou AddressParser. Il est préférable d'éviter les termes Manager, Processor, Data ou Info dans le nom d'une classe. Un nom de classe ne doit pas être un verbe.

**Noms méthodes**

**Ne pas faire le malin**

**Choisir un mot par concept**

**Éviter les jeux de mots**

**Choisir des noms dans le domaine de la solution**

**Choisir des noms dans le domaine du problème**

**Ajouter un contexte significatif**

**Ne pas ajouter de contexte inutile**