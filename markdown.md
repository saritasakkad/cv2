<!-- c'est deux méthode permet d'affiché une image -->
# Markdown ça doit vous parlez ! ![alt text]( https://github.com/saritasakkad/cv2/blob/master/markdown_128.png "Logo Title Text 1")



# Je voie certain arriver ! ![alt text]( https://github.com/saritasakkad/cv2/blob/master/non.png "Logo Title Text 1")   


 ## Non ce n’est pas le mcdo !  
![alt text][logo]

[logo]: https://github.com/saritasakkad/cv2/blob/master/images.png
"Logo Title Text 2"


### Certes Markdown, il est alléger et délicieux à employer, ça c'est vrai !
***


Introduction: Markdown c'est quoi?
Markdown est un language de balisage léger, une sorte de cousin du HTML. C'est à dire que toute balise HTML fonctionne dans un fichier Markdown. Toutefois, si vous voulez créer un élément HTML dans un fichier Markdown, vous ne pourrez pas utiliser du Markdown à l'intérieur de ce dernier.. Ce language à pour but d'être léger et facile à lire en soi. Il se base sur le balisage des e-mails. [plus d'info] (https://fr.wikipedia.org/wiki/Markdown)

Le Markdown est implémenté de différentes manières, selon le parser.
Ce guide va alors tenter de trier les fonctionnalités universelles de celles
spécifiques à un parser.  

# syntaxe
## Headers
### option 1
Le nombre de dièses (#) indiquent le niveau du titre. 1# = titre de niveau 1
# 1# - titre 1 <h1>
## 2# - titre 2 <h2>
### 3# - titre 3 <h3>
#### 4# - titre 4 <h4>
##### 5# - titre 5 <h5>
###### 6# - titre 6 <h6>

###option 2
Alternative pour Titre de niveau 1&2: le tiret simple ou double en dessous du texte

<!-- Ceci est un h1
     =============

     Ceci est un h2
     -------------
-->
## Styles de base
On peut facilement rendre un texte "gras" ou "italique" en Markdown:
par l'utilisation des asterixes* et underscore_ autour du texte

\*Ce texte est en *italique* Grace à une asterixe\*
\__Celui-ci_ grace à un underscore.\_

\*\*le **gras** s'indique par deux asterixes.\*\*
\_\_Ou deux underscore\_\_

\*\*\* ***Ce texte a les deux styles.*** \*\*\*
**_Pareil ici_**
*__Et là!__*

Pour le texte barré on utilise la vague:

\~\~ ~~Ce texte est barré avec strikethrough.~~ \~\~

##Paragraphes

Les paragraphes sont séparés par des lignes de vides.

Ceci est un paragraphe. Le paragraphe 1.

Maintenant je suis dans le paragraphe 2.
Je suis toujours dans le paragraphe 2!


Puis là, eh oui, le paragraphe 3!

Bien sur la balise HTML <br/> fonctionne aussi.

## Citations
Pour avoir un 'Blocs de Citations' il suffit d'ajouter le caractère >

> Ceci est une superbe citation. Vous pouvez même
> revenir à la ligne quand ça vous chante, et placer un `>`
> devant chaque bout de ligne faisant partie
> de la citation.
> La taille ne compte pas^^ tant que chaque ligne commence par un `>`.

> Vous pouvez aussi utiliser plus d'un niveau
>> d'imbrication!
> Classe et facile, pas vrai?

## Les listes
### Non-ordonnées
 Sont indiquées par des asterixes* des plus+ ou des moins- en début de ligne.
\* Bananes
\* lait
\* Avoine

ou

\+ Cacahouette
\+ Pistache
\+ Encore un item

ou

\- Item
\- Item
\- Un dernier item

###Ordonnées
\1. element1
\2. element2
\3. element3

1. Python
2. ruby
3. SPSS

Il est possible de se passer du numérotage, markdown le fera pour nous. Bien que cela perde en clareté.

1. element1
1. element2
1. element3

### imbrications
Il est également possible de créer des sous-listes:

\1. Item un
\2. Item deux
\3. Item trois
\* Sub-item
\* Sub-item
\4. Item quatre

### listes de tâches
ou des listes de tâches avec des cases à cocher:

Les [ ] ci dessous, n'ayant pas de [ x ],
deviendront des cases à cocher HTML non-cochées.

- [ ] Première tache à réaliser.
- [ ] Une autre chose à faire.
La case suivante sera une case à cocher HTML cochée.
- [x] Ça ... c'est fait!

## Blocs de Code
Pour marquer du texte comme étant du code, il suffit de commencer
chaque ligne en tapant 4 espaces (ou un Tab)

\  echo "Ça, c'est du Code!";
\  var Ça = "aussi !";

<!-- L'indentation par tab ou série de quatre espaces
fonctionne aussi à l'intérieur du bloc de code -->

    my_array.each do |item|
       puts item
    end

<!-- Des bouts de code en mode 'inline' s'ajoutent en les entourant de ` -->

La fonction `run()` ne vous oblige pas à aller courir!

<!-- Via GitHub Flavored Markdown, vous pouvez utiliser
des syntaxes spécifiques -->

\`\`\`ruby
<!-- mais enlevez les backslashes quand vous faites ça,
gardez juste ```ruby ( ou nom de la syntaxe correspondant à votre code )-->
def foobar
puts "Hello world!"
end
\`\`\` <!-- pareil, pas de backslashes, juste ``` en guise de fin -->

<!-- Pas besoin d'indentation pour le code juste au dessus, de plus, GitHub
va utiliser une coloration syntaxique pour le langage indiqué après les ``` -->

##Ligne Horizontale

Pour en insérer une, utilisez trois ou plusieurs astérisques ou tirets,
avec ou sans espaces entre chaque un.

\*\*\*
\-\-\-
\- \- \-
\*\÷\*\*\*************

##Liens
Il suffit de mettre le texte du lien entre [ ], l'url entre ( ).

\[Clic moi!\]\(http://test.com/\)

Pour ajouter un attribut Title, collez le entre guillemets, avec le lien.


[Clic moi!](http://test.com/ "Lien vers Test.com")

Les Liens Relatifs marchent aussi

[En avant la musique](/music/).

Les liens façon "références" sont eux aussi disponibles en Markdown

[Cliquez ici][link1] pour plus d'information!
[Regardez aussi par ici][foobar] si vous voulez.




Le titre peut aussi être entouré de guillemets simples,
entre parenthèses ou absent. Les références peuvent être placées
un peu où vous voulez dans le document, et les identifiants
(link1, foobar, ...) quoi que ce soit tant qu'ils sont uniques

Il y a également le "nommage implicite" qui transforme le texte du lien
 en identifiant

[Ceci][] est un lien.

mais ce n'est pas beaucoup utilisé.

## images
Pour les images, la syntaxe est identique aux liens, sauf que précédée
 d'un point d'exclamation!

![Attribut ALT de l'image](http://imgur.com/monimage.jpg "Titre optionnel")

Là aussi, on peut utiliser le mode "références"

![Ceci est l'attribut ALT de l'image][monimage]



##Divers
Liens Automatiques

<http://testwebsite.com/> est équivalent à :
[http://testwebsite.com/](http://testwebsite.com/)

Liens Automatiques pour emails

<foo@bar.com>

##Escaping
Il suffit de précéder les caractères spécifiques à ignorer par des backslash \

Pour taper *ce texte* entouré d'astérisques mais pas en italique :
Tapez \*ce texte\*.

## Tableaux
Les Tableaux ne sont disponibles que dans le GitHub Flavored Markdown
 et c'est ce n'est pas super agréable d'utilisation.
 Mais si vous en avez besoin :

| Col1 | Col2 | Col3 |
| :----------- | :------: | ------------: |
| Alignement Gauche | Centé | Alignement Droite |
| bla | bla | bla |

ou bien, pour un résultat équivalent :

Col 1 | Col2 | Col3
:-- | :-: | --:
Ough que c'est moche | svp | arrêtez
