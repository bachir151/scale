# Espaces, états et émergence
## Du pendule à l’hypothèse d’une réalité explorée par plusieurs formes d’intelligence

*Dialogue recomposé à partir de notre discussion. Les interventions d’Ahmed et les réponses sont reformulées pour la lecture. Les huit étapes suivent l’ordre de l’échange.*

## 1. Qu’est-ce qu’un état ?

**Ahmed.** Je suis obsédé par les notions d’espace et d’état en mathématiques.

**Réponse.** Imagine qu’on photographie un pendule au moment où il passe à la verticale. Il peut aller à gauche, aller à droite ou être immobile. Une photo donne sa position. Que faut-il savoir de plus pour prédire la suite ?

Pour un pendule idéal de longueur fixée dont la loi du mouvement est connue, l’angle et la vitesse angulaire suffisent. Le couple $(\theta,\omega)$ est son **état**. L’angle revient à sa valeur initiale après un tour, donc il vit sur un cercle. La vitesse angulaire, positive, nulle ou négative, vit sur une droite. L’**espace des états** est ainsi un cylindre $S^1\times\mathbb R$. Un point du cylindre représente une situation instantanée. Une trajectoire décrit une histoire, et le pendule peut repasser plusieurs fois par le même point.

En mathématiques, un point peut donc représenter bien plus qu’un lieu. Une fois l’espace choisi, il peut désigner un mouvement initial, une fonction entière ou une distribution de probabilités.

## 2. Peut-on voir cette idée à l’œuvre dans au moins vingt exemples ?

**Ahmed.** Peux-tu creuser encore et me proposer au moins vingt exemples ?

**Réponse.** Les vingt-quatre exemples de notre échange se répartissent autour de quatre questions.

### Que faut-il connaître d’un système physique ?

| Nº | Système | Ce que représente l’espace |
|---|---|---|
| 1 | Aiguille d’horloge | Son orientation appartient au cercle. Les angles 359° et 1° sont à seulement 2° l’un de l’autre. |
| 2 | Deux cadrans indépendants | Chacun fournit un angle. Leur configuration est un point du tore $S^1\times S^1$. |
| 3 | Pendule | Angle et vitesse forment un point du cylindre. Au passage par la verticale, le signe de la vitesse donne le sens du mouvement. |
| 4 | Masse sur un ressort | Le plan $(x,v)$ contient tous les états. À énergie positive fixée, l’équation $kx^2/2+mv^2/2=E$ dessine une ellipse. Un point donne l’état actuel, l’ellipse les états accessibles sur cette trajectoire idéale. |
| 5 | Robot sur le sol | Pour prévoir où le conduira la commande « avance d’un mètre », il faut sa position et son orientation $(x,y,\theta)$. |
| 6 | Livre qui tourne | Si l’on fixe le centre, les orientations forment l’espace des rotations $SO(3)$. Composer deux rotations dans l’ordre inverse peut changer le résultat. |

### Que se passe-t-il quand un point représente un objet entier ?

| Nº | Objet | Lecture de ses coordonnées |
|---|---|---|
| 7 | Polynôme de degré au plus deux | $(a,b,c)$ représente la fonction $x\mapsto ax^2+bx+c$. Le point $(1,0,-1)$ contient ainsi toute l’information sur une parabole. |
| 8 | Droite non verticale | $(m,b)$ représente $y=mx+b$. Les droites passant par $(2,3)$ vérifient $b=3-2m$ et forment elles-mêmes une droite dans l’espace des paramètres. |
| 9 | Solution de $y''+y=0$ | $(A,B)$ représente toute la fonction $A\cos t+B\sin t$. Comme $A=y(0)$ et $B=y'(0)$, l’état initial détermine une histoire complète. |
| 10 | Température le long d’une barre | Dans le modèle continu, un état thermique est une fonction $x\mapsto T(x)$. Un seul point de cet espace peut demander une infinité de valeurs pour être décrit. |
| 11 | Image grise de 100 × 100 pixels | Un point possède 10 000 coordonnées. Avec 256 niveaux, il existe $256^{10\,000}$ images. Il reste à choisir une notion de ressemblance. |
| 12 | Loi sur trois issues | Les triplets de probabilités de somme 1 remplissent un triangle. Ses sommets représentent des certitudes, son centre l’équiprobabilité. |

### Quelle partie du passé peut-on oublier ?

