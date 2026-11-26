# Cours audio — Ondes sonores (transcription)

Transcription du cours audio de révision (10 pistes, ≈ 14 min). L'audio suit l'ordre du document `01_Cours_Ondes_Sonores.html`.

**Conseil d'écoute :** une première fois sans rien faire d'autre, puis une seconde fois avec la fiche sous les yeux, en mettant en pause à chaque formule.

---

## Piste 1 — Introduction

Bienvenue dans ce cours audio de révision sur les ondes sonores. Tu as une évaluation demain, et cet enregistrement a un seul but : te faire entendre, dans l'ordre, tout ce qu'il faut savoir sur les quatre travaux dirigés. Pas de démonstration interminable, pas de calculs à rallonge : uniquement les idées, les formules et les réflexes. Écoute-le une première fois tranquillement, sans rien noter, juste pour te remettre les idées en tête. Puis remets-le une deuxième fois, cette fois avec la fiche de révision sous les yeux, et arrête-toi dès qu'un point te semble flou. On va suivre l'ordre du cours : d'abord le vocabulaire des ondes, ensuite Fourier, puis les cordes vibrantes, puis la propagation dans un fluide, puis l'énergie et les décibels, et pour finir la méthode et les pièges. Allons-y.

## Piste 2 — Le vocabulaire de base

Commençons par la base. Une onde, c'est une perturbation qui se propage en transportant de l'énergie, mais sans transporter de matière. Les molécules d'air qui transmettent un son vibrent sur place : elles ne voyagent pas de ta bouche jusqu'à mon oreille. Il existe deux familles d'ondes, et les exercices utilisent les deux. L'onde progressive : la forme se déplace, par exemple A cosinus de oméga t moins k x. Et l'onde stationnaire : la forme ne se déplace pas, elle gonfle et se dégonfle, par exemple A sinus de k x fois cosinus de oméga t ; certains points ne bougent jamais, ce sont les nœuds. Retiens la phrase clé : une corde de guitare donne des ondes stationnaires, parce qu'elle est coincée aux deux bouts ; un son qui se propage dans l'air loin du musicien est une onde progressive.

Maintenant les cinq grandeurs, et surtout ne les confonds pas. La période T, en secondes : la durée d'un cycle. La fréquence f, égale à un sur T, en hertz. La pulsation oméga, égale à deux pi f, en radians par seconde. La longueur d'onde lambda, en mètres. Et le nombre d'onde k, égal à deux pi sur lambda. Deux relations servent partout : lambda égale c T, c'est-à-dire c sur f ; et c égale oméga sur k. La célérité c dépend du milieu, jamais de la fréquence.

## Piste 3 — Fourier : la série

Deuxième étape : Fourier. L'idée en une phrase : n'importe quel signal, une corde pincée, un son de piano, peut s'écrire comme une somme de sinusoïdes. Fourier, c'est l'art de trouver combien de chaque sinusoïde il y a dans le signal.

Pour un signal périodique de période T, on écrit f de t égale a zéro sur deux, plus la somme, pour n supérieur ou égal à un, de a n cosinus de n oméga zéro t, plus b n sinus de n oméga zéro t. Le terme a zéro sur deux, c'est simplement la valeur moyenne du signal. Les intégrales qui donnent les coefficients sont sur la fiche.

Ce qui compte, c'est le raccourci de parité. Si la fonction est paire, tous les b n sont nuls : il ne reste que des cosinus. Si la fonction est impaire, tous les a n sont nuls, y compris a zéro : il ne reste que des sinus. Premier réflexe devant un énoncé : ma fonction est-elle paire ou impaire ? Ça divise le travail par deux.

Le cas qui tombe à l'évaluation, c'est la corde fixée aux deux bouts. On développe alors uniquement en sinus : u zéro de x égale la somme des b n sinus de n pi x sur L, avec b n égale deux sur L, fois l'intégrale de zéro à L de u zéro de x sinus de n pi x sur L, d x. Pourquoi ? Parce qu'on prolonge la fonction par imparité, et les conditions aux bords sont alors automatiquement respectées. Et pour les fonctions en lignes brisées, un raccourci très rentable : b n égale moins deux sur L k n au carré, fois la somme des sauts de pente multipliés par le sinus au point anguleux.

## Piste 4 — La transformée de Fourier

Toujours dans Fourier, mais pour les signaux non périodiques : la transformée de Fourier. La définition, avec la convention en e moins i deux pi u x : F de u égale l'intégrale sur toute la droite de f de x, e moins i deux pi u x, d x. Attention : certains cours utilisent la convention avec oméga. Les deux sont correctes, mais garde la même dans tout l'exercice.

