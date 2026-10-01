# Cahier des charges – Application de gestion de stock et de commandes d’une entreprise d’électricien

## Introduction
Powerbase – l’application de gestion de commandes internes.
J’ai choisi ce projet car j’ai voulu trouver une solution pour la gestion de commandes internes d’une société d’électricité, qui pour le moment présente quelques difficultés dans le processus de commandes internes. 
On m’a parlé de plusieurs scénarios problématiques, que je voudrais résoudre à travers mon application. J’ai choisi d’en faire une application qui est utilisable par plusieurs sociétés car j’ai entendu dire que plusieurs sociétés présentent les mêmes problèmes.


## Modifications attendues
Puisque le projet est déjà en cours, je cite ci-après les modifications que j’aimerais apporter à mon projet.
J’aimerais bien :
-	ajouter une interface qui pourrait contenir toutes les données des différents clients;
-	faire une réorganisation complète de l’interface électricien en centralisant plus les besoins des éléctriciens;
-	prévoir des options d’abonnement;
-	prévoir des options d’abonnement sélectionnables dans la partie société de l’interface du manager;
-	faire des fonctionnalités « Recommander une ancienne commande »;
-	faire des fonctionnalités « Créer des commandes » à base d’une ancienne commande;
-	ajouter une route de base /;
-	améliorer l’interface register pour une utilisation plus facile;
-	ajouter la possibilité pour les électriciens d’ajouter des produits à leurs favoris;
-	ajouter des filtres pour la recherche de produits des électriciens (technique à déterminer);
-	ajouter des images aux produits commandés pour améliorer la réperabilité;
-	ajouter une section pricing aux pages publiques;
-	améliorer le flux utilisateur;
-	faire une complète refonte du design pour les différentes interfaces;
-	donner plus de cohérence aux différents éléments des interfaces;
-	réorganiser les pages publiques;
-	améliorer l’hierarchie des informations sur les différentes interfaces;
-	ameliorer les problèmes d’espacement et d’interligne;
-	améliorer le vocabulaire utilisé et l’adapter le plus possible au vocabulaire utilisé dans les sociétés d’électricité;
-	rendre plus visible la différence entre éléments clickables et non;
-	rendre les cartes du dashboard (manager et magasinier) clickables;
-	faire un design cohérent des différents éléments (inputs, effets hover, etc.);
-	améliorer les mentions légales;
-	faire une présentation et une organisation différentes des contenus des interfaces différentes (public, magasinier, éléctricien et manager);
-	ajouter des icones pour faciliter la réperabilité;
-	améliorer les effets hover et repenser leur utilisation pour certains éléments;
-	renommer patron en manager;
-	renommer projets en chantiers;
-	renommer produit en matériel;
-	ajouter du contenu sur certaines pages;
-	pour les commandes repenser la liste de recherche (pas très lisible et difficilement utilisable pour l’instant).


## 1. Contexte général
Ce projet vise à concevoir une application Web permettant à la société de :
-	passer des commandes,
-	suivre le statut des commandes,
-	créer, modifier des chantiers,
-	gérer les commandes,
-	gérer le stock,
-	rechercher et trier des produits,
-	gérer les différents utilisateurs,
-	rappeler les électriciens de passer leur commande.

Il y a également une page publique pour présenter l’application auprès du public avec les différentes formules d’abonnement. 
  
   
## 2. Personas et scénarios
### 👨🏻‍💼 Marc Arimont - Administrateur / Patron  
**Âge :** 41 ans  
**Profil :** patron depuis 16 ans  
**Compétences numériques :** normales  

#### 🎯 Objectifs
-	gérer les utilisateurs (électriciens, magasiniers),
-	avoir un système fiable et organisé,
-	augmenter la productivité,
-	assurer un flux de travail fluide entre les équipes.

#### 😣 Frustrations
-	pas de système qui permet de relier les commandes au stock,
-	pas de système qui permet automatiquement de faire des rappels de commande,
-	perte de temps par le magasinier car électriciens oublient de passer la commande et donc perte d’argent,
-	pas de gestion par chantier.