| Nº | Problème | Mémoire suffisante |
|---|---|---|
| 13 | Fibonacci | Conserver les deux derniers termes suffit. La mise à jour est $(a,b)\mapsto(b,a+b)$. |
| 14 | Parité du nombre de 1 | Un bit mémorise « pair » ou « impair ». Lire 1 le fait basculer, lire 0 le conserve. |
| 15 | Reste modulo 3 | Si le reste courant est $r$, lire le chiffre décimal $d$ donne le reste $(10r+d)\bmod 3$. |
| 16 | Parenthèses équilibrées | On compte les ouvertures non refermées. Une fermeture à zéro rend la chaîne invalide. À la fin, le compteur doit être nul. Une imbrication arbitraire demande un compteur sans borne fixée. |
| 17 | Thermostat à deux seuils | Avec allumage sous 19 °C et extinction au-dessus de 21 °C, la température de 20 °C est compatible avec les deux modes. Il faut retenir si le chauffage était allumé. |
| 18 | Urne sans remise | Les effectifs restants $(r,b)$ déterminent la probabilité $r/(r+b)$ d’un tirage rouge dans une urne non vide. Un état peut donc déterminer une loi du futur même quand l’issue reste inconnue. |

Le thermostat fournit une méthode pour éprouver une définition de l’état. Imaginons deux histoires qui arrivent à 20 °C, l’une depuis 18 °C, l’autre depuis 22 °C. Si ces histoires appellent deux commandes différentes, la température seule oublie une information nécessaire. À l’inverse, pour la parité, les préfixes 11 et 0000 sont interchangeables devant toute continuation. Regrouper les histoires équivalentes pour une question donnée permet de construire son espace d’états.

### Que révèlent les transformations autorisées ?

| Nº | Objet | Structure obtenue |
|---|---|---|
| 19 | Trois lampes | Huit configurations forment les sommets d’un cube. Si l’on actionne un interrupteur par pas, la distance minimale compte les lampes qui diffèrent. |
| 20 | Taquin à huit pièces | Relier les dispositions par un glissement autorisé fait apparaître deux composantes. Depuis une disposition donnée, seule la moitié des $9!$ dispositions est accessible. |
| 21 | Graphes simples sur quatre sommets étiquetés | Six arêtes sont possibles. Leurs présences ou absences forment six bits. Changer une arête donne un déplacement élémentaire sur un hypercube de dimension six. |
| 22 | Classements de quatre coureurs | Parmi les 24 ordres, passer de ABCD à DCBA par échanges voisins demande six échanges au minimum. Chacune des six paires doit inverser son ordre. |
| 23 | Directions de droites non orientées | Les angles $\theta$ et $\theta+\pi$ décrivent la même direction. Les identifier conduit à la droite projective réelle $\mathbb{RP}^1$. |
| 24 | Formes de triangles étiquetés | À similitude près, réflexions comprises, deux angles $(A,B)$ suffisent. Les conditions $A>0$, $B>0$, $A+B<\pi$ dessinent un triangle ouvert dont chaque point représente une forme de triangle. |

## 3. Et le modèle d’Ising ?

**Ahmed.** Il y a aussi le modèle d’Ising, non ?

**Réponse.** Plaçons quatre spins sur les sommets d’un carré. L’espace physique contient quatre sites. L’espace des configurations contient seize points, car chacun des quatre spins vaut $+1$ ou $-1$. Si un mouvement élémentaire retourne un spin, ces seize points forment un hypercube de dimension quatre.

La physique apparaît lorsqu’on associe une énergie à chaque configuration. Comptons les quatre côtés du carré, avec interaction ferromagnétique $J>0$ et sans champ extérieur. Deux voisins alignés contribuent pour $-J$, deux voisins opposés pour $+J$. Les signes se lisent en faisant le tour du carré.

| Configuration | Côtés alignés | Énergie | Aimantation totale $M$ |
|---|---:|---:|---:|
| $(+,+,+,+)$ | 4 | $-4J$ | 4 |
| $(+,+,-,-)$ | 2 | 0 | 0 |
| $(+,-,+,-)$ | 0 | $+4J$ | 0 |

Les deux dernières lignes donnent la même aimantation. Pourtant, leurs énergies diffèrent, car la somme des spins oublie qui est voisin de qui. La température ajoute une loi de probabilité sur ce même espace. À basse température, les deux configurations entièrement alignées dominent à l’équilibre. Dans la limite de température infinie, les seize deviennent équiprobables.

## 4. Que deviennent l’entropie, l’information et les catégories ?

**Ahmed.** Et l’entropie dans tout ça ? Et la théorie de l’information ? Et la théorie des catégories ?

**Réponse.** Partons d’une annonce concrète : « L’aimantation du carré vaut zéro. » Que savons-nous désormais de la configuration ?

**Boltzmann compte les possibilités.** Une aimantation de 4 désigne une seule configuration. Une aimantation nulle en désigne $\binom42=6$. L’entropie de Boltzmann du macroétat est $S_B=k_B\ln\Omega$, où $\Omega$ est le nombre de configurations compatibles avec la description retenue.