La table à connaître. La fonction porte donne un sinus cardinal : L sinus de pi u L sur pi u. L'impulsion de Dirac donne un : un spectre plat, toutes les fréquences à poids égal. Un Dirac décalé en x zéro donne e moins i deux pi u x zéro, c'est-à-dire un simple déphasage. Une exponentielle complexe donne un Dirac en u zéro. Un cosinus donne deux Dirac symétriques, avec un facteur un demi. Un sinus, la même chose avec un facteur un sur deux i. Et un peigne de Dirac de pas a donne un peigne de pas un sur a : un peigne fin dans l'espace donne un peigne large en fréquence.

Et l'intuition à garder : étroit contre large. Une impulsion très courte a un spectre très large ; un signal très étalé a un spectre très piqué.

## Piste 5 — La corde vibrante

Troisième étape : les cordes vibrantes. L'équation d'onde s'écrit : dérivée seconde de u par rapport au temps, égale c carré, dérivée seconde de u par rapport à x. Et la formule clé : c égale racine carrée de T sur mu, où T est la tension en newtons et mu la masse linéique en kilogrammes par mètre. Conséquence musicale : plus la corde est tendue, plus c est grand, donc plus le son est aigu ; plus la corde est épaisse, plus c est petit, donc plus le son est grave.

Sans conditions aux limites, la solution est celle de d'Alembert : u égale f de x moins c t, plus g de x plus c t. Deux ondes progressives en sens opposés. Sur une corde fixée aux extrémités, l'onde se réfléchit en changeant de signe, et la superposition d'une onde et de son écho donne une onde stationnaire. C'est la réponse courte à la question : montrer que les solutions sont des ondes stationnaires.

On sépare les variables : u égale X de x fois G de t. Le rapport X seconde sur X égale le rapport G seconde sur c carré G, égal à une constante négative, moins k carré. On résout, et surtout on applique les conditions aux limites : X de zéro égale zéro, donc le cosinus disparaît ; X de L égale zéro, donc sinus de k L égale zéro, donc k L égale n pi. Résultat central : k n égale n pi sur L ; lambda n égale deux L sur n ; oméga n égale n oméga un ; et f n égale n fois c sur deux L. Les fréquences sont quantifiées : le mode n a n fuseaux, n moins un nœuds internes et n ventres. Le mode un, c'est le fondamental.

## Piste 6 — Conditions initiales et musique

Comment trouver les coefficients ? À l'instant zéro : u de x zéro est la somme des A n sinus, et la vitesse initiale est la somme des n oméga un B n sinus. Donc A n, c'est le coefficient de Fourier de la forme initiale. Et attention au piège : c'est n oméga un B n qui est le coefficient de Fourier de la vitesse initiale, pas B n tout seul. Corde lâchée sans vitesse : B n égale zéro. Corde frappée depuis l'équilibre : A n égale zéro.

Deux résultats à connaître. Une corde pincée en a, de hauteur h, donne b n égale deux h L carré, sur pi carré a fois L moins a, fois sinus de n pi a sur L, sur n carré : décroissance en un sur n carré. Une corde frappée par un marteau de largeur e donne une décroissance en un sur n : le spectre est plus riche, c'est le timbre percussif du piano.

Le geste instrumental, c'est de la géométrie : pincer ou frapper en a égale k L sur n impose un nœud, et l'harmonique n disparaît. Pour supprimer le septième harmonique, on pince ou on frappe à L sur sept. Pincer au milieu supprime tous les harmoniques pairs.

Et les ordres de grandeur du violon : une corde de trente-trois centimètres qui donne six cent cinquante-neuf hertz a une célérité de quatre cent trente-cinq mètres par seconde, et une masse linéique de zéro virgule trois gramme par mètre. Si on appuie au tiers de la corde, on crée un nœud, le premier mode possible est le mode trois, et la fréquence la plus basse devient mille neuf cent soixante-dix-sept hertz.

## Piste 7 — Propagation dans un fluide

Quatrième étape : la propagation dans un fluide. Trois ingrédients. Un : la conservation de la masse. Deux : la dynamique, une différence de pression accélère le fluide. Trois : le comportement du fluide, sa compressibilité. On linéarise, c'est-à-dire qu'on ne garde que les petits écarts, puis on dérive et on élimine pour aboutir à l'équation d'onde. Et la célérité vaut un sur racine carrée de rho zéro khi, ou encore racine carrée de B sur rho zéro, où B est le module de compression.

