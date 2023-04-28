---
title: compte rendu - traduction automatique et lemmatisation
---

Lemmatisation (or lemmatization) in linguistics is the process of grouping together the inflected forms of a word so they can be analysed as a single item, identified by the word's lemma, or dictionary form.

## Utilisation du plongement du domaine pour l'adaptation non supervisée en traduction automatique (Xavier Frenette)

> La traduction automatique (TA) est un processus informatique où un texte dans une langue *source* est traduit vers une langue *cible*.\[] pour être efficace et utile, un bon système de traduction automatique devrait être complet, sans nécessiter de prétraitement ni de postédition humaine de la traduction. (p. 30)

La traduction automatique est née avec l'informatique.
Dictionnaire mécanique -> Traduction statistique -> Traduction neuronale. 

Rapport Automatic Language Processing Advisory Committee (ALPAC), 1966 -> deçu avec la quantité de traductions faites et leur qualité

Traduction Automatique statistique (TAS)
> Avec la TAS, la tâche de traduire un texte n'est plus vue comme une série de règles à applique, mais comme un problème probabiliste qui se résout par la statistique. (p. 31)

Le Perseus a un approche statistique aussi. Il nous donne le percentage de chaque option possible au mot.
Perseus travaille avec une méthode statistique.

Métaphore: la traduction automatique comme un problème de cryptographie.

> Les modèles de TAS resteront les modèles les plus efficaces en TA pendant plus de vignt ans, jusqu'au développement de la traduction automatique par réseaux de neurones. (p. 32)

Traduction automatique neuronale (TAN): les réseaux de neurones sont des modèles d'apprentissage automatique

un modèle TAN résout une tâche de traduction automatique en cherchant une solution à l'équation probabiliste

## Vers un concordanceur-lemmatiseur en ligne du grec ancien (Laurent Kevers and Bastien Kindt)

Le *Projet de recherche en lexicologie grecque*
- Constitution de *corpus* pourvus d'un étiquetage lexical - des entrées systématiquement lemmatisées et désambiguïsées
- Elaboration du *Dictionnaire Automatique Grec* (D.A.G)

Pour chaque mot, les dictionnaires du *Projet* fournissent la forme, son lemme et des codes relatifs à sa flexion. 
Perseus fournit quoi à chaque mot? <-- Il faut décrire cela à mon texte. 

Les dictionnaires permettent la lemmatisation, mais la vérification manuelle qui permet de lever les cas d'ambiguïtés.

Le texte s'affiche en grec polytonique. 
À Perseus, on doit faire la transcription du grec vers l'alphabeth latin

Types de requêtes: un lemme, une forme, un code d'analyse attaché à un lemme. 
Et à Perseus ?

## Perseus

Parmi les objectifs de Perseus: 
> Machine actionable knowledge: catalogue records, encyclopedia articles, lexicon entries, and other structured information sources. Physical access can serve our senses but provides no information about what we are encountering - in effect, physical access is like visiting a historical site about which we may know nothing and where any visible documentation is in a language that we cannot understand. **Machine actionable knowledge allows us to retrieve information about what we are viewing**. Thus, if we encounter a page from a Greek manuscript of Homer, we could at this stage find cleanly printed modern editions of the Greek, modern language translations, commentaries and other background information about the passage on that manuscript page. If we moved through a virtual Acropolis, we could retrieve background information about the buildings and the sculpture.
C'est exactement ça. La machine nous aide à trouver des informations, mais elle ne résout pas les questions posées par la traduction. Perseus n'est pas un logiciel de traduction automatique. 

> Machine generated knowledge: By analyzing existing information automated systems can produce new knowledge. Machine actionable knowledge allows, for example, us to look up a dictionary entry (e.g., facio, "to do, make") in a dictionary or to find pre-existing translations for a passage in Latin or Greek. Machine generated knowledge allows a machine to recognize that fecisset is a pluperfect subjunctive form of facio and to provide reading support where there is no pre-existing human translation. Such reading support might include full machine translation but also finer grained services such as word and phrase translation (e.g., recognizing whether orationes in a given context more likely corresponds to English "speeches," "prayers" or some other term), syntactic analysis (e.g., recognizing that orationes in a given passage is the object of a given verb), named entity identification (e.g., identifying Antonium in a given passage as a personal name and then as a reference to Antonius the triumvir).
La machine nous donne des réponses par rapport aux formes lexicales qu'on trouve aux épigrammes