**Shannon quantifie l’incertitude d’une distribution.** Si les seize états sont équiprobables, l’incertitude initiale est de quatre bits. Voici ce qu’apportent deux résultats possibles d’une même mesure.

| Résultat annoncé | Probabilité | Incertitude restante | Information apportée par ce résultat |
|---|---:|---:|---:|
| $M=4$ | $1/16$ | 0 bit | 4 bits |
| $M=0$ | $6/16$ | $\log_2 6\approx2{,}585$ bits | $4-\log_2 6\approx1{,}415$ bit |

À température finie, les configurations d’aimantation nulle peuvent avoir des probabilités différentes. La formule générale est $H(X)=-\sum_x p(x)\log_2 p(x)$. Pour la même distribution discrète, l’entropie de Gibbs vaut $S_G=-k_B\sum_x p(x)\ln p(x)=k_B\ln(2)\,H(X)$. Le simple logarithme du nombre de possibilités se retrouve pour une loi uniforme.

**Les catégories éclairent la composition des descriptions.** On passe de la configuration à l’aimantation par une application $m$, puis à l’amplitude par la valeur absolue. Leur composée associe directement à une configuration l’amplitude de son aimantation. Les six configurations regroupées au-dessus de zéro constituent la *fibre* de $m$ en zéro.

Peut-on aussi décrire l’évolution au seul niveau de l’aimantation ? Si $F$ retourne le spin supérieur gauche, on cherche une règle $g$ telle que $m\circ F=g\circ m$. Autrement dit, observer avant ou après l’évolution devrait donner des résultats compatibles. Or deux configurations d’aimantation nulle peuvent avoir des spins opposés dans ce coin. Après retournement, l’une passe à $-2$, l’autre à $+2$. Cette contradiction montre exactement pourquoi aucune telle règle déterministe $g$ n’existe ici.

## 5. Et le monde platonicien ?

**Ahmed.** Et le monde platonicien dans tout ça ?

**Réponse.** Si aucun esprit n’avait étudié quatre spins, leur espace à seize états existerait-il quand même ? Le platonicien des mathématiques répond oui. L’expression « monde platonicien » traduit ici une thèse sur l’existence indépendante des objets mathématiques.

Dans *La République* (VI, 510d–e), Platon distingue le carré tracé par le géomètre et le carré sur lequel porte sa démonstration. Le dessin est imparfait. La longueur de la diagonale du carré idéal de côté $a$ vaut pourtant exactement $a\sqrt2$. Le rapprochement avec le platonisme mathématique moderne s’appuie sur cette distinction.

Le carré d’Ising rend sensible la tension entre **choix et découverte**. Nous choisissons quatre variables binaires. Une fois ce cadre fixé, exactement six configurations ont une aimantation nulle. Nous ne pouvons pas décider qu’il y en aura sept. Quatre interrupteurs et quatre spins ont en outre des espaces de configurations isomorphes comme graphes si, dans les deux cas, on change un site par pas. Leurs propriétés physiques peuvent différer alors que la même preuve sur l’hypercube s’applique aux deux. Le platonicien y voit une structure indépendante que l’on découvre. Une autre lecture attribue cette convergence aux règles de représentation que nous avons choisies. La preuve combinatoire laisse cette question philosophique ouverte.

