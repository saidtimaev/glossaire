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

3.	<b>Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?</b>

    Une variable est une donnée dans PHP dont la valeur change, son préfixe est le signe $

4.	<b>Qu’est-ce que la portée d’une variable ?</b>

    La portée d'une variable c'est la partie du script à partir de laquelle elle peut être utilisée/ référencée
  	
6.	<b>Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?</b>

    Une constante est une donnée qui ne changera pas durant l'exécution du programme, la variable quand à elle peut changer de valeur

7.	<b>Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation </b>

    Il en existe 9 :
  	- $GLOBALS
    - $_SERVER
    - $_REQUEST
    - $_POST
    - $_GET
    - $_FILES
    - $_ENV
    - $_COOKIE
    - $_SESSION

    Exemple : la superglobale $_POST qui permet de récupérer les données envoyées par une requête dont la méthode est POST
  	
9.	<b>Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)</b>

    int -> 9
    float -> 0.9
    string -> « Une chaîne de caractères »
    bool -> true
    null -> n’a pas de valeur

10.	<b>Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?</b>

    Oui, des tableaux indexés, tableaux associatifs et tableaux multidimensionnels

11.	<b>Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles</b>

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

12.	<b>Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?</b>

    strlen()

13.	<b>Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP</b>

    Une session est un moyen de stocker des informations dans des variables pour qu'elles puissent ensuite être utilisées sur différentes pages

    Exemple d'application : Enregister des informations (nom d'utilisateur, couleur favorite, etc...) sur un utilisateur pour qu'elles puissent ensuite être utilisées sur différentes pages

14.	<b>Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP</b>

    Un cookie permet d’enregister des données sur un client et de les utiliser. 
    Un exemple serait de récupérer une session d’utilisateur.

15.	<b>Quelle est la différence entre les instructions « require » et « include » en PHP</b>

    La différence est que include n’arrêtera pas l’exécution du code si le fichier est n’existe pas alors que require le fera

16.	<b>Comment effectuer une redirection en PHP ?</b>

    Avec la fonction header();

    Exemple : header('Location: http://www.exemple.com/');

17.	<b>Définir la partie « front-end » et « back-end » d’une application</b>

    Le front-end est ce que voit l’utilisateur et avec quoi il interagit, le back-end ce sont les fonctionnalités de l’application

18.	<b>Définir le contrôle de version ? Qu’est-ce que Git ?</b>

    Le contrôle de version permet d’avoir plusieurs sauvegardes de son projet à ses différentes étapes d’avancement

19.	<b>Qu’est-ce qu’un CMS ? Citer au moins 2 exemples</b>

    Un CMS, Content Management System ou Système de gestion de contenu est un système qui permet de créer ou de mettre a jour un site internet 
    sans avoir besoin de toucher au code source

    Exemples : WordPress, Drupal

## Front-end
18.	<b>Définir HTML</b>

    HTML signifie HyperText Marqup Language
    Le html sert à structurer une page web

19.	<b>Définir CSS</b>

    CSS signifie Cascading Style Sheets et permet de mettre en forme une page web

20.	<b>Définir Javascript</b>

    Javascript est un langage qui permet de programmer en back-end et front end, en front il permet de modifier les éléments du DOM de la page HTML

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
23.	<b>Qu’est-ce qu’un sélecteur CSS ?</b>

    Un sélecteur CSS permet de cibler les éléments d’une page HTML sur laquelle les styles CSS seront appliqués

24.	<b>Quelle balise HTML permet de créer un lien hypertexte ?</b>

    La balise '<'a'>'

25.	Qu’est-ce qu’une requête AJAX ?
26.	<b>Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?</b>

    Le selectionneur CSS qui permet de séléctionner tous les éléments d’une classe spécifique est le “.”
    Le selectionneur CSS qui permet de séléctionner un identifiant spécifique est le “#”

27.	<b>Définir le responsive design</b>

    Le responsive design est la manière dont la page web sera présentée selon la taille de la page

28.	Qu’est-ce que le templating ?
29.	<b>Qu’est-ce qu’une fonction anonyme en Javascript ?</b>

    Une fonction qui n’a pas de nom

30.	<b>Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?</b>

    ‘nom du tableau’.push()

