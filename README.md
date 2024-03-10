# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)

## Général
1.	<b>Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte</b>

    L’environnement à installer pour exécuter un script PHP est un serveur local apache (par exemple
    MAMP ou Laragon) .

2.	<b>Qu’est-ce qu’un algorithme ? </b> 

    Un algorithme est une suite d’opérations qui permet d’arriver à un resultat

3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?

    Une variable est une donnée dans PHP dont la valeur change, son préfixe est le signe $

4.	Qu’est-ce que la portée d’une variable ?
5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?

    Une constante est une donnée qui ne changera pas

6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation 
7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)

    int -> 9
    float -> 0.9
    string -> « Une chaîne de caractères »
    bool -> true
    null -> n’a pas de valeur

8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?

    Oui, des tableaux indexés, tableaux associatifs et tableaux multidimensionnels

9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles

    La séquence :
        Début algo
        Action 1 ;
        Action 2 ;
        Fin algo

    La sélection :
        Début algo
        SI CONDITION alors 
            Action 1
        SINON
            Action 2
        Fin algo

    La répétition :
        Début algo
        TANT QUE CONDITION faire
        Action 1 ;
        Fin algo

10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?

    strlen()

11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP
12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP

    Un cookie permet d’enregister des données sur un client et de les utiliser. 
    Un exemple serait de récupérer une session d’utilisateur.

13.	Quelle est la différence entre les instructions « require » et « include » en PHP

    La différence est que include n’arrêtera pas l’exécution du code si le fichier est n’existe pas alors que require le fera

14.	Comment effectuer une redirection en PHP ?

15.	Définir la partie « front-end » et « back-end » d’une application

    Le front-end est ce que voit l’utilisateur et avec quoi il interagit, le back-end ce sont les fonctionnalités de l’application

16.	Définir le contrôle de version ? Qu’est-ce que Git ?

    Le contrôle de version permet d’avoir plusieurs sauvegardes de son projet à ses différentes étapes d’avancement

17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples

## Front-end
18.	Définir HTML

    HTML signifie HyperText Marqup Language
    Le html sert à structurer une page web

19.	Définir CSS

    CSS signifie Cascading Style Sheets et permet de mettre en forme une page web

20.	Définir Javascript

    Javascript est un langage qui permet de programmer en back-end et front end, en front il permet de modifier les éléments du DOM de la page HTML

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
23.	Qu’est-ce qu’un sélecteur CSS ?

    Un sélecteur CSS permet de cibler les éléments d’une page HTML sur laquelle les styles CSS seront appliqués

24.	Quelle balise HTML permet de créer un lien hypertexte ?

    <a>

25.	Qu’est-ce qu’une requête AJAX ?
26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?

    Le selectionneur CSS qui permet de séléctionner tous les éléments d’une classe spécifique est le “.”
    Le selectionneur CSS qui permet de séléctionner un identifiant spécifique est le “#”

27.	Définir le responsive design

    Le responsive design est la manière dont la page web sera présentée selon la taille de la page

28.	Qu’est-ce que le templating ?
29.	Qu’est-ce qu’une fonction anonyme en Javascript ?

    Une fonction qui n’a pas de nom

30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?

    ‘nom du tableau’.push()

31.	Qu’est-ce qu’un « media query » ?

    Les media queries sont des règles qui indiquent quand on doit appliquer des propriétés CSS, en fonction de la taille de l'écran sur lequel s'affiche le site web

32.	Qu’est-ce qu’un pseudo élément en CSS ?

    Un pseudo-élément est un mot-clé ajouté à un sélecteur qui permet de mettre en forme certaines parties de l'élément ciblé par la règle.

    Exemple : 

    p::first-line {
    color: blue;
    text-transform: uppercase;
}

33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent
34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes

    GET et POST

    La méthode GET transmet les paramètres au serveur par l’intermédiaire de l’URL de la requête

    La méthode POST transmet les paramètres par l’intermédiaire d’un formulaire


## UX UI
35.	Quelle est la différence entre UX Design et UI Design ?
36.	Qu’est-ce qu’un wireframe ? 
37.	Qu’est-ce qu’un prototype ? 
38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?
39.	Qu’est-ce que l’accessibilité en UX Design ? 
40.	Qu’est-ce qu’une grille de mise en page ?
41.	Qu’est-ce que la notion d’affordance en UX Design ?
42.	Qu’est-ce qu’un « mobile first design » ?

## IV. Programmation orientée objet (POO)

43.	Donner une définition de la programmation orientée objet 

    C’est un modèle de langage de programmation qui s’articule autour d’objets et de données

44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?

    Une classe est un template pour un objet, lorsque l’objet sera crée il aura comme propriétés les propriétés de la classe à partir de laquelle il a été crée

45.	Qu’est-ce qu’un objet ?

    C’est l’instance d’une classe

46.	Définir la notion de propriété / attribut / méthode

    Une propriété c’est les différentes caractéristiques que va avoir une classe

    Une méthode permet d’effectuer des opérations avec ses propriétés

47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité

    La visibilité d’une propriété ou d’une méthode c’est à partir de quel endroit dans le programme elles peuvent être appelées ou modifiées.
    Les differents types de visibilité sont public, private et protected.

48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?

    La méthode magique __construct($parametre1, …)

49.	Qu’est-ce que l’encapsulation ?

    L’encapsulation permet lors de la création d’un objet de le stocker dans la propriété de type tableau d’un autre objet

50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple

    Le concept mis en œuvre est celui de l’héritage. Pour exemple on pourrait dire que la classe VoitureElectrique hérite de la classe Voiture

51.	Définir l’opérateur de résolution de portée

    Il est représente par un double deux-points :: et il permet d’accéder une constante, une méthode ou propriété statique de la classe