Références évoquées dans l’échange : [Platon, *La République*, livre VI, 509c–511d (extrait en anglais)](https://assets-us-01.kc-usercontent.com/c7bb3f89-eb78-007e-971a-d5864cf7a236/fba27ad2-5ea9-4156-b5a2-22f173798fca/Plato%2C%20_Republic_%2C%20Book%20VI%2C%20Excerpts.pdf) · [*Platonism in the Philosophy of Mathematics*, Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/entries/platonism-mathematics/).

## 6. Comment un espace peut-il en faire émerger un autre ?

**Ahmed.** Ce qui me fascine, c’est comment un espace peut influer sur un autre jusqu’à faire émerger des structures. Je pense au passage du binaire aux espaces vectoriels, puis aux embeddings et aux LLM. J’omets volontairement plusieurs étapes.

**Réponse.** La chaîne devient plus précise dès qu’on distingue le **codage**, les **opérations** et l’**apprentissage**.

1. **Coder.** Quatre bits donnent seize configurations. Munies du XOR et des scalaires binaires, elles forment l’espace vectoriel $\mathbb F_2^4$. Dans un LLM, les bits servent aussi à coder numériquement les coordonnées des vecteurs. L’arithmétique sur ces coordonnées est différente de l’addition par XOR.
2. **Apprendre des représentations.** Des phrases comme « le chat boit » et « le chien boit » soumettent le modèle à des problèmes de prédiction apparentés. L’apprentissage peut faire apparaître des comportements communs aux deux mots. Cette parenté peut se manifester dans plusieurs couches, et sa présence ne garantit pas une faible distance euclidienne entre les embeddings initiaux.
3. **Transformer selon le contexte.** Le même token « souris » peut commencer avec le même vecteur dans « le chat attrape la souris » et « je clique avec la souris ». Les couches du Transformer construisent ensuite des représentations différentes en tenant compte des autres tokens.

Comment un espace agit-il concrètement sur un autre ? Pendant l’entraînement, un point dans **l’espace des paramètres** fixe les opérations du réseau. Ces opérations transforment les vecteurs dans **les espaces de représentations** successifs. La sortie donne un point de **l’espace des probabilités** sur le vocabulaire. Pour « le chat boit du… », si la cible est « lait », la probabilité de cette cible détermine la perte. La rétropropagation en calcule le gradient, et l’optimiseur ajuste les paramètres. Au passage suivant, la même phrase peut suivre une autre trajectoire dans les représentations internes.

Le parallèle avec Ising porte sur une question : comment des règles spécifiées à un niveau rendent-elles possible une organisation observable à un autre ? Dans Ising, des interactions locales peuvent favoriser un ordre collectif. Dans un LLM, les régularités dépendent des données, de l’architecture et de l’objectif d’apprentissage. La possibilité de représenter un motif et le mécanisme qui favorise son apparition sont deux questions distinctes.

## 7. Toute structure se ramène-t-elle à une géométrie ?

**Ahmed.** Peut-on, au fond, résumer toute structure abstraite ou concrète à une géométrie ?

**Réponse.** Quatre bits fournissent une expérience décisive. Avec la règle « retourner un bit par pas », la distance entre 0111 et 1000 vaut quatre. Avec la lecture de ces mots comme entiers binaires, ils valent 7 et 8, donc leur distance numérique vaut un. Le même ensemble porte deux géométries légitimes. Chacune répond à une question différente.

La difficulté se concentre dans le mot *toute*. Dans un réseau de pages web, un lien peut mener de A à B à sens unique. Une distance ordinaire étant symétrique, elle ne peut à elle seule exprimer le sens de ce lien. Un graphe orienté conserve cette relation. Le choix de représentation se juge donc à ce qu’il préserve et à ce qu’il oublie.

Les embeddings donnent une version expérimentale de cette idée. On peut demander quelles relations utiles au langage l’apprentissage traduit par des proximités ou des directions entre vecteurs, et quelles distinctions cette géométrie laisse échapper.

## 8. Une réalité peut-elle produire plusieurs manières de l’explorer ?

**Ahmed.** Si la réalité est un espace de tous les possibles, le cerveau humain pourrait être une entité qui en émerge et qui apprend à l’explorer, avec ses limites. En l’explorant, les humains auraient à leur tour fait émerger des entités comme les LLM. Au sens platonicien, nous aurions découvert et réalisé une possibilité. Humains et LLM exploreraient alors une même réalité par des chemins très différents.

**Réponse.** Cette hypothèse demande de distinguer les états physiquement possibles et l’histoire effectivement parcourue. Dans cette manière de représenter le monde, une trajectoire particulière a conduit à des cerveaux, à des sociétés capables de transmettre leurs découvertes, puis à des machines entraînées sur une partie des traces qu’elles ont produites. Dire que la structure mathématique était possible indépendamment de nous relève d’une lecture philosophique. L’existence de ce modèle entraîné, sur ce support, relève d’une histoire matérielle.

**Pour un objet mathématique**, deux chemins peuvent converger vers une même preuve. Une personne peut dessiner les seize configurations du carré et compter celles d’aimantation nulle. Un LLM peut proposer de choisir deux emplacements parmi quatre. Les deux chemins conduisent à six, et chacun peut être vérifié.

**Pour un objet physique**, l’accès dépend des moyens d’observation et d’action. Si un aimant est posé sur ta table, tu peux le retourner et constater un résultat inattendu. Dans un échange textuel, le modèle dépend de ce que tu lui en rapportes. Il peut proposer une expérience ; tu peux la réaliser ; son résultat peut conduire à revoir l’explication. Ici, « explorer » désigne des opérations observables telles que formuler une hypothèse, en tirer une conséquence et la confronter à une mesure. La question d’une expérience subjective du modèle demeure distincte.

L’intuition finale va au-delà de l’image d’un cerveau qui contemplerait un espace déjà donné. **L’explorateur fait partie du monde qu’il explore.** Des humains produisent des descriptions du monde. Ces descriptions contribuent à entraîner un système qui, à son tour, peut suggérer une expérience. Si quelqu’un la réalise, une représentation du réel aura modifié, par son incarnation physique et son usage, la suite de l’histoire de ce même réel.
