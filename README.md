# Stable-Management
Stable management software

1. FRENCH --------------------------------------------------------------------

Qu'est ce Stable-Management ?
Stable-Management est un logiciel de gestion d'écurie.

Il couvrira l'ensemble des aspects métiers qui l'on peut retrouver dans ce type d'établissement.

L'application sera découpée en micro-services pour un développement plus aisé de celle-ci.

Mise en place de l'application
-- L'administration
  - Les utilisateurs ===> Actions : ajout, supprimer, modifier, désactiver, droits d'accès
       - profil administrateur
       - les palfreniers
       - les moniteurs
       - les élèves
       - les propriétaires
       (- les bénévoles)
 
 -- Le nettoyage des boxes
   - 7 tables principales
       - T_boxe :
         - id_boxe
         - id_cheval
         - id_litière
         - taille
         - remarque
       - T_nettoyage_boxe
         - id_nettoyage_boxe
         - id_boxe
         - id_utilisateur
         - date_realisation
         - remarque
       - T_utilisateur
         - id_utilisateur
         - id_type_utilisateur
         - nom
         - prenom
         - date_naissance
         - adresse
       - T_type_utilisateur
         - id_type_utilisateur
         - rôle
       - T_cheval
         - id_cheval
         - nom_usuel
         - microship
         - ueln
         - date_naissance
         - id_origine_carnet (pays, studbook, ...)
       - T_litiere
          - id_litiere
          - nom_litiere
        - T_origine_carnet
           - id_origine_carnet
           - origine
