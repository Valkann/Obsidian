---
share: true 
category: source
Alias:
---
Date:: 2022-11-21-Mon
Week:: 47
Rating::
Summary:: 
Author::
Source:: 
Type:: #SN/
Status:: 
MOC::
Projet:: 
Tags:: 

# Obsidian, bien plus qu’une prise de notes


***

## Notes

Obsidian, bien plus qu’une prise de notes...

Depuis quelques mois, des révolutions sont en cours dans les logiciels de saisie des notes. A ce titre on parle beaucoup de Notion qui permet d'aller au delà de la prise de notes mais il y a aussi Roam, Bear ou Remnote. Je vous invite à découvrir la puissance d’Obsidian.

<img width="701" height="234" src="../_resources/64d8904a867a46429befb9bc0f81d3ce.png"/>

Personnellement je préfère utiliser un système de notes permettant d'obtenir une vue graphique des liens entre les différents documents afin de mieux les analyser. C'est peut-être parce que je suis un adepte du mind-mapping. Il faut aussi que la gestion du stockage de ces notes ne soit pas imposée. A ce titre ~~j'utilise~~ j'utilisais l'outil Open Source Trilium Notes : [https://github.com/zadam/trilium](https://href.li/?https://github.com/zadam/trilium). Mais la complexité de celui au fil des versions a rendu son utilisation complexe. La découverte d[‘Obsidian](https://href.li/?https://obsidian.md/) il y a quelques mois, m'a convaincu d’adopter cet outil même s’il n’est pas OpenSource. 

