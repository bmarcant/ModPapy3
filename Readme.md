ModPapy3 : modification de documents dans le logiciel Papyrus2000
=================================================================

Introduction
------------

Le logiciel [Papyrus2000](http://www.papyrus2000.com) est un très bon logiciel de gestion de bibliothèque, compatible avec toutes les versions de Windows, de XP à Windows 8.

Ce logiciel est désormais disponible en téléchargement gratuit en version complète. 

Pour entrer de nouveaux documents dans Papyrus2000, il y a la possibilité d'importer un fichier au format WK1 ([Lotus 1-2-3](https://fr.wikipedia.org/wiki/Lotus_1-2-3)).

Dans la documentation de ce logiciel, il est dit que si des documents de mêmes références existent déjà dans la base, les champs du fichier écrasent les données de la base.

On pourrait donc utiliser l'import pour faire des mises à jour de document dans Papyrus2000.

Attention, car dans le fichier d'import, il y a des champs inhérents à la gestion des prêts ("Prete a", "CodeLecteur", "Prete le", ...) qui, s'ils ne correspondent pas aux données de la base, vont perturber le fonctionnement de Papyrus. Il faudra alors réparer cela avec `Papyrus2000 > Fichier > Utilitaires > Docteur Papyrus`.

Objet
-----

Le script `ModPapy3` permet de modfier des documents dans Papyrus (Titre, Auteur, Editeur, ...) à partir d'un fichier au format CSV, sans perturber la gestion des prêts pour les documents concernés.

Utilisation
-----------

Ce script est à insérer dans la définition des scripts dans Papyrus2000 : `Papyrus 2000 > Spécifique`.

Le fichier CSV, en entrée, est celui qui découle de l'export de Papyrus2000 : `ExpPapy3.xls`.

Version
-------

La version courante est la 1.0.

Note
----

J'ai aussi créé le script [ImpPapy3](https://github.com/bmarcant/ImpPapy3.git) pour importer des documents dans Papyrus2000.