#### 📌 Besoins
-	Dashboard clair,
-	gestion des rôles simples,
-	système qui permet aux employés de passer des commandes plus facilement,
-	système facile à utiliser pour tous les employés et travailleurs.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Marc a engagé un nouveau électricien. Il doit lui créer un compte sur l’application. Il peut renseigner son nom et prénom, son rôle (électricien), son numéro de téléphone de tavail et son numéro de téléphone privé. Il peut aussi ajouter dans sa fiche son adresse. Après validation de la fiche du nouveau électricien, celui-ci reçoit un email de bienvenue avec une invitation à définir son nouveau mot de passe.
Le logiciel lui permet de faire les mêmes manipulations pour un magasinier.

##### 🤔 Scénario 2
Le magasinier a constaté qu’il y a du matériel défectueux dans le stock. Il fait une liste du matériel pour Marc et envoie la à Marc, qui doit vérifier la liste et se renseigner sur des remplacements, ou autres solutions. Entre temps, le magasinier a retiré ce matériel du stock pour ne pas rencontrer des problèmes lors de la préparation des commandes.
Marc a réçu la liste de son magasinier par email. Marc vérifie d’abord cette liste. Ensuite il prend contact avec les délégués pour des produits de remplacements. Un des délégués se rend sur place et apporte des remplacements pour certains produits. Après le rendez-vous, Marc se rend dans l’onglet matériel et change le stock de ses produits et apporte les produits chez son magasinier.

##### 🤔 Scénario 3
Franco travaille depuis 15 ans pour Marc. Il a 54 ans et il a demandé à son patron Marc, s’il pouvait changer de job au sein de sa société. Marc lui a proposé un job au magasin qui vient de se libérer, car Franco a de bonnes connaissances du matériel et car le travail est moins exigeant pour ses genoux.
Marc a déjà créé une fiche pour Franco, mais il est enregistré en tant qu’éléctricien. Il doit changer le rôle de Franco pour que Franco ait accès aux fonctionnalités du stock.

---

### 🧑🏽‍🔧 Pierre Simon - Electricien
**Âge :** 34 ans  
**Profil :** electricien dans la société depuis 4 ans  
**Compétences numériques :** normales   
**Objectif principal :**  rechercher facilement des produits, les ajouter à la commande et passer une commande.  

#### 🎯 Objectifs
-	rechercher le matériel,
-	reconnaître facilement le matériel grâce à des images,
-	ajouter les produits à la commande,
-	augmenter ou diminuer les quantités du matériel,
-	retirer du matériel de la commande,
-	passer une commande attachée à un chantier.

#### 😣 Frustrations
-	oublie souvent de passer sa commande. Pas de système qui permet automatiquement de faire des rappels de commande,
-	pas de système pour choisir des produits sur internet (appel téléphonique ou mail),
-	commande par email ou téléphone. Pas d’images lors de la commande. Erreurs fréquents.

#### 📌 Besoins
-	page de produits claire,
-	barre de recherche et fonctionnalités de tri,
-	image qui illustre le produit,
-	description ou données clées sur la fiche de détail du produit,
- favoris pour retrouver les produits qu’il utilise régulièrement.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Pierre est sur un chantier. Il lui manque du matériel pour terminer son travail. Il se connecte à l’application et il se rend sur la page du matériel de l’application. Il recherche le matériel qu’il a besoin et il l’ajoute à la commande en indiquant la quantité nécessaire. Avant de confirmer la commande, il doit renseigner le chantier pour lequel il commande ce matériel.

##### 🤔 Scénario 2
Pierre est sur un chantier. Il est 13h00. Il reçoit un mail, lui rappelant qu’il doit passer sa commande avant 14h00 pour avoir son matériel prêts pour le lendemain.

---

