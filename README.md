## Le Html et le CSS : ##

Les balises **html**: http://41mag.fr/liste-des-balises-html5.
La prise de notes en Collectif : demande de commentaire → Vous pouvez mettre un commentaire en cliquant sur le bouton outils > commentaire ou clique droit, commentaire ou Ctrl + Alt +  M   
Pour rendre ce cour plus accessible :
	Le mettre en favories en cliquant sur l’etoile a droite de la barre d’Url.
Clique droit afficher la barre de fav ou Menu > Favoris > Afficher la barre de Favories

HTML:
Installer des guides dans atom
`install a package`
Indent guide improved
`Ouvrir Explorer > CePc > C: > Xampp > Htdocs`
	(C:\xampp\htdocs)
	`Créer un dossier nommé “DashboardXampp”`
	On déplace tous les fichiers et dossiers de Htdocs dans DashboardXampp  → Sert à rendre Htdocs exploitable.
	Dans Htdocs on crée un dossier:`Html-Css
Atom >File>open folder >C:\xampp\htdocs\Html-Css
Atom> sur le dossier Html-Css clik droit New file >index01.html`


**Dans index01.html:**   
```html
<!DOCTYPE Html>
<html>
<head>
</head>
<body>
</body>
</html>```

**! Indentation** : Manière de structurer les choses pour nous permettre de clarifier son travail.
nécessaire pour le travail à plusieurs
Permet de se repérer plus facilement dans la hiérarchie

Head  / Métadonnées : informations en arrière plan.
Informations fonctionnelles de la page
```<html>
  <head>
    <meta charset="utf-8"> 2
    <title></title> 1
  </head>
  <body>
    <style> 3
    </style>
  </body>
</html>```
Titre → 1
Type de caractères → 2
Feuilles de styles → 3   link rel="stylesheet" href="/css/style.css"
Frameworks → link / script ( entouré de <> )

**Body** : Contenu visible du site
**Header** : Informations de fonctionnement relatives au site (menu, barre de recherche, Log in, logo ou nom du site)
**Footer**: Bas de page (coordonnées, navigation secondaire, etc…)

**Div** : Bloc d’éléments→ permet de manipuler un ensemble d'éléments.

	<Section>
	<Article>	Ensemble d'éléments syntaxique permettant de manipuler un bloc.
	<Div>

	Ces 3 éléments représentent la même chose mais correspondent à des niveaux de représentation différents. section sera utilisé pour un grand ensemble, div pour un ensemble plus ou moin grand de type indéfinis et article pour un bloc contenant un article ( sous-titre, paragraphe.)

! ne pas oublier d’enregistrer et de recharger la page pour avoir un visuel de son code!

Supplements on sélectionne :
  (head)
  (/head)
  (body)
  (/body)
et on appuis sur la touche Tab ou shift Tab dans le head les métadonnée   
```<html>
      <head>
      </head>
      <body>
      </body>

      <meta charset="Utf-8">
      <meta name="twitter:" content="utf-8"
      <title>Index de demo</title>```

      ''' <meta name="Utf-8">'''  est une information sur le style de caractère utiliser sur le fichier.




Body (généralement en haut de la page)

dans body (exclusif au body)

```<html>
    <body>				
    <header>
    </header>
    <footer>
    </footer>
    </body>
           ```<html>

**Footer**(en bas de la page généralement avec les réseaux sociaux et contacts )

**nav** c’est pour naviguer dans les sites
La nav correspond au Menu, elle va servir à naviguer dans un site
div c’est un bloc d'éléments

```<html> <div class=""> ```</html>

on ouvre Xamp control pannel  / conflit avec skype !!
On autorise Apache qui un émulateur  qui exécutera le code d’Atom

**dans chrome on écrit localhost puis apres Html-Css et index01.hml**
http://localhost/Html-Css/index01.html


si besoin aller dans View et mettre Toggle Soft Wrap pour supprimer le texte qui depasse et tout voir.

 ```<html>
      <article>
      </article>
      <section>
      </section>
```
sont des balises qui ont la même utilisation, ils vont servir à sélectionner une grosse partie pour pouvoir la modifier.


exemple pour modifier la couleur du fond d’écran.#26A69A est un code couleur (background-color).
### Ne pas oublier le point virgule à la suite de la couleur ###

margin 50px 25 px
50 pour haut et bas et 25 pour gauche et droite
pour les marges ca marche de la manière suivante: haut, droite, bas, gauche
Pour centrer un texte: text-align: center;


Exemple de code CSS

 ```<html>
Insérer une image:
  <h1>Titre Principal</h1>
      <img src="img/xx.jpg" alt="Logo xx">
      ```

```<html>
Retoucher l’image:
      img{
        width:25%;
        height:auto;
      }
      header img{
        width:10%;
      }
      ```




Ctrl+Maj+/ pour mettre en pause une ligne (commenter une ligne)

Les commentaires :
	Les commentaires servent à noter des informations textuels au milieu du code sans perturber son exécution. Ils peuvent également servir à masquer une partie du code sans avoir à effacer son contenus.
	raccourcis clavier : Ctrl + Maj + /

commentaires en html : <!--  Zone de commentaire -->  →
commentaire en CSS : /*  Zone de commentaire   */
Déplacer un paragraphe d’un emplacement à un autre:
ctrl + flèche haut / bas.
Lexique :
Définitions générales Css :

 Class :
Éléments central du html / css, les classes permettent de sélectionner plusieurs éléments et de leur appliquer du style dans l’ensemble.
On définit à travers les classes, des propriétés communes à plusieurs éléments.

		Id :
	Identité de la balise, l’attribut ID permet d’identifier un balise précisément. Elle va nous permettre d’appliquer du style qui ne doit apparaître que sur cet élément.

		Typo / Font / Police de caractère :
	La police de caractère correspond à ce que l’on nomme en css la font-family.
Ce sont les visuels de caractère qui vont nous permettre de changer l’affichage du texte.

On peut les récupérer sur  google font ou Dafont et les charger via un système de balise <link> ou directement dans le css via ce que l’on appel les media queries

Terminologies Html / Css :

head : Le head contient toutes les <meta> ou métadonnée. Ce sont les informations structurelles de la page qui n'apparaîtront pas directement à l'écran mais qui sont nécessaire pour le bon fonctionnement de la page.

body : Représente le corps de la page HTML.(un seul par document)

header : Partie haute de la page web/html. Contient en général le titre et la navigation

	link: balise servant à charger du contenus CSS -- police + feuille de style

<p> définit un paragraphe.
<span : pour sélectionner une partie du texte que l’on veut modifié.
<strong / <b : affiche un texte en gras
<u : souligne un texte
<i : affiche le texte en italique
<em : italique ou gras pour un texte ( dépend du navigateur )
<div :définit une division ou une section,appelé aussi calque

.container : la classe container va nous servir à définir un espace donné qui contient les données dans une partie de la page. C’est une classe que l’on définit soi même.

attributs : les attributs sont les informations notées

float → left / right:
Mettre une image en habillage du texte
positionner un élément à droite ou à gauche d’un autre.
inconvénients : sort du flux → certaines propriétés ne fonctionnent pas et les éléments ne sont plus relatif entre eux

	font-family :change la police de caractères

	**display** :
		inline : aligne les éléments les uns à la suite des autres.
		block : réserve tout l’espace disponible sur la ligne, illustré par une marge qui remplis l’espace.
		inline-block : lorsque des éléments inline-block sont côte à côte, ils se mettent à la suite et ensemble, forment un block.
