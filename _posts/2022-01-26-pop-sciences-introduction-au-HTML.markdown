L'application web que j'ai développée Pictalk, comme tout ce qui est sur le web, utilise HTML.

HTML [kézako](https://www.linternaute.fr/dictionnaire/fr/definition/quesaco/)  ?

HTML en langue anglaise signifie "HyperText Markup Language".  Je sais... ça ne nous aide pas bien plus... L'HTML est le language qui est utilisé pour structurer une page web et son contenu. Les premières pages HTML ressemblent pas mal à un document Word:

![](https://www.pierre-giraud.com/wp-content/uploads/2019/05/affichage-titres-h-html.png)

On dispose de titres, sous-titres, paragraphes et même d'images 🤩 ça ressemblait un peu à ça le web au début.

Dans ce court TP nous allons comprendre la syntaxe de ce language et l'utiliser pour faire un site web personnalisé qui nous présente 😎

## Les bases

Ne prenez pas peur !!! Tous ces caractères farfelus ne sont enfaite pas si difficiles à comprendre. 

On va commencer par la base de la base: 

HTML fonctionne avec des balises (ces `< > < />` trucs). La balise `<exemple>` indique le début d'un élément de type exemple  et `</exemple>` indique au contraire sa fin. Tout ce qui va se trouver entre ces balises est donc un élément de type *exemple*. 

`<exemple> Je suis un texte de type exemple </exemple>`

`<p> Je suis un texte de type paragraphe </p>`

```html
<titre>
Je suis un texte de type titre
<italique> Je suis un texte de type titre ET italique </italique>
</titre>
<p> Je suis un texte de type paragraphe et je ne suis pas un titre </p>
```

Cet exemple bien qu'il soit faux a du vous permettre de bien comprendre ce fonctionnement en balises.

Passons maintenant à quelque chose de plus concret: 

```html
<html>
<body>

<h1>Coucou Pop'sciences</h1>

</body>
</html>
```

La balise `<html>` dit tout simplement qu'il s'agit d'un code écrit en HTML. Il y a bien d'autres langages de programmation et il faut donc bien préciser dans quelle langage ont écrit à chaque fois !

La balise `<body>` (en français: *corps*)  est utilisée pour signaler le **corps** de la page web. C'est ici que l'on va placer le titre, les paragraphes, les images etc.

La balise `<h1>`  qui est l'abréviation de **heading** (en français: *titre*) nous permet d'écrire un titre. Pour écrire un titre plus petit il suffit d'incrémenter (faire monter) le chiffre à côté du `h` . Par exemple `<h6>` va être un titre très petit et `<h3` sera un titre de taille moyenne.

La brique de code d'au dessus va donner cela: 



![](/assets/img/2022-01-26-11-52-40-image.png)

 Cooooool pas vrai ? Vous devriez être chauds bouillants pour la suite dans ce cas.

## A vos claviers ! 👩‍💻 👨‍💻

[Cliquez ici pour démarrer]([Tryit Editor v3.7](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elements)) < --- Clique ici 🤗

Je vous présente

> Rrrrroulement de tambours

##### Notre éditeur de code pour ce TP

![](/assets/img/2022-01-26-14-44-15-image.png)

Bon pour la plupart du code écrit dans cette page vous devriez reconnaître une grande partie des balises.

Le bouton vert *run* sert à actualiser la page sur la droite avec le code de gauche.

Je vais vous donner trois petites tâches histoire de vérifier que vous avez-bien tout compris jusqu'à maintenant:

1. Changer le titre *Hello world* avec votre nom et prénom

2. Ajouter un titre de petite taille en dessous du titre avec votre nom et prénom (anciennement *Hello world*) indiquant le nom de votre établissement et votre classe

3. Enlever le paragraphe



Fini ? 🥳

Voici ma solution: 

```html
<!DOCTYPE html>
<html>
<body>

<h1>Alexandros SIDIRAS</h1>
<h3> INSA Lyon 6ème année </h3>
</body>
</html>

```

![](/assets/img/2022-01-26-14-40-36-image.png)

#### Les listes

Bon j'imagine que vous ne pouvez être résumé à juste votre nom prénom et année scolaire... 

Ajoutons vos activités favorites sur votre site web ! Dans un <u>paragraphe</u>, écrivez en dessous de votre année scolaire ce que vous aimez faire.

Moi c'était facile:

![](/assets/img/2022-01-26-14-41-52-image.png)

Le rendu n'est pas terrible non ? J'aimerais plutôt faire une ... LISTE !

Pour faire une liste il faut deux balises: Les balises `<ul>` signifiant "unordered list" (en français: *liste désordonnée*). Cette balise marque le début et la fin de la liste. Ensuite nous avons les balises `<li>` qui sont les acronymes de "list item" (en français: *élément de liste*) pour chaque élément que l'on veut mettre dans notre liste.

```html
<ul>
  <li>Manger de la salade</li>
  <li>Dormir</li>
  <li>Jouer</li>
</ul> 
```

![](/assets/img/2022-01-26-14-42-23-image.png)

Beaucoup mieux pas vrai ?

On peut même rajouter un titre avant la liste:

![](/assets/img/2022-01-26-14-43-07-image.png)

Pour vérifier que vous avez bien compris, <u>ajouter</u> une dernière chose que vous aimez faire.

#### Les liens

Et si on rajoutait un lien vers votre site favori ?

Pour cela il faut s'armer de la balise `<a>` . Voici un petit exemple:

```html
<a href="https://www.pictalk.xyz">Cliquez ici pour accéder à Pictalk</a>
```

A l'intérieur de la première balise `<a>` on place l'argument *href* qui définit l'url de notre site. Entre nos deux balises `<a>` et `</a>` on place le texte qui apparaîtra [comme ça]() .

#### Les images

Le site est un peu triste sans images... Vous avez envie d'en mettre une d'image aussi ?

Voici la balise qu'il nous faut:

```html
<img src="photo_de_chats.png" />
```

Ici la balise image a besoin d'un argument *src* , acronyme de <u>source</u> . Nous allons y mettre le lien vers notre image.

L'image de chats dans l'exemple ne va pas marcher car elle n'est pas accessible sur nos ordinateurs mais nous pouvons choisir une image disponible sur internet.

Une image de manchot vous va ? On va aller la chercher sur wikipedia a cette adresse: [Manchot empereur — Wikipédia](https://fr.wikipedia.org/wiki/Manchot_empereur)

#### ![](/Users/alex/Library/Application%20Support/marktext/images/2022-01-26-14-23-31-image.png)

Copiez le lien à la place de *photo_de_chats.png* et le tour est joué :

![](/assets/img/2022-01-26-14-43-47-image.png)

#### Défis

On commence a être bons en HTML n'est-ce pas ? Voici une petite liste de défis que vous êtes libres de faire si l'envie vous en prend 😎

- Mettre un smiley sur votre page

- Sachant que la balise pour mettre en gras un texte est: `<b>` Mettre en gras votre prénom

- L'attribut style permet de colorer (et plus) votre texte: `<h1 style="color: blue;">` va rendre le texte du titre de couleur bleue. Mettez un peu de couleur dans votre site !