52.	Définir une méthode / propriété statique
53.	Définir le polymorphisme en POO
54.	Définir une méthode / classe abstraite ?
55.	Définir le chaînage de méthodes

    Le chaînage de méthodes permet d’écrire plusieurs méthodes l’une à la suite de l’autre sur la même ligne

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »

    La méthode __toString() permet de définir ce que l’on veut afficher lorsque on appelle la fonction echo() sur un objet

57.	Qu’est-ce qu’un « autoload » ?

    C’est une fonction ( __autoload() ) qui permet d’inclure automatiquement des classes enregistrées dans différents fichiers

58.	Comment appelle-t-on en français les « getters » et les « setters » ?

    Accesseurs et mutateurs

59.	Qu’est-ce que la sérialisation en PHP ? 

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence

    Grâce aux requêtes http qui signifie HyperText Transfer Protocol 

61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
62.	Qu’est-ce que l’architecture MVC ?
63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
64.	Quels sont les avantages de l’architecture MVC ?
65.	Existe-t-il des variantes à l’architecture MVC ?
66.	Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise
68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation
b.	Planification, exécution et contrôle
c.	Création, modification et suppression
69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
71.	Donner la définition des mots suivants :
a.	Entité
b.	Relation
c.	Cardinalité
d.	Clé primaire / clé étrangère
72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
73.	Qu’est-ce qu’une base de données ?

    C’est un système électronique qui permet d’accéder, de manipuler ou de mettre à jour des données

74.	Définir les notions suivantes :

a.	SQL

    Structured Query Language qui est un langage informatique servant à exploiter des bases de données

b.	MySQL

    Un SGBD

c.	SGBD (donner 2 exemples de SGBD)

    Système de gestion de base de données (MySQL, Oracle)

75.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___

    Dans une base de données, les données sont stockées dans des TABLES. Celles-ci sont constituées de lignes appelées ENREGISTREMENTS et de colonnes appelées CHAMPS

76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?

    C’est l’opération qui permet d’associer plusieurs tables d’une BDD par le biais d’un lien logique entre ces tables

78.	A quoi sert une vue dans une base de données ?

    Sert à visualiser le résultat d’une requête 

79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
80.	Quelles sont les fonctions d’agrégation en SQL ?
81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
b.	Modifier un enregistrement dans une table
c.	Supprimer un enregistrement dans une table
d.	Supprimer la base de données
e.	Filtrer les résultats d’une requête SQL
f.	Trier les résultats d’une requête SELECT
g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
h.	Concaténer 2 chaînes de caractères 
83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony
84.	Qu’est-ce que Symfony ?
85.	Sur quel langage de programmation et design pattern repose Symfony ? 
86.	Quelle est la dernière version en date de Symfony ?
87.	Qu’est-ce qu’un bundle ? 
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97.	Définir l’attaque par force brute et l’attaque par dictionnaire
98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101.	Qu’est-ce qu’une politique de mots de passe forts ?
102.	Qu’est-ce que l’hameçonnage ?
103.	Définir la « validation des entrées »

## RGPD
104.	Qu’est-ce que le RGPD ?
105.	Quel est son objectif principal ?
106.	Quelle est la date d’entrée en vigueur du RGPD ?
107.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
108.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
109.	Quel est le consentement valide selon le RPGD ?
110.	Qu’est-ce qu’une politique de confidentialité ?
111.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112.	Quels sont les droits des utilisateurs selon le RGPD ?
113.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
114.	Qu’est-ce que le SEO ? 

        Optimisation pour les moteurs de recherche

115.	Quel est l’objectif principal du SEO ?

        D’améliorer le positionnement d’un site dans les moteurs de recherche

116.	Existe-t-il plusieurs types de référencement ? Lesquels ?
117.	Qu’est-ce que la densité de mots-clés en SEO ?
118.	Qu’est-ce qu’une balise « alt » ?

        Une balise alt permet de communiquer aux personnes malvoyantes la description d’un élément d’une page qu’ils ne peuvent pas voir

119.	Qu’est-ce que la balise « meta description » ?
120.	Qu’est-ce que le « nofollow » en SEO ?
121.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123.	Quelle est la recommandation pour les URL d'un site web bien référencé ?
124.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125.	Qu'est-ce que l'optimisation des images pour le référencement ?
126.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127.	Qu’est-ce que la gestion de projet ?	
128.	Qu’est-ce qu’une méthode Agile de gestion de projet ? 
129.	Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130.	A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131.	Qu’est-ce que la planification itérative ?
132.	Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133.	Qu’est-ce qu’une réunion de revue de projet ?
134.	Qu’est-ce qu’un livrable dans un projet ? 
135.	Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136.	Qu’est-ce que le DevOps et quel est son objectif principal ?
137.	Qu’est-ce que l’intégration continue ? 
138.	Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
139.	Qu’est-ce qu’un test unitaire ? 
140.	Quelle est l'unité de code testée lors d'un test unitaire ?
141.	Quelles sont les caractéristiques d'un bon test unitaire ?
142.	Qu'est-ce qu'une assertion dans un test unitaire ?
 
## English
1)	What does JavaScript enable you to do on a website ?

    Add interactive behavior and dynamic content

2)	Which programming language is primarily used for server-side web development ?

    PHP

3)	What is the purpose of a web browser ?

    To render and display web pages

4)	What is the difference between GET and POST methods in HTTP ?

    GET and POST methods are interchangeable
    
5)	What is the purpose of version control systems (e.g., Git) in web development ?

    To track changes and manage collaborative development

6)	What is the purpose of a framework in web development ?

    To provide a structured environment for building web applications

7)	What does NoSQL stand for ?
a.	Not Only SQL
b.	Non-Structured Query Language
c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models