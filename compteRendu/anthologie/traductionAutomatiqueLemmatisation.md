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
