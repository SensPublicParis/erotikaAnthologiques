La traduction des épigrammes vers le portugais faite avec des outils numériques.

## Introduction

La question qu'on se pose est de comment représenter la sexualité de l'autre.
La traduction est de l'intertextualité
Le traducteur doit suivre des normes linguistiques de la langue cible, mais aussi des conventions sociales.

## *Anthologia*, une édition pluriprésentationnelle

[*Anthologia* est une édition pluriprésentationnelle de l'*Anthologie grecque*]{.these}. 
L'édition pluriprésentationnelle est le rassemblement de « éditions conjointes d'un même texte obéissant à des modalites de présentation différentes »[@breuil_methodes_2019, p. 695] ; 
elle est une édition où la remédiation est inhérente.
Dans ce contexte, l'anthologie est une œuvre essentiellement pluriprésentationelle.

<!-- est-ce que toute Anthologie est essentiellement pluriprésentationelle? -->

*Anthologia* est une édition pluriprésentationnelle parce qu'elle fait de la remédiation de différentes éditions de l'*AG*, et chacune de ses éditions a ses propres caractéristiques de présentation. 
Dans le cas de l'épigramme 5.55, *Anthologia* presente 7 éditions de la même épigramme -- *fac-similé*, Paton, Perseus, Waltz et 3 traductions. 
Par exemple, au *fac-similé* du *CP*23, le texte fut manuellement écrit à un *codex*, ainsi on doit comprendre la graphie et l'écriture du copiste, et chaque vers du distique a une formatation particulière, le deuxième vers est en retrait par rapport au premier. 
Aux éditions papiers de Paton, le texte change par rapport à la date de publication. Le texte publié en 1916 n'est pas le même que le texte revisé et publié en 2014. 
À Perseus, le texte est majoritariement la version de 1916 de Paton. 
Nonobstant, comme au cas de l'adjectif *χλοερῖς*, parfois le logiciel qui lit et numérise le texte crée une nouvelle version.

À *Anthologia*, l'épigramme est inscrite à multiples supports -- un parcours d'inscription qui commence aux papyrus et aujourd'hui est au système binaire <!-- le système binaire est le support? L'ordinateur est le support? --> .
[Le *fac-similé* numérisé par la Bibliothèque de l'Université de Heidelberg]{.exemple} :

![*Fac-similé* du *Codex Palatinus* 23, p. 96](http://digi.ub.uni-heidelberg.de/iiif/2/cpgraec23%3A096.jpg/pct:7.56231,40.887,60.77272,16.02525/full/0/default.jpg)

[L’édition numérique de Perseus :]{.exemple}

![Épigramme 5.55 à Perseus](https://user-images.githubusercontent.com/79371444/225750239-6a20c94a-3219-43d8-a74c-e07bfbd289fc.png)

La plateforme *Anthologia* developpe un travail philologique et joue le role d'éditeur scientique. 
[L'éditeur scientifique agence les différentes versions de l'œuvre. Il presente une édition du texte et fournit en paratexte autres lectures]{.concept}. 
*Anthologia* presente plusieurs textes, en différents formats, des metadonnées et des éléments d'enrichissement du texte.
*Anthologia* est une édition scientifique, mais elle n'est pas une édition critique de l'*Anthologie grecque*.
La plateforme propose une édition de l'*AG* dans une pensée philologique autre, où l'œuvre est ouverte et perpétue la procedure anthologique de constant ajout de données [@chaire_de_recherche_du_canada_sur_les_ecritures_numeriques_about_nodate].
Dans ce contexte de multiplicité essentielle, l'idée de « correction du texte » n'est pas applicable.
Aux éditions critiques, il y a toujours un texte qui le plus correct et adéquat.
[Par exemple, Paton et Waltz présentent chacun sa version « correct » du texte, et les variations sont aux paratextes.]{.exemple}
*Anthologia* présente la version de Paton, celle de Waltz, celle de Perseus, et toutes les autres qu'y sont ajoutées.
En plus, toutes ces versions sont au même niveau hiérarchique.

## Traduction automatique et ses outils

[La traduction automatique (TA) est un processus informatique où un texte dans une langue source est traduit vers une langue cible]{.definition}. Un biais d'analyse mesure l'efficience de la TA par rapport à la nécessité d'intervention humaine, où « un bon système de traduction automatique devrait être complet, sans nécessiter de prétraitement ni de postédition humaine de la traduction » [@frenette_utilisation_2022, p. 30]. Dans le cadre de la traduction des épigrammes palatines, on propose de penser autrement. Ici, [la TA est un processus où traitement informatique du texte et l’intervention humaine sont indissociables]{.these}. Seules, les machines ne traduisent pas les épigrammes ; par contre, le traducteur ne fait pas le travail de traduction comme il était fait auparavant. Si les outils sont autres, le travail est autre. On distingue trois étapes dans le développement de la TA : les dictionnaires électroniques, la traduction statistique et la traduction neuronale. Dans la traduction des épigrammes palatines, on travaille avec les dictionnaires électroniques et la traduction statistique.

Les dictionnaires électroniques sont un outil de traduction très efficient. La rapidité d’accès et la quantité d’information rassemblée sont des avantages du dictionnaire électronique par rapport au dictionnaire papier. Prenons Usito, le dictionnaire électronique de l’Université de Sheerbroke, en tant qu’exemple. [Usito a accès à une banque de données, la Banque de données textuelles de Sherbrooke (BDTS), qui a plus de 50 millions de mots-formes [@universite_de_sherbrooke_histoire_nodate]. On tape un mot, et sont affichés des données lexicogrammaticales, la définition du mot, des synonymes et autres informations]{.exemple}. On peut même commettre des fautes orthographiques que le logiciel va proposer des résultats. Les études classiques ont ses dictionnaires électroniques aussi. [Perseus dispose d’une version numérique du *Liddell, Scott, Jones Ancient Greek Lexicon* (LSJ), du *Lexicon to Pindar*, par William J. Slater, et du *A Homeric Dictionary for Schools and Colleges*, par Georg Autenrieth. Ces dictionnaires sont grec-anglais. Mais sont aussi disponibles en ligne *Eulexis*, de la Boîte à outils Biblissima (Baobab) [-@biblissima_baobab_nodate], qui donne accès au LSJ, au dictionnaire grec-allemand de W. Pape et au dictionnaire grec-français de Anatole Bailly]{.exemple}.

Les dictionnaires électroniques sont basés sur la lemmatisation. [La lemmatisation est la procedure linquistique de rassembler toutes les formes déclinées d'un mot]{.definition}. Ainsi, les formes peuvent être analysées comme un item unique, le lemma du mot. La lemmatisation doit aussi désambigüiser [@vatri_lemmatization_2020]. Dans le cadre des textes grecs, la lemmatisation est, par exemple, la machine en cherchant au Marinone [-@marinone_all_1998] une forme inusuelle d'aoriste à la place du traducteur. Perseus a son outil de lemmatisation, Morpheus. Tous les textes à la plateforme sont encodés dans un format TEI-XML. Ainsi, chaque mot du texte est un *input*, et le *output* donné par Morpheus est le *lemma*, ou plusiers *lemmata* selon le cas, et la description morphologique [@perseus_digital_library_open_nodate]. De cette façon, pour une recherche lexicogrammaticale, il sufit de cliquer sur le mot. 

![On clique sur le mot *ἅψεσιν*](https://user-images.githubusercontent.com/79371444/229613376-7aec500c-a1fb-4642-8ac9-a868e933aa18.png)

![Morpheus donne la description morphologique](https://user-images.githubusercontent.com/79371444/229820348-e1b43b4e-2938-48e2-816c-6edef0059b92.png)

Morpheus a un approche statistique, où [la tâche de traduire un *lemma* n'est plus vue comme une série de règles à appliquer, mais comme un problème probabiliste qui se résout par la statistique]{.definition} [@frenette_utilisation_2022 p. 31]. Le système de Morpheus est basée sur cinq éléments :

1. L'évaluation de la fréquence du mot, où est compté combien de fois la forme dictionnarisé (nominatif singulier pour les noms et première personne du singulier de l'indicatif présent pour les verbes) du mot apparaît au *corpus* de Perseus. Ce critère n'est utilisé qu'au cas d'ambiguité ;
2. L'évaluation de la fréquence de la forme du mot, où est compté combien de fois les traits morphologiques (la personne, le mode et le nombre pour les verbes; le cas, le genre et le nombre pour les noms) ocurrent dans tous les mots au *corpus* de Perseus ;
3. Les votes des usagers, qui votent pour detérminer le bon choix. Aujourd'hui, n'est plus possible de voter
4. L'évaluation de la forme du mot précedent, où la forme du mot précedent est un critére pour l'analyse du mot. Il trouve la forme la plus probable parmi les caractéristiques morphologiques du mot analysé et les caractéristiques possibles du mot précédent en fonction de la fréquence de chaque paire possible ;
5. L'évaluation précalculé d'occurence des pairs morphologiques [@perseus_digital_library_open_nodate]. 

Au cas d'*ἅψεσιν*, Morpheus présente deux *lemmata* : *ἅψος, ους (τό)* et *ἅψις,εως (ἡ)*. Face à ces diverses possibilités, Morpheus va classer la probabilité de chacune des options. En agissant de cette façon, l'outil travaille au sein de la traduction statistique. Après l'analyse statistique, Morpheus atteint le chiffre de 52,1% pour *ἅψις,εως (ἡ)*. Or, comme on vera plus tard à ce texte, *ἅψις,εως (ἡ)* n'est pas la bonne option ici. Le logiciel est un outil de traduction, mais il ne traduit pas seul. Le traducteur doit faire des choix, surtout lorsqu'on travaille avec un objet pluriel comme les épigrammes de l'*AG*.

<!-- 
mentionner des cas où le dictionnaire ne trouve pas les mots envisagés.?
Je pense que n'est pas le cas de discuter ce point ici. De quelque façon, je laisse ce note pour y réflechir un peu plus au futur.
-->

## Comment traduire le *pornikotaton*

Les traductions vers de Paton et de Waltz font partie des édition présentes à *Anthologia*.
Ainsi, dans un première moment, on analyse les choix de Paton et de Waltz pour ensuite présenter mes choix et discuter si *πορνικώτατος* veut dire plus pornographique.

### Les traductions de Paton et de Waltz

L'épigramme 5.55 est considerée *πορνικώτατον* par le lemmatiste C. 
Traduire l'érotique demande choisir avec soin des termes à utiliser, et on se demande pourquoi C a utilisé ce superlative pour classer 5.55. 
Quelles sont les caractéristiques déploiées au texte pour qu'il soit *πορνικώτατον* ? 
L'adjectif *πορνικός,ή, όν*, selon le Bailly [-@biblissima_eulexis_nodate], veut dire « de prostituée ». 
À 5.55.2, C écrit aussi que l'épigramme est dediée à « Doris, la prostituée »^[*εἰς Δωρίδα τὴν πόρνην*]. 
Au texte de l'épigramme, il n'y a aucune référence explicite que Doris soit en fait une prostituée. 
C'est C qui determine l'ocupation de Doris et le caractère de « putasserie » de l'épigramme. 
Autres traducteurs, on pense principalement à Paton, on suivi l'indication de C et on lu 5.55 en tant qu'une épigramme très obscène. 
L'obscènité de l'épigramme pousse le traducteur à prendre des choix dans la présentation de son texte.

Les érudits du XIX^ème^ siècle et début du XX^ème^ avaient une méthode pour « cacher » l'obscenité des textes : ils vont traduire ces passages dans une langue autre ou vont les remplacer par des points de suspension [@pierreville_choix_2018 p. 153]. 
Paton a choisit de traduire les passages « licencieuses » de l'*AG* vers le latin, et l'épigramme 5.55 fut traité de cette façon.
Ainsi, dans son édition de 1916, la traduction de 5.55 est :

> *Doride roseis natibus puella super grabatulum distenta in floribus roscidis immortalis factus sum. Ipsa enim mirabilibus pedibus medium me amplexa, rectamque se tenens, absolvit longum cursum Veneris, oculis languidum tuens ; hi autem velut vento folia tremebant purpurei, dum circumagitabatur, donee effusum est album robur ambobus et Doris solutis jacuit membris*. [@paton_greek_1916]

Traduire vers une langue autre indique un type de censure, une tentative de préserver le lecteur du choc et de la confrontation crue avec les réalités corporelles et sexuelles apportées par l'épigramme. 
C'est un choix de traduction courant au passé, mais un choix extrême parce que le traducteur prendre des décisions à la place du lecteur. 
Il decide que le texte est obscène et par conséquent le lecteur ne peut pas aisement en accèder. 
Il traduit vers le latin parce qu'il juge que le texte a des propos qui peuvent déranger la morale et la pensée *mainstream* [@vitali-rosati_ce_2021]. 
De cette façon, il faut limiter le nombre de lecteurs aux gens qui lisent le latin.
Ces lecteurs -- les érudits, le clergé et les élites surtout -- sont censés d'être suffisament éclairés pour traiter le fait de l'écriture pornographique.
De cette façon, le texte est traduit, mais il n'est pas compréhensible par tous.

Waltz traduit l'épigramme 5.55 vers le français. <!-- qu'est-ce que je peux dire à propos de Waltz? --> 

### Vers le portugais

À l’édition de Perseus, le texte du premier distique est :

> Δωρίδα τὴν ῥοδόπυγον ὑπὲρ λεχέων διατείνας  
**ἅψεσιν ἐν χλοερῖς** ἀθάνατος γέγονα.^[Quando Doris de nádegas rosáceas estava em meu leito     
e eu abri suas pernas juvenis, tornei-me imortal.]

Au passage, Perseus apporte le nom *ἅψος, ους (τό)*, qui est traduit par « attache d’un membre, articulation ». Le texte de Perseus est plus explicite. On peut traduire le distique vers le français par : « quand Doris aux fesses de rose était à mon lit et j’ai écarté les jeunes jambes, je suis devenu immortel ». Une autre traduction possible est : « quand Doris aux fesses de rose était à mon lit et j’ai écarté la fraîche vulve, je suis devenu immortel ». Or, cette édition du texte n’emploie pas une métaphore. On peut traduire par « jambes » ou par « vulva », mais les deux options font référence directement à un organe du corps humain. Le texte grec disponible à Perseus est l’édition de 1916 de Paton.

![Épigramme 5.55 à l'édition de Paton[-@paton_greek_1916]](https://user-images.githubusercontent.com/79371444/225756857-46e2ae1f-be2b-4cc9-b721-527f3d5ae851.png)

On voit que l’édition de Perseus suit le texte établit par Paton à 1916. L’exception est l’adjectif *χλοερῖς*, qui semble être une variation du datif pluriel de l’adjectif *χλοερός,ά, όν*, traduit par « d'un vert tendre comme les jeunes pousses » d’où le sens de « frais, récent ». Par hasard ou intentionnellement, on ne peut pas déterminer, le logiciel qui a fait la numérisation du texte a créé une nouvelle version. La question devient plus intéressante lorsqu’on constate que Perseus est la source numérique la plus importante pour plusieurs textes grecs, dont l’*Anthologie grecque*. Par exemple, les textes grecs de la plateforme *Anthologia* ont été automatiquement récupérés de Perseus. Pourtant l’édition papier révisée du texte de Paton [-@paton_greek_2014] a un autre texte.

![Épigramme 5.55 à l'édition papier révisée de Paton[-@paton_greek_2014]](https://user-images.githubusercontent.com/79371444/225753521-b7148ff1-947d-4086-b07d-0b8a7be2136d.png)

Le distique à l’édition papier révisée de Paton [-@paton_greek_2014], et aussi à l’édition de Waltz [-@waltz_anthologie_2003], est : 

> Δωρίδα τὴν ῥοδόπυγον ὑπὲρ λεχέων διατείνας  
**ἄνθεσιν ἐν χλοερoῖς** ἀθάνατος γέγονα.^[Quando Doris de nádegas rosáceas estava em meu leito    
e eu estirei sua jovem flor, tornei-me imortal.]

On traduit ce distique vers le français par : « quand Doris aux fesses de rose était à mon lit et j’ai écarté la jeune fleur, je suis devenu immortel  ». Ce texte est moins explicite que le texte à Perseus. Le nom *ἅψος, ους (τό)*, qu'on a traduit par « jambe » ou « vulva », cède sa place à *ἄνθος, εος-ους (τὸ)*, « fleur ». Il n'y a plus un clair envoi au corps humain, et ce qu'on a est le polysémique fleur. Le nom *ἄνθος* élargit le sens du distique. La métaphore n'est pas hermétique et, avec un peu d'abstraction, on fait la association entre la fleur et la vulva. Mais la raison du choix est plus large que la facilité de comprendre la métaphore. L'idée de la fleur est un sujet fondamental pour l'*Anthologie grecque*. Étymologiquement la fleur est toujours dedans les anthologies, un recueil de belles fleurs. À la préface de Méléagre, chaque poète est une fleur. Aux épigrammes de Dioscorides au livre 5, le champ léxicale de la botanique est courant. Considérons la rose -- *ῥόδον,ου (τό)* -- et nous trouvons « fesses rosées » -- *ῥοδόπυγον* -- à 5.55 et « qui a la couleur de la rose » -- *ῥοδόχροα* --  à 5.56. Au livre 5, la fleur apparaît à des épigrammes de Rufin^[[5.19](https://anthologiagraeca.org/passages/urn:cts:greekLit:tlg7000.tlg001.ag:5.19/) et [5.74](https://anthologiagraeca.org/passages/urn:cts:greekLit:tlg7000.tlg001.ag:5.74/)], de Méléagre^[[5.144](https://anthologiagraeca.org/passages/urn:cts:greekLit:tlg7000.tlg001.ag:5.144/)], d'Asclépiades^[[5.158](https://anthologiagraeca.org/passages/urn:cts:greekLit:tlg7000.tlg001.ag:5.158/)], de Nossis^[[5.170](https://anthologiagraeca.org/passages/urn:cts:greekLit:tlg7000.tlg001.ag:5.170/)] et d'autres. Dans ce contexte, en tant que traducteur, il a fallu faire des choix entre les textes disponibles dans la langue source. La première décision prise fut de ne pas utiliser la forme χλοερῖς. En plus, on travaille avec le nom *ἄνθος, ους (τό)*.

<!--

> the anthology can be read as a form that gives a structure to narrative content in relation to a cultural, social, economic context, among others (p. 34) (Redefining the anthology)

> from its very origin the anthology form presented itself as a collection of separate, standalone stories. Narratives are therefore the nuclei of the anthology, which is primarily a form built on the assemblage of multiple forms. (p. 30) (Redefining the anthology)

-->

<!-- 

- Le *πορνικώτατος* veut dire que l'épigramme est le plus pornographique ? Un texte pornographique est plus explicite ? On doit choisir quels mots dans ce type de traduction?

- La traduction apporte des pertes, bien sûr, mais elle ouvre des possibilités aussi. En traduisant, le sens, les jeux phoniques, les allitérations de la langue source peuvent disparaître. Ainsi, le rôle du traducteur est aussi créer des nouveaux sens, sons etc. Le texte traduit est un objet en soi. Il a des liaisons avec le texte source, mais il autonôme aussi. Or, toute traduction est de la intertextualité.

- Le "*πορνικώτατον*" à 5.55.2. En portugais j'ai trouvé la solution "a maior putaria". Je joue avec la polysémie de "putaria" en portugais. Par contre, je n'ai pas de réponse pour le français

- peut être, l'épigramme 5.55 est pornikotaton parce qu'elle joue même avec la métaphore fondant de l'anthologie palatine: la métaphore de la fleur 

- La question de la censure apparaît lorsqu'on voit que, à Paton, l'épigramme est traduite vers le latin, pas le français. 

À propos du mot πυγή, Chantraine [-@chantraine_dictionnaire_1999] écrit qu'« il ne figure pas dans l'épopée ni dans la poésie lyrique ou tragique et Wackernagel, *Spr. Uni.* 225 sq., pense qu'il est vulgaire ». 
-->
## Bibliographie