[Obsidian](https://href.li/?https://obsidian.md/) est téléchargeable gratuitement et sans limitation. La société qui produit l’outil se rémunère en permettant de publier les notes créées sur internet. Cet article n’est pas une formation sur l’outil mais simplement un retour d'expérience de mon utilisation.

Quand vous prenez en main Obsidian, vous trouverez peut-être austère l’interface. Je veux plutôt dire “minimaliste”. Obsidan se veut simple, rapide et aller à l'essentiel. Donc oubliez les barres d'outils, les éditeurs complexes, tout se fait avec des raccourcis claviers (que vous pouvez d’ailleurs customiser). Vous pouvez aussi changer l’interface, il existe de nombreux thèmes qui, en plus de modifier l’aspect visuel, vous permettent de choisir le style de votre note si vous souhaiter l’exporter en PDF. Chaque note que vous rédigez est au format markdown. Vous pouvez facilement passer du mode édition en visualisation. Même si je ne suis pas un grand spécialiste du Markdown son utilisation “de base” permet de gagner en rapidité. 

<img width="701" height="758" src="../_resources/0779e8f64b314fbca77f06513d51872a.jpg"/>

Je vous livre ici les syntaxes que j'utilise :

Pour faire des titres il suffit de mettre un # devant chaque titre suivant la hiérarchie désirée :
\# H1
\## H2
\### H3

Pour mettre en gras vous encadrez le texte de 2 * :
\*\*texte en gras\*\*

Pour surligner un texte remplacer les * par des =
==Surligner==

Pour mettre en Italic, une seule *
\*texte en italique\*

Pour faire un “bloc de citation” il suffit de commencer la ligne par >
\> blockquote

Pour faire des listes numérotées, rien de plus simple :
1\. Premier titre
   1\. Sous titre
   2\. Sous titre
2\. Second titre
3\. Troisième titre

Des listes simples, c’est encore plus simple : 
\- Premier
\- Deuxième
\- Traisième

Pour mettre du code :
\`code\`

Pour tracer une ligne horizontale :
\*\*\*

Pour faire des cases à cocher : 

> \- \[x\] Choix Un  
> \- \[ \] Choix Deux
> \- \[ \] Choix Trois

Pour mettre en forme d'un tableau (la 2ème ligne indique le format de la colonne) :

> | Syntax      | Description | Test Text     |
> | :—        |    :—-:   |          —: |
> | Header      | Title       | Here’s this   |
> | Paragraph   | Text        | And more      |

Ajouter un commentaire non visible en visualisation :
%%commentaire%%

Si vous désirez aller plus loin, il existe de nombreux sites et ouvrages disponibles pour approfondir vos connaissances.

<img width="701" height="486" src="../_resources/1963a4fc5a104fdf8328678fb2cc009a.jpg"/>

Chaque note sera donc un fichier markdown (.md) stocké dans le dossier de votre projet (Vault). Il est possible de créer des sous-dossiers dans ce Vault pour structurer votre travail (même si les liens suffisent).

Dés que je crée un nouveau projet, je règle le paramétrage de l’éditeur. L’objectif est d’aller vite et de me consacrer à l’essentiel. Par exemple j’active les raccourcis vim, si vous n’êtes pas un connaisseur de vim je vous invite d’aller sur [https://www.vimgolf.com/](https://href.li/?https://www.vimgolf.com/). Je crée éventuellement de nouveaux raccourcis clavier puis je choisis les plugins que je vais utiliser.

Obsidian fonctionne avec de nombreux plugins permettant d'accroître les possibilités. La configuration des plugins est propre à chaque projet. Il est difficile ici d'évoquer tous les plugins “officiels” mais également ceux de la communauté. Car c’est aussi le point fort d’Obsidian, une communauté très active pour améliorer continuellement l’outil à l’aide de plugins OpenSource. 

J’ajoute ensuite 2 sous-dossiers dans mon projet :

\- Asset : qui va contenir tous les documents externes (images, documents, média…) ou je copie éventuellement mes ressources locales.
\- Template : qui va contenir des modèles de notes (pensez à activer le plugin puis configurer pour qu’il pointe vers ce dossier).

![image](../_resources/a647c3a617ec4b11bb63fafedb436e64.png)

Je commence par créer un document template qui va contenir des méta-données. Pour cela je crée une nouvelle note dans le répertoire template et au début de la note, je crée un bloc délimité par 3 tirets :

> —
> Metadonnées
> —

Chaque métadonnée est composé d'un nom (label) suivi de 2 points, au moins un espace et la valeur désirée.  L’intérêt est lorsqu’on applique ce template à une note, on a déjà des métadonnées que l’on peut compléter, par exemple :

> —
> Date: {{date}}
> tags: superman, batman
> Alias:  superhero
> —

-\> Date : Date de création de la note (le format est paramétrable dans la configuration du plugin)
-\> Tags : mots clés de la note
-\> Alias : Autre nom de la note
Vous pouvez créer autant de métadonnées que cela vous semble utile.

Evidemment, en prévisualisation ces métadonnées ne seront pas visibles à moins que vous modifiez les préférences de l'éditeur mais elles restent “interrogeables” par des recherches.

Une fois le (ou les) modèle(s) définis, je peux prendre mes notes en appliquant les templates définis. En tant que “keyboard Ninja”, j’utilise certains raccourcis comme :

Ctrl+N : Nouvelle note
Ctrl+O : Sélecteur rapide => Non de la page de la note
Ctrl+E : Previsualisation / Édition

Et si vous ne savez plus, faites Ctrl+P pour la liste des commandes.

Pour faire un lien vers une autre note de votre projet, commencez à taper :

\[ \[ => Vous pouvez alors naviguer vers les différentes notes.

Pour insérer une image du répertoire asset : ! \[ \[ 
Cette syntaxe sert aussi en visualisation d’insérer aussi une autre note.

Si vous désirez faire un lien externe : \[nom du site\](https://labonnedonne.fr/post/644122684651945984/[https://obsidian.md](https://href.li/?https://obsidian.md))

Il existe beaucoup plus de possibilités pour gérer les liens (consultez l’aide) et de nombreux plugins vous automatisent les créations de notes et les liens.

Un autre avantage d’obsidian est la possibilité de créer des liens internes vers des notes qui n’existent pas encore. Cela permet de les représenter graphiquement et d’obtenir des résultats dans les recherches globales. Il sera toujours possible de cliquer sur ce lien pour créer physiquement la note. Pour vous illustrer mon propos et vous montrer les possibilités d’obsidian dans l’analyse de données, je vais vous montrer comment Obsidian peut répondre aux questions suivantes :

Qui entre Jon Favreau et Joss Whedon a réalisé le plus de films Marvel ? Qui entre Chris Evans, Robert Downey Jr., Chris Hemsworth, Scarlett Johansson et Mark Ruffalo a joué le plus dans des films Marvel ?  

<img width="701" height="394" src="../_resources/6b43f7175cfd416faf54796261b3d234.jpg"/>

Certes vous trouverez ces renseignements sur internet mais il faudra consulter différentes pages, puis comparer et noter les résultats. Obsidian peut vous faciliter la vie. On va en premier utiliser la base de Wikipedia pour extraire les données puis convertir ces données au format markdown pour finalement les analyser. Rassurez vous c’est très facile. 

Le moteur de Wikipedia est mediawiki. Par défaut il existe des fonctions pour extraire des pages notamment cette URL :

> [https://fr.wikipedia.org/wiki/Special:Exporter/Nom\_de\_la_page](https://href.li/?https://fr.wikipedia.org/wiki/Special:Exporter/Nom_de_la_page)

Pour convertir les fichier de mediawiki vers markdown, on va utiliser [pandoc](https://href.li/?https://pandoc.org/).
Donc en une ligne on pourra extraire et convertir :

> pandoc -f mediawiki -t markdown -s [https://fr.wikipedia.org/wiki/Special:Exporter/Nom\_de\_la_page](https://href.li/?https://fr.wikipedia.org/wiki/Special:Exporter/Nom_de_la_page) -o nom\_de\_la_page.md

On crée un répertoire puis on récupère toutes les données de wikipedia des films Marvel, exemple :

pandoc -f mediawiki -t markdown -s 'https://fr.wikipedia.org/wiki/Special:Exporter/Iron\_Man\_(film)’ -o 'Iron\_Man\_(film).md’

Une fois terminé, on va ouvrir un nouveau projet dans Obsidian en pointant vers ce répertoire et par magie, en visualisant le graph du projet, on découvre tous les lien (même si on n’a importé que les notes des films).

<img width="701" height="434" src="../_resources/dd82854b88234268a386168ce5f1ba8d.png"/>

Dans cette représentation ci-dessus, les “gros” points représentent les notes correspondantes aux films Marvel récupérés. Tous les autres points sont des noeuds créés automatiquement. Ainsi même si les notes ne sont pas présentes, obsidian nous présente tous les liens. On peut donc facilement “naviguer”. Si on ne veut voir que les liens qui pointent vers une note existante physiquement, il suffit de jouer sur les filtres du graph. 

<img width="701" height="620" src="../_resources/142b530a06e4447898e866d0ecf29d01.png"/>

Bon répondons maintenant à la première question. Le plus simple (mais ce n’est pas la seule solution possible) est de définir des “groupes de couleurs” qui se base sur une recherche, le résultat est flagrant :

<img width="701" height="601" src="../_resources/217590f093b743b69bd6c83d5ce18db1.png"/>

Pour la deuxième question nous allons utiliser une autre méthode (mais il en existe beaucoup autres !). On va utiliser la recherche d’Obsidian pour chaque acteur. Nous obtenons le nombre d’occurrences dans chaque note :

![image](../_resources/e38bf4c3d0bf4edf81435aaaecadccb3.png)

On copie le résultat en transformant chaque élément par un lien et en numérotant la liste (tout cela automatiquement). Puis on crée une nouvelle note avec le nom de l’acteur (que l’on peut  placer dans un sous répertoire) en collant le résultat obtenu :

<img width="701" height="320" src="../_resources/d954fffbc49a4e53815e7b380b3f4d65.png"/>

Il ne reste plus qu’à utiliser les possibilités de division des fenêtres pour obtenir les résultats. A noter que chaque lien est cliquable ce qui peut permet de naviguer dans les différents films pour rebondir sur d’autres acteurs…

<img width="701" height="650" src="../_resources/cc27b5661cf04e7792dcbc3df8b1a8d4.png"/>

Maintenant supposons qu’au lieu des 5 acteurs, on est choisi 20 acteurs qui ont tourné dans des films Marvel. Si je vous demande rapidement qui parmi ces acteurs a joué dans les films “Iron Man” ? Rien de plus simple, on clique sur les notes des films Iron Man et avec la vue graphique on obtient les résultats (ici avec mes 5 acteurs) :

<img width="701" height="526" src="../_resources/253f16770f8c42c3aa6133ed27d2a93a.png"/>

Evidemment tous les liens sont bi-directionnels et en jouant sur la profondeur on peut visualiser tous les éléments liés.

Par ce petit exemple vous comprenez qu’Obsidian est bien plus qu’un logiciel de prise de notes. Il me sert pour l’analyse des données et avec des plugins les possibilités sont infinies (Query d’analyse en SQL, extraction et la création de notes automatiques, timelines, analyse des meilleurs chemins, augmentation des possibilités de recherches, synchronisation avec un dépôt git…).

Maintenant imaginez les possibilités d’analyse avec le réseau “linkedin” et la puissance qui vous est offerte pour découvrir rapidement les meilleurs interlocuteurs pour cibler un objectif…

J'espère que ce petit article vous aura permis de prendre conscience des avantages d'Obsidian et d’essayer cet outil. Le seul reproche (si c'est un reproche) de l'outil est les fréquentes mises à jour qui nécessitent de suivre les changelogs pour connaître les améliorations ou changements apportés. Sous Linux les dernières versions sont disponibles sous 3 formats : Appimage, Snap et Flatpak.

Je vous invite aussi de consulter une autre présentation en Français qui montre une autre utilisation d’Obsidian :
[https://publish.obsidian.md/opspl-wiki/Table+of+Contents](https://href.li/?https://publish.obsidian.md/opspl-wiki/Table+of+Contents)

Il existe aussi un clipper :
[https://jplattel.github.io/obsidian-clipper/](https://href.li/?https://jplattel.github.io/obsidian-clipper/)