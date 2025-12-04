# Cahier des charges – Application de gestion de stock et de commandes d’une entreprise d’électricien
## 1. Contexte général
Ce projet vise à concevoir une application Web permettant à la société de :
-	passer des commandes,
-	suivre le statut des commandes,
-	créer, modifier des projets,
-	gérer les commandes,
-	gérer le stock,
-	rechercher et trier des produits,
-	gérer les différents utilisateurs,
-	rappeler les électriciens de passer leur commande.
  
   
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
-	pas de stystème qui permet automatiquement de faire des rappels de commande,
-	perte de temps par le magasinier car électriciens oublient de passer la commande et donc perte d’argent,
-	pas de gestion par projet.

#### 📌 Besoins
-	Dashboard clair,
-	gestion des rôles simples,
-	système qui permet aux employés de passer des commandes plus facilement,
-	système facile à utiliser pour tous les employés et travailleurs.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Marc a engagé un nouveau électricien. Il doit lui créer un compte sur l’application. Il peut renseigner son nom et prénom, son rôle (électricien), son numéro de téléphone de tavail et son numéro de téléphone privé. Il peut aussi ajouter dans sa fiche son adresse. Après validation de la fiche du nouveau électricien, il reçoit un email de bienvenue avec ses identifiants temporaires et une invitation à les modifier dans son profil.  
Le logiciel lui permet de faire les mêmes manipulations pour un magasinier. 

##### 🤔 Scénario 2
Le magasinier a constaté qu’il y a du matériel défectueux dans le stock. Il fait une liste du matériel pour Marc et envoie la à Marc, qui doit vérifier la liste et se renseigner sur des remplacements, ou autres solutions. Entre temps, le magasinier a retiré ce matériel du stock pour ne pas rencontrer des problèmes lors de la préparation des commandes.   
Marc a réçu la liste de son magasinier par email. Marc vérifie d’abord cette liste. Ensuite il prend contact avec les délégués pour des produits de remplacements. Un des délégués se rend sur place et apporte des remplacements pour certains produits. Après le rendez-vous, Marc se rend dans l’onglet stock et change le stock de ses produits et apporte les produits chez son magasinier. 

##### 🤔 Scénario 3
Franco travaille depuis 15 ans pour Marc. Il a 54 ans et il a demandé à son patron Marc, s’il pouvait changer de job au sein de sa société. Marc lui a proposé un job au magasin qui vient de se libérer, car Franco a de bonnes connaissances des produits et car le travail est moins exigeant pour ces genoux.   
Marc a déjà créé une fiche pour Franco, mais il est enregistré en tant qu’éléctricien. Il doit changer le rôle de Franco pour que Franco ait accès aux fonctionnalités du stock. 

---

### 🧑🏽‍🔧 Pierre Simon - Electricien
**Âge :** 34 ans  
**Profil :** electricien dans la société depuis 4 ans  
**Compétences numériques :** normales   
**Objectif principal :**  rechercher facilement des produits, les ajouter à la commande et passer une commande.  

#### 🎯 Objectifs
-	rechercher des produits,
-	reconnaître facilement les produits grâce à des images,
-	ajouter les produits dans le panier,
-	augmenter ou diminuer les quantités de produits,
-	retirer des produits du panier,
-	passer une commande attachée à un projet.

#### 😣 Frustrations
-	oublie souvent de passer sa commande. Pas de stystème qui permet automatiquement de faire des rappels de commande,
-	pas de système pour choisir des produits sur internet (appel téléphonique ou mail),
-	commande par email ou téléphone. Pas d’images lors de la commande. Erreurs fréquents. 

#### 📌 Besoins
-	page de produits claire,
-	barre de recherche et fonctionnalités de tri,
-	image qui illustre le produit,
-	description ou données clées sur la fiche de détail du produit.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Pierre est sur un chantier. Il lui manque du matériel pour terminer son travail. Il se connecte à l’application et il se rend sur le site des produits de l’application. Il recherche les produits qu’il a besoin et il les ajoute au panier en indiquant la quantité nécessaire. Avant de confirmer la commande, il doit renseigner le projet pour lequel il commande ces produits. 