Pour un gaz parfait : c égale racine carrée de gamma R T sur M. Gamma vaut un virgule quatre, R vaut huit virgule trente et un, T en kelvins, et M la masse molaire en kilogrammes par mole. Newton avait supposé la transformation isotherme et trouvait deux cent quatre-vingt-dix mètres par seconde pour l'air : trop faible. Laplace a corrigé avec l'adiabatique, d'où le gamma, et on retrouve trois cent trente et un mètres par seconde. Retiens : c varie comme racine de T, et ne dépend pas de la pression.

Les trois ondes : la pression, la densité et le déplacement. Pression et densité sont proportionnelles, donc en phase. Pression et déplacement sont déphasés de pi sur deux, c'est-à-dire d'un quart de longueur d'onde, parce que la pression est proportionnelle à la dérivée spatiale du déplacement. Là où la surpression est maximale, le déplacement est nul.

Et l'impédance acoustique : Z égale rho zéro c, environ quatre cents dans l'air. Pour une onde plane, p m égale Z fois v m.

## Piste 8 — Énergie et décibels

Cinquième étape : l'énergie. L'intensité, c'est la puissance transportée par unité de surface, en watts par mètre carré. Une seule formule, trois écritures : I égale p m carré sur deux rho c, égale un demi rho c v m carré, égale un demi rho c oméga carré U m carré. Le facteur un demi vient de la moyenne temporelle de sinus carré, qui vaut un demi : ne l'oublie jamais.

Le niveau sonore : L égale dix logarithme décimal de I sur I zéro, avec I zéro égale dix puissance moins douze watts par mètre carré. Les règles : doubler l'amplitude de pression multiplie l'intensité par quatre, soit plus six décibels. Multiplier par dix l'amplitude de pression multiplie l'intensité par cent, soit plus vingt décibels. Et pour gagner dix décibels, il faut multiplier la pression par racine de dix, environ trois virgule seize.

Les repères : zéro décibel, c'est le seuil d'audition, avec une amplitude de pression de deux fois dix puissance moins cinq pascals. Cent vingt décibels, c'est le seuil de douleur. Et un niveau négatif, ce n'est pas une erreur : cela veut simplement dire que l'intensité est inférieure à I zéro.

Dernier point qui impressionne toujours : l'amplitude de déplacement est minuscule. Au seuil d'audibilité, le déplacement de l'air est de l'ordre de dix puissance moins onze mètre. L'oreille est un détecteur extraordinaire.

## Piste 9 — Méthode, réflexes et pièges

Sixième étape : la méthode. Cinq types de questions, cinq réflexes.

Un : développer en série de Fourier. Vérifie la parité, calcule la valeur moyenne, puis les coefficients, et justifie la convergence par le théorème de Dirichlet. Aux discontinuités, la série vaut le milieu du saut.

Deux : calculer une transformée. Écris la définition, découpe selon le support, et utilise les propriétés plutôt que d'intégrer.

Trois : établir une équation d'onde. Pose les trois équations physiques, linéarise, dérive, élimine, puis identifie la célérité.

Quatre : conditions initiales. Écris la série, identifie A n et B n, en n'oubliant pas le facteur n oméga un.

Cinq : le numérique. Convertis en unités internationales, écris la formule littérale avant de remplacer, calcule, puis contrôle l'ordre de grandeur.

Les pièges qui coûtent le plus : oublier de convertir les watts par centimètre carré en watts par mètre carré ; écrire f un égale c sur L au lieu de c sur deux L ; confondre oméga et f ; mettre B n au lieu de n oméga un B n ; oublier le un demi dans l'intensité ; dire que pression et déplacement sont en phase ; utiliser le logarithme népérien au lieu du logarithme décimal ; et vouloir corriger un niveau négatif.

## Piste 10 — Conclusion

Voilà, tu as l'essentiel des quatre travaux dirigés. Un plan simple pour ce soir : écoute une première fois cet enregistrement en entier, sans rien faire d'autre. Ensuite, ouvre les corrections et refais chaque exercice au brouillon avant de lire la solution : c'est là que la mémoire se fixe. Termine par la fiche, en te testant sur les dix questions flash. Demain matin, cinq minutes de relecture des formules suffisent. Tu as le cours, les corrections, la fiche, et maintenant l'audio : il ne manque plus que ton crayon. Bon courage pour demain.
