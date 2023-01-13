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

**Éviter les associations mentales**

>Le lecteur ne doit pas avoir à convertir mentalement vos noms en noms qu'il connaît déjà. Ce problème survient généralement lorsque les termes choisis ne font pas partie du domaine du problème ou de la solution.

**Noms classes**

>Pour les classes et les objets, nous devons choisir des noms ou des groupes nominaux comme Customer, WikiPage, Account ou AddressParser. Il est préférable d'éviter les termes Manager, Processor, Data ou Info dans le nom d'une classe. Un nom de classe ne doit pas être un verbe.

**Noms méthodes**

>Pour les méthodes, nous devons choisir des verbes ou des groupes verbaux comme postPayment, deletePage ou save. Les accesseurs, les mutateurs et les prédicats doivent être nommés d’après leur valeur et préfixés par get, set ou is.

**Ne pas faire le malin**

>Si les noms sont trop astucieux, ils ne seront mémorisés que par les personnes qui possèdent le même sens de l’humour que l’auteur, et uniquement aussi longtemps qu’elles se souviendront de la blague.

>Dites ce que vous pensez. Pensez ce que vous dites.

**Choisir un mot par concept**

>Choisissez un mot pour un concept abstrait et restez-y fidèle. Par exemple, il est assez déroutant d’avoir fetch, retrieve et get pour représenter des méthodes équivalentes dans des classes différentes.

>Les noms de fonctions doivent être autonomes et cohérents afin que vous puissiez choisir la méthode adéquate sans autre exploration.

**Éviter les jeux de mots**

>Vous devez éviter d’employer le même mot dans deux sens différents. Si vous utilisez le même terme pour deux idées différentes, il s’agit d’un jeu de mots.

>Si vous respectez la règle "un mot par concept", vous pouvez arriver à un grand nombre de classes qui offrent, par exemple, une méthode add. Tant que la liste des paramètres et la valeur de retour des différentes méthodes add sont sémantiquement équivalentes, tout va bien.

**Choisir des noms dans le domaine de la solution**

>N’oubliez pas que les personnes qui liront votre code seront des programmeurs. Par conséquent, n’hésitez pas et employez des termes informatiques, des noms d’algorithmes, des noms de motifs, des termes mathématiques, etc.

**Choisir des noms dans le domaine du problème**

>La séparation des concepts du domaine de la solution et du problème fait partie du travail du bon programmeur et du bon concepteur. Le code qui est fortement lié aux concepts du domaine du problème doit employer des noms tirés de ce domaine.

**Ajouter un contexte significatif**

>Quelques noms sont en eux-mêmes significatifs, mais ce n’est pas le cas de la plupart. Vous devez redonner aux noms leur contexte en les englobant dans les classes ou des fonctions aux noms appropriés, ou dans des espaces de noms. En dernier ressort, il peut être nécessaire d’ajouter un préfixe aux noms.

**Ne pas ajouter de contexte inutile**

>Tant qu’ils restent clairs, il est généralement préférable de choisir des noms plus courts que des noms longs. N’ajoutez pas de contexte inutile à un nom.

>Les noms accountAddress et customerAddress sont parfaits pour des instances de la classe Address, mais ils font de piètres noms de classes. Address convient parfaitement à une classe.

**Mots de la fin**

>Le choix de bons noms est difficile car cela demande une aptitude à la description et une culture générale partagée. Il s’agit d’un problème d’enseignement, non d’un problème technique, métier ou de gestion. C’est pourquoi peu de personnes apprennent à le faire correctement.

>Les gens ont également peur de renommer les choses, de crainte que d’autres développeurs soulèvent des objections. Nous ne partageons pas cette crainte et sommes plutôt reconnaissants lorsque les noms changent (en mieux).