### 👷🏼‍♂️ Kevin Meunier - Magasinier
**Âge :** 28 ans  
**Profil :** magasinier dans la société depuis 10 ans  
**Compétences numériques :** avancées   
**Objectif principal :**  gérer le stock, reçevoir des commandes par l’interface  

#### 🎯 Objectifs
-	ajouter, supprimer, modifier des produits,
- reçevoir des commandes dans le Dashboard de l’interface,
- modifier les quantités de stock des produits (ajouts, suppressions),
-	imprimer une liste de la commande,
-	créer des chantiers, clôturer des chantiers,
-	imprimer une liste du matériel utilisé par chantier.

#### 😣 Frustrations
-	il perd beaucoup de temps à téléphoner à chaque électricien pour avoir toutes les commandes,
-	pas de système par internet pour visualiser les commandes,
-	beaucoup de fiches papiers pour commandes et projets.

#### 📌 Besoins
-	Dashboard clair et simple,
-	page de matériel,
-	page de chantier,
-	fonctionnalités export en pdf ou impression.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Il est 14h15, Kevin est au travail et veut préparer les commandes pour le jour suivant. Il regarde dans son Dashboard et voit qu’il a 15 nouvelles commandes. Il va dans l’onglet de commandes et il commence à préparer les commandes. Il ouvre une commande et imprime la liste de la commande. Il prépare les produits et colle la liste imprimée sur la caise du matériel pour que les électriciens puissent collecter leur commande le lendemain. Il retourne dans l’application et marque la commade terminée.
Pour les produits spéciaux ou les produits en rupture, les électriciens doivent passer un appel téléphonique pour assurer la disponibilité au futur du produit.

##### 🤔 Scénario 2 
Vers 16h20, Pierre arrive au dépôt avec plusieurs produits qu’il n’avait pas besoin au chantier. Le chantier est terminé. Kevin vérifie que les produits ne sont pas défectueux. Il ouvre la dernière commande de Kevin dans l’interface et diminue la quantité des produits éffectivement utilisés avant de les ranger par après. Ensuite il clôture le chantier et exporte une liste du matériel utilisé. Il envoie la liste par mail au responsable du chantier.

##### 🤔 Scénario 3
Une commande de matériel pour le stock arrive, mais Kevin remarque que la couleur de l’emballage des vis a changé. Il vérifie le produit, mais c’est bien le bon produit. Il va dans la page du produit et ajoute une note pour prévenir les électriciens que l’emballage a changé, mais qu’il s’agit bien du bon produit.

 
## 3. Fonctionnalités principales
### Magasiniers
-	créer, modifier ou supprimer du matériel,
-	imprimer des listes par commande à préparer,
-	gestion de stock,
-	imprimer une liste par chantier avec le matériel utilisé,
-	créer les chantiers,
-	modifier la quantité de matériel utilisé pour un chantier,
-	clôturer les chantiers,
-	créer et modifier des fiches de clients.

### Electriciens
-	rechercher de produits,
-	mettre en commande du matériel,
-	mettre en favoris le matériel préféré,
-	indiquer un chantier pour une commande.

### Administrateur (manager)
-	créer et modifier les électriciens et les magasiniers dans l’interface,
-	attribuer les rôles des utilisateurs,
-	créer et modifier des fiches de clients.

### Commandes
-	notifications de nouvelles commandes (magasinier),
-	suivi du statut d’une commande,
-	ajout d’un chantier à la commande.

### Matériel
-	fiche détaillée pour chaque produit avec image,
-	recherche et tri du matériel.

### Clients
- fiche détaillée pour chaque client avec les données nécessaires,
- recherche et tri des clients.

### Tous les utilisateurs
-	authentification,
-	rôles : magasinier, administrateur et électricien,
-	accès restreint selon les permissions.

 
## 4. Méthodologie 
-	Repository Github,
-	avancement par issues,
-	utilisation de milestones,
-	utilisation de branches multiples dans la branche de travail “dev”,
-	avancement par test.