31.	<b>Qu’est-ce qu’un « media query » ?</b>

    Les media queries sont des règles qui indiquent quand on doit appliquer des propriétés CSS, en fonction de la taille de l'écran sur lequel s'affiche le site web

32.	<b>Qu’est-ce qu’un pseudo élément en CSS ?</b>

    Un pseudo-élément est un mot-clé ajouté à un sélecteur qui permet de mettre en forme certaines parties de l'élément ciblé par la règle.

    Exemple : 

    p::first-line {
    color: blue;
    text-transform: uppercase;
}

33.	<b>Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent</b>

    C'est un framework front-end 

    Exemples : Tailwind, React

34.	<b>Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes</b>

    GET et POST

    La méthode GET transmet les paramètres au serveur par l’intermédiaire de l’URL de la requête

    La méthode POST transmet les paramètres par l’intermédiaire d’un formulaire


## UX UI
35.	<b>Quelle est la différence entre UX Design et UI Design ?</b>

    L'UX Design désigne l'intéraction de l'utilisateur avec l'interface d'un page web alors que l'UI Design désigne l'optimisation d'éléments graphiques d'une interface

36.	<b>Qu’est-ce qu’un wireframe ? </b>

    C'est le schéma d'une interface utilisateur avec un graphisme simplifié

37.	<b>Qu’est-ce qu’un prototype ? </b>

    C'est la répresentation la plus proche du produit final

38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?
39.	Qu’est-ce que l’accessibilité en UX Design ? 
40.	Qu’est-ce qu’une grille de mise en page ?
41.	Qu’est-ce que la notion d’affordance en UX Design ?
42.	Qu’est-ce qu’un « mobile first design » ?

## IV. Programmation orientée objet (POO)

43.	<b>Donner une définition de la programmation orientée objet </b>

    C’est un modèle de langage de programmation qui s’articule autour d’objets et de données

44.	<b>Qu’est-ce qu’une classe ? Comment la déclare-t-on ?</b>

    Une classe est un template pour un objet, lorsque l’objet sera crée il aura comme propriétés les propriétés de la classe à partir de laquelle il a été crée

45.	<b>Qu’est-ce qu’un objet ?</b>

    C’est l’instance d’une classe

46.	<b>Définir la notion de propriété / attribut / méthode</b>

    Une propriété c’est les différentes caractéristiques que va avoir une classe

    Une méthode permet d’effectuer des opérations avec ses propriétés

47.	<b>Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité</b>

    La visibilité d’une propriété ou d’une méthode c’est à partir de quel endroit dans le programme elles peuvent être appelées ou modifiées.
    Les differents types de visibilité sont public, private et protected.

48.	<b>Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?</b>

    La méthode magique __construct($parametre1, …)

49.	<b>Qu’est-ce que l’encapsulation ?</b>

    L’encapsulation permet lors de la création d’un objet de le stocker dans la propriété de type tableau d’un autre objet

50.	<b>Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple</b>

    Le concept mis en œuvre est celui de l’héritage. Pour exemple on pourrait dire que la classe VoitureElectrique hérite de la classe Voiture

51.	<b>Définir l’opérateur de résolution de portée</b>

    Il est représente par un double deux-points :: et il permet d’accéder une constante, une méthode ou propriété statique de la classe

52.	<b>Définir une méthode / propriété statique</b>

    Une méthode statique est une méthode qui peut-être appelée directement d'une classe

    Une propriété statique est une propriété qui peut-être appelée directement d'une classe

53.	<b>Définir le polymorphisme en POO</b>

    Le principe du polymorphisme permet à des classes d'implémenter la même méthode mais avec un comportement différent 

54.	<b>Définir une méthode / classe abstraite ?</b>

    Une classe abstraite est une classe qui contient au moins une méthode abstraite
    Elle ne peut pas être instanciée
    Une méthode abstraite est une méthode qui est définie dans une classe enfant

55.	<b>Définir le chaînage de méthodes</b>

    Le chaînage de méthodes permet d’écrire plusieurs méthodes l’une à la suite de l’autre sur la même ligne

56.	<b>Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »</b>

    La méthode __toString() permet de définir ce que l’on veut afficher lorsque on appelle la fonction echo() sur un objet

    Exemple de méthodes magiques : __construct(), __get(), set(), __isset(), ...