Fourth-generation collections integrate not only carefully transcribed text and the original page images but also other forms of annotation (e.g., morphological and syntactic analysis, indices of people and places, markup for the particular sense of particular words in context). 
Perseus est maintenant dans la quatrième géneration

## Lemmatization for Ancient Greek. An experimental assessment of the state of the art (Alessandro Vatri, Barbara McGillivray)


Lemma searches --> 
> the researchers specify a dictionary-entry form (or lemma, such as ἄνθρωπος) and all texts containing a word form of that lemma are returned (such as ἀνθρώπου, ἀνθρώπῳ and so on), thus removing the need to specify all inflected forms or spelling variants (p. 180)
Le travail de traduction fait à Perseus suis le chemin inverse. On commence avec une forme d'un mot donné (ἀνθρώπου, pour rester à l'exemple donné par Vatri et McGillivray) pour arrive au lemma (ἄνθρωπος) et à la classification morphosyntatique du mot (un génitif masculin singulier, au cas).

Lemmatization: process in which each word form in a text is associated to its lemma
Lemmatization is expected to disambiguate ambiguous forms in context (ici, la lemmatisation est moins effective. À Perseus, le logiciel nous donne les possibles formes du mot et le porcentage, mais à la fin c'est au traducteur de choisir la bonne interpretation)

Il y a plusieurs "lemmatizers" disponibles pour le grec ancien. 

> Perseus project, ehich was historically one of the first initiatives to build tools for the automatic linguistic analysis of Ancient Greek (and Latin) texts. Gregory Crane has developed the morphological analyzer Morpheus (Crane 1991), which has been implemented on the Perseus Project digital library hosted at Tufts University. Morpheus returns all possible lemmas (and morphological analyses) for a given word

Classical Language Toolkit (CLTK) contains a lemmatizer that disambiguates between multiple lemmas by choosing the most frequent one according to its corpus frequency. 
CLTK runs differents lemmatizers in sequence. So, if one lemmatizer cannot find the answer, another one will be able to lemmatise the word
C'est un cas au champs de la traduction automatique statistique

Perseus est une des sources pour les autres lemmatizers.

Le lemmatizer n'est pas toujours correct. Ainsi, pour les tester, Vatri and McGillivray ont utilisé trois lecteurs de grec ancien d' haute proficiency pour examiner les samples des textes lemmatisés. 
Cela veut dire qu'il faut toujours, au moins jusqu'ici, l'analyse du traducteur/lecteur humain. 

Le plus grand le lexica (les formes déclinnées et les lemmas), le mieux fonctionne le lemmatizer

## Méthodes et pratiques de l'édition critique des textes et documents modernes (Eddie Breuil)

Édition critique: la pratique d'établissement scientifique d'une œuvre
L'éditeur scientifique tente d'agencer les différentes versions d'une œuvre

> l'édition suppose une intervention sur le texte à établir, tandis que la publication suppose une simple mise à disposition sans intervention voulue (p. 11)

Édition critique: établissement du texte.
Édition savante: éclaircissement du texte.

Appareil critique: 
-  chronologie; 
- index des nom propres et des matières;
- bibliographie complémentaire;
- notes et variantes d'un texte, souvent en bas de page

éditon critique -> philologie

être éditeur à *Anthologia* veut dire être au centre d'un travail philologique rafiné et ouvert

> la notion d'auteur en lien étroit avec celle d'œuvre est un facteur déterminant dans l'émergence d'une tradition d'édition des œuvres modernes. (p. 27)

La question posée: faut-il nécessairement faire le choix d'une version? (Breuil)
*Anthologia* réponde cette question par un sonore "non". 
Il ne faut pas choisir parmi les versions et, à la fin, présenter "la bonne version". 
Étant une place de remédiation d'autres éditions, la plateforme fait le choix de ne pas choisir une seule version.
Potentiellement, elle en présente toutes les versions.
L'anthologie est une *forme* qui établit une *structure* pour présenter un *contenu* narrative. (Redefining the anthology)
<!-- à mieux cerner les concepts de forme de et structure-->
L'anthologie est une œuvre dépendante d'autres œuvres.
Dépendant au sens qu'il n'y a pas des anthologies sans qui aient des œuvres sources où l'anthologie va chercher son contenu.
Là, le fait de la remédiation se dévoile.
Pourtant, la remédiation peut être plus ou moins opaque. 
<!-- définition remédiation opaque et transparente-->
*Anthologia* se place au côté de la transparence, une fois qu'elle montre ses plusieurs sources.

Anthologia: édition pluriversionnelle ou édition pluriprésentationnelle

- Éditions pluriprésentationnelles (p. 694)
les éditions conjointes d'un même texte obéissant à des modalites de présentation différentes (p. 695)
Le type le plus répandu est la reproduction du *fac-similé*, accompagnée de sa transcription
Ce que propose ce type d'édition
1. un *fac-similé* du manuscrit
2. transcription diplomatique (pour l'AG il y en a 2 au moins, celle de Waltz et celle de Paton)
3. Une édition du texte
4. Des traductions

> Ces éditions pluriprésentationnelles apportent à la fois des gages de fiabilité et des garanties de démocratisations du patrimoine textuel édité. Elles présentent toutefois un coût certain, relativisé lorsqu'elles sont réalisées sur un format numérique (p. 697)


## Penser le palimpseste numérique (Margot Mellet)

Espace numérique: espace de médiation de corpus antiques. 
Les projets numériques: possibles remédiations, héritage et tradition vers un nouvel héritage en développement

Projet Anthologia: une plateforme éditable par l'utilisateur.trice (API)

Notion du lien faible:

> En effet, si la notion est utilisée dans les théories de l'information et des communications pour qualifier les "simples connaissances" d'un individu dans le contexte des réseaux sociaux (Casilli, 2010; Granovetter, 1973), elle désigne ici les associations libres, faites par l'utilisateur.trice, de contenus divers à un contenu édité et figé, qui est celui de l'*Anthologie palatine* (p. 3)

Liens faibles sont associations libres (c'est, par exemple, un erotomanes devenir un cheia de manias)

Tout lien faible (celui du classiciste et celui de l'amateur.trice) est une émergence de l'imaginaire anthologique.

Une écriture autre, qui peut être étrangère au corpus épigrammatique par rapport à l'époque, à la thématique, auteur, format, langue.

Transmédiation du support papier au support écran

L'AP dévoile des défis philologiques -- plusieurs sources identifiées -- de auteur -- il y a une centaine d'auteur.e.s.

Un objet littéraire ouvert: un dépositaire d'un réseau d'imaginaires.

Anthologia: 
1. metadonnées
- auteur.e;
- URI; 
- Image du manuscrit
2. Texte
- versions et traductions
- alignement du texte
3. Enrichissement
- mots-clefs thématiques;
- images;
- scholies; 
- reférences; 

Anthologie palatine: une œuvre de composition  et résultat d'une somme d'évènements éditoriaux.
Co-construction éditoriale

Les 'types' d'épigrammes à l'AP: 
- épigramme au sens étymologie (inscrit sur une tombe quelconque)
- une inscription brève, mais avec des images poétiques ingénieuses
- un dialogue court

> en couronne épigrammatique, l'*Anthologie palatine* tresse ses éléments autour de nœuds (les topoï) qui génèrent un réseau de connivences d'imaginaires (p. 6)

Imaginaire collectif: dynamiques d'association et d'appropriation transhistoriques de contenus classiques; un commun fondé sur un principe de partage continu de savoirs en réseau.

> le topos structure l'*Anthologie palatine* (intertextualité entre les épigrammes) et révèle sa participation à un imaginaire collectif (hypertextualité) (p. 6)

- Hypertextualité

" Toute relation unissant un texte B (hypertexte) à un texte antérieur A (hypotexte) sur lequel il se greffe d'une manière qui n'est pas celle du commentaire."

Les liens faibles sont de l'hypertextualité
L'hypertextualité (par rapport les liens faibles) fait partie de l'imaginaire anthologique autant que les propres épigrammes 

- Intertextualité

Relation de coprésence entre deux ou plusieurs textes. 

- Transtextualité

La transtextualité comprend la relation entre textes, ainsi que les relations entre un texte et une extratextualité

> Les liens faibles, parce qu'ils se fondent sur un geste d'association libre -- c'est-à-dire sans limitation de forme, de source ou de contenu --, peuvent être des hypertextes, des intertextes, ou ne pas être des textes et participer d'une relatino de transtextualité avec l'épigramme source. (p. 10)
