# Spécifications fonctionnelles et techniques

STATUT : EN COURS

[Les bonnes pratiques du web]: https://checklists.opquast.com/fr/oqs-v2
[First Step]: https://checklists.opquast.com/fr/accessibility-first-step
[Second Step]: http://checklists.opquast.com/fr/accessibility-second-step

## Sommaire

- [Généralités](#généralités)
	- [Vie privée](#vie-privée)
	- [Transparence](#transparence)
- [Fonctionnalités](#fonctionnalités)
	- [Le compte](#le-compte)
	- [L'item](#litem)
	- [La liste](#la-liste)
	- [Le contact](#le-contact)
	
## Généralités

### Vie privée

Toutes les données de l'utilisateur peuvent être modifiées ou supprimées à sa demande.

### Transparence

Une section "À propos" lie l'application, le site et le bookmarklet à sa conception open source.

Le site fait l'objet d'une déclaration publique Opquast référencée depuis la section "À propos" sur les référentiels suivants :
- [Les bonnes pratiques du web][]
- [First Step][] (Premier pas vers WCAG 2.0 : erreurs)
- [Second Step][] (Second pas vers WCAG 2.0 : risques)


## Fonctionnalités

### Le compte

#### Création

La création du compte peut se faire :
- depuis l'application
- depuis le site web

La création du compte nécessite :
- un identifiant (pseudonyme ou e-mail)
- un mot de passe

La création de compte passe par un mail de confirmation.

#### Gestion du compte

##### Connexion au compte

La connexion au compte propose un processus de renouvellement de mot de passe via envoi de mail.

Toutes les informations du compte à l'exception de l'identifiant peuvent être changés autant de fois que l'utilisateur le souhaite.

##### Gestion des données du compte

Un compte =
- Données obligatoires
	- identifiant / mot de passe
- Données facultatives
	- adresse(s) postale(s)
	- paramètres
		- visibilié par défaut
		- adresse par défaut
		- devise par défaut
		- notifications
		- notification par défaut
		- notifications à propos de SpoiledPeople

###### Export des données du compte

L'ensemble des données du compte sont exportables dans un format ouvert et courant (à défaut dans un format ouvert et dans un format courant)

###### Suppression du compte

Le compte peut-être supprimé à la demande de l'utilisateur.
Un avertissement et une demande de confirmation sont affichés avant de valider l'opération.
En cas de suppression de compte, toutes les informations du compte sont supprimées de la base de données.

### L'item

- Données obligatoires :
	- titre et/ou image
- Données facultatives :
	- description
	- prix
	- quantité souhaitée
	- statut

#### Ajout d'un item

L'ajout peut se faire :
- via la galerie du mobile
- via l'appareil photo du mobile
- via une image téléchargée depuis le navigateur
- via URL copiée-collée
- via le scan d'un code-barre
- via le bookmarklet
- manuellement

Quel que soit le mode d'ajout, la totalités des informations sont accessibles et modifiables manuellement.
Quel que soit le mode d'ajout, l'enregistrement de l'item est soumis à un bouton de validation que l'utilisateur doit activer.

Les données attendues sont :
- Données obligatoires :
	- titre et/ou image
- Données facultatives :
	- description
	- prix et devise
	- quantité

##### Ajout via la galerie du mobile

Permet d'aller choisir dans les photos de la galerie du mobile.

##### Ajout via l'appareil photo du mobile

Ouvre l'application appareil photo du mobile.
Une fois la photo prise, elle est affichée avec une confirmation d'utiliser cette photo. 
Un autre choix est possible : prendre une aute photo.

Tout du long, on peut annuler via la navigation native du terminal.

##### Ajout via une image téléchargée depuis le navigateur

##### Ajout via URL copiée-collée

L'élément \<title\> de la page de destination est récupéré et placé par défaut dans le champ de titre de l'item.

L'élément \<meta description\> de la page de destination est récupéré et placé par défaut dans le champ de description de l'item.

L'ensemble des images sont récupérées et proposées à l'utilisateur pour le champ image de l'item.
Par défaut, c'est la première image trouvée qui est retenue. L'utilisateur peut choisir de ne retenir aucune image.

##### Ajout via le scan d'un code-barre

##### Ajout via le bookmarklet

##### Ajout manuel

Un item peut-être rajouter via une édition manuelle depuis l'application ou depuis le site web.

#### Formulaire d'un item (ajout ou édition)

##### Titre 

Le titre est obligatoire si l'image n'est pas renseignée.

##### Image

L'image est obligatoire si le titre n'est pas renseigné.

##### Description

La description est facultative.

##### Prix

Le prix est facultatif.

##### Devise.

La devise est affichée par défaut avec la valeur indiquée dans les paramètres du compte.
Elle peut être modifiée lors du remplissage du formulaire.

##### Quantité

La quantité est facultative.

### La liste

#### Création d'une liste

Les données attendues :
- Données obligatoires :
	- nom
	- visibilité (privée / partagée / publique)
- Données facultatives :
	- date de l'événement
	- adresse liée
	- notification
	- un ou des contacts attachés

### Le contact