57.	<b>Qu’est-ce qu’un « autoload » ?</b>

    C’est une fonction ( __autoload() ) qui permet d’inclure automatiquement des classes enregistrées dans différents fichiers

58.	<b>Comment appelle-t-on en français les « getters » et les « setters » ?</b>

    Accesseurs et mutateurs

59.	Qu’est-ce que la sérialisation en PHP ? 

## Architecture 
60.	<b>Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence</b>

    C'est un environnement dans lequels un client communique avec un serveur

    Grâce aux requêtes HTTP qui signifie HyperText Transfer Protocol 

    HTTPS (HyperText Transfer Protocol Secure) est une version plus sécurisée du protocole HTTP

61.	<b>Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern</b>

    C'est une méthodologie qui permet l'optimisation du code dans un projet

    Exemples : Factory, Composite, Iterator ...


62.	<b>Qu’est-ce que l’architecture MVC ?</b>

    C'est un design pattern

63.	<b>Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?</b>

    Model : accès à la BDD
    View : Affichage de la page
    Controller : logique, calculs et décisions

64.	<b>Quels sont les avantages de l’architecture MVC ?</b>

    Il permet une meilleur organisation du code 

65.	<b>Existe-t-il des variantes à l’architecture MVC ?</b>

    MVP , Model View Presenter

66.	Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données
67.	<b>Qu’est-ce que la modélisation de données ? Définir la méthode Merise</b>

    Le processus de création d'une représentation visuelle ou d'un plan qui définit les systèmes de collecte et de gestion de l'information de toute organisation.

    Merise est une méthode d'analyse, de conception et de gestion de projet informatique.


68.	<b>Quelles sont les 3 étapes principales de la méthode Merise ? </b>
    
    a.	Analyse, conception et réalisation

69.	<b>Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?</b>

    Le modèle conceptuel de données est une représentation formelle de données

70.	<b>Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?</b>

    Le modèle logique de données est une répresentation textuelle de données


71.	<b>Donner la définition des mots suivants :</b>
    
    <b>a.	Entité</b>
    C'est un ensemble d'éléments ou d'objets de même nature

    <b>b.	Relation</b>
    C'est une association entre les tables d'une BDD qui est créé à l'aide d'une instruction de jointure

    c.	Cardinalité

    d.	Clé primaire / clé étrangère
72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
73.	Qu’est-ce qu’une base de données ?

    C’est un système électronique qui permet d’accéder, de manipuler ou de mettre à jour des données

74.	<b>Définir les notions suivantes :</b>

<b>a.	SQL</b>

    Structured Query Language qui est un langage informatique servant à exploiter des bases de données

<b>b.	MySQL</b>

    Un SGBD

<b>c.	SGBD (donner 2 exemples de SGBD)</b>

    Système de gestion de base de données (MySQL, Oracle Database)

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
82.	<b>Quelles sont les clauses qui permettent de :</b>
    <b>a.	Insérer un nouvel enregistrement dans une table</b>

        INSERT 

    <b>b.	Modifier un enregistrement dans une table</b>

        UPDATE

    <b>c.	Supprimer un enregistrement dans une table</b>
    
        DELETE

    <b>d.	Supprimer la base de données</b>

        DROP 

    e.	Filtrer les résultats d’une requête SQL
    f.	<b>Trier les résultats d’une requête SELECT</b>

        ORDER BY

    g.	<b>Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique</b>

        GROUP BY

    h.	<b>Concaténer 2 chaînes de caractères</b>

        CONCAT 

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
1)	<b>What does JavaScript enable you to do on a website ?</b>

    Add interactive behavior and dynamic content

2)	<b>Which programming language is primarily used for server-side web development ?</b>

    PHP

3)	<b>What is the purpose of a web browser ?</b>

    To render and display web pages

4)	<b>What is the difference between GET and POST methods in HTTP ?</b>

    GET and POST methods are interchangeable
    
5)	<b>What is the purpose of version control systems (e.g., Git) in web development ?</b>

    To track changes and manage collaborative development

6)	<b>What is the purpose of a framework in web development ?</b>

    To provide a structured environment for building web applications

7)	<b>What does NoSQL stand for ?</b>
    
    a.	Not Only SQL

8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models
