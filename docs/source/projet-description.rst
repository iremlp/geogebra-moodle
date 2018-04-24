====================
GeoGebra et Moodle ?
====================

.. 
   Ceci est un commentaire :
   Pour retrouver toutes les directives ou les possibilités du reStructuredText :
   http://docutils.sourceforge.net/docs/user/rst/cheatsheet.txt


Il existe un plugin pour *Moodle* [#f1]_ permettant de créer des activités *GeoGebra* et de sauvegarder son état. Il est alors possible :

* de sauvegarder la production d'un élève
* d'évaluer manuellement ou **automatiquement** l'activité.




GeoGebra
========

GeoGebra [#fggb]_ est un logiciel de géométrie dynamique permettant d'explorer, d'expérimenter mais aussi de créer de la ressource pour les élèves.

Nous utilisons *GeoGebra* pour créer des exerciseurs. Généralement, nos activités élèves sont construites de la façon suivante :

#. réaliser une tâche générée avec des **valeurs aléatoires**
#. saisir sa réponse et valider
#. si c'est incorrect, alors la réponse est affichée avec un corrigé
#. recommencer un certain nombre de fois les points 1 à 3
#. à la fin, obtenir un score sur son activité


.. todo::  

   Insérer une gif animée d'un exerciseur GGB



Moodle
======

   
Moodle [#fmoodle]_ est une application en ligne permettant de faire de la formation à distance. De nombreux MOOC actuels l'utilisent. Cet outil est disponible dans de nombreuses académie. Par exemple sur les académies de Nice et d'Aix-Marseille, Moodle est intégré à l'ENE Atrium [#fatrium]_.


Nous utilisons Moodle pour mettre les élèves en activités à l'aide d'**évaluations formatives**. En effet, la notation choisie permet à l'éléve de s'entraîner, de se former et d'être en réussite.

.. tip:: 

   .. image:: _static/fig-moodle.png
      :width: 30%
      :align: right

   Dans Moodle, nous utilisons la notation suivante :
    
   * nombre maximum de tentatives : **illimité**
   * méthode d'évaluation : **Tentative la plus haute**

Ainsi, l'élève fait autant de fois qu'il le désire l'actitivé proposée. Il n'est pas obligé d'aller à son terme si c'est une activité répétitive. L'élève apprend de ses erreurs car un corrigé l'accompagne à chaque tentative. Lorsqu'il le désire, l'élève recommence l'activité et tente alors d'avoir un score maximal.

Cette façon d'évaluer est pour nous très pertinente. 
L'élève est en activité, il est motivé car il sait qu'il peut réussir.
Il gagne en autonomie car, grâce au corrigé, il cherche à comprendre et à ne pas reproduire ses erreurs. 
En effet, chaque tentative est différente de la précédente car les fichiers sont conçus à partir de **valeurs aléatoires**.


Le plugin GeoGebra pour Moodle
==============================

Ce plugin offre un nouveau type d'activité dans Moodle : *GeoGebra*.

Utilisation de base
-------------------

De base, il permet à l'enseignant de diffuser un fichier GeGebra (à envoyer dans l'onglet *Contenu*).
L'élève entre alors dans l'activité et peut :

* modifier le fichier 
* sauvegarder ses modifications pour y revenir plus tard
* envoyer sa production à l'enseignant.

L'enseigant pourra alors consulter les productions de chaque élève (un peu long car à chaque fois le fichier doit s'ouvrir), ajouter commentaire et/ou note.

Utilisation avancée
-------------------

Une utilisation avancée du plugin permet la **notation automatique**.

.. tip::

   Pour activer la notation automatique, il faut :

   * dans Moodle
     * cocher *Activité auto-évaluée* dans l'onglet *Note*
     * définir la note maximale
   * dans GeoGebra
     * créer une variable *grade* qui aura une valeur entre 0 et la note maximale
     * incrémenter la variable grade en fonction de l'activité de l'élève


   .. image:: _static/fig-moodle2.png
      :width: 30%
   .. image:: _static/fig-moodle3.png
      :width: 60%
      :align: right



----


.. [#f1] Voir le site officiel du plugin : https://moodle.org/plugins/mod_geogebra
.. [#fggb] Site GeoGebra : http://geogebra.org/
.. [#fmoodle] Site francophone de Moodle : https://moodle.org/?lang=fr
.. [#fatrium] Présentation de l'intégration de Moodle (et autres) avec Atrium : https://www.atrium-paca.fr/web/assistance/acceder-a-moodle-chamilo-pronote-correlyce