##### 🤔 Scénario 2
Pierre est sur un chantier. Il est 13h00. Il reçoit un mail, lui rappelant qu’il doit passer sa commande avant 14h00 pour avoir ses produits prêts pour le lendemain.

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
-	créer des projets, clôturer des projets,
-	imprimer une liste des produits utilisés par projet.

#### 😣 Frustrations
-	il perd beaucoup de temps à téléphoner à chaque électricien pour avoir toutes les commandes,
-	pas de système par internet pour visualiser les commandes,
-	beaucoup de fiches papiers pour commandes et projets.

#### 📌 Besoins
-	Dashboard clair et simple,
-	page de stock,
-	page de produits,
-	page de projets,
-	fonctionnalités export en pdf.

#### 📚 Scénario d’utilisation
##### 🤔 Scénario 1
Il est 14h15, Kevin est au travail et veut préparer les commandes pour le jour suivant. Il regarde dans son Dashboard et voit qu’il a 15 nouvelles commandes. Il va dans l’onglet de commandes et il commence à préparer les commandes. Il ouvre une commande et imprime la liste de la commande. Il prépare les produits et colle la liste imprimée sur la caise du matériel pour que les électriciens puissent collecter leur commande le lendemain. Il retourne dans l’application et marque la commade terminée. Les produits vont automatiquement sortir du stock après validation de la commande.  
Pour les produits spéciaux ou les produits en rupture, les électriciens doivent passer un appel téléphonique pour assurer la disponibilité au futur du produit.


##### 🤔 Scénario 2 
Kevin imprime la liste du stock pour faire inventaire. Il trouve des produits défectueux. Kevin retire ces produits du stock et les mets de côté. Il envoie un mail à son patron Marc pour lui demander ce qu’il veut faire maintenant (recommander les produits, demander des remplacements aux délégués ou ne plus en recommander).

##### 🤔 Scénario 3
Vers 16h20, Pierre arrive au magasin avec plusieurs produits qu’il n’avait pas besoin au chantier de son projet. Le projet est terminé. Kevin vérifie que les produits ne sont pas défectueux. Il ouvre la page du projet dans l’interface et diminue la quantité des produits éffectivement utilisés. Il retourne dans la page du stock et augmente les quantités des produits retournés avant de les ranger par après. Ensuite il clôture le projet et exporte une liste du matériel utilisé. Il l’envoie par mail au département de facturation.

##### 🤔 Scénario 4
Une commande de produits pour le stock arrive, mais Kevin remarque que la couleur de l’emballage des vis a changé. Il vérifie le produit, mais c’est bien le bon produit. Il va dans la page du produit et ajoute une note pour prévenir les électriciens que l’emballage a changé, mais qu’il s’agit bien du bon produit. Il actualise aussi l’image du produit en même temps. 

 
## 3. Fonctionnalités principales
### Magasiniers
-	créer, modifier ou supprimer des produits,
-	imprimer des listes par équipe à préparer,
-	gestion de stock,
-	imprimer une liste par projet avec le matériel utilisé,
-	créer les projets,
-	modifier les produits utilisés pour un projet,
-	clôturer les projets.

### Electriciens
-	rechercher de produits,
-	mettre dans un panier des produits,
-	indiquer un projet pour une commande.

### Administrateur (patron)
-	peut créer et modifier les travailleurs et magasiniers,
-	peut attribuer les rôles des utilisateurs.

### Commandes
-	notifications de nouvelles commandes (magasinier),
-	suivi du statut d’une commande,
-	ajout d’un projet à la commande.

### Produits
-	fiche détail pour chaque produit avec image,
-	recherche et tri des produits,
-	les produits en rupture de stock ne sont pas affichés aux électriciens.

### Tous les utilisateurs
-	authentification,
-	rôles : magasinier, administrateur et travailleur,
-	accès restreint selon les permissions.


 
## 4. Méthodologie 
-	Repository Github,
-	avancement par issues,
-	utilisation de milestones,
-	utilisation de branches multiples dans la branche de travail “dev”,
-	avancement par test.



