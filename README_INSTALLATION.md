Cette documentation a pour but de faciliter la préparation à la publication dans les différents stores d’application. À faire une fois le développement terminé et testé !

/!\ il n’est pas possible d’installer une extension non signée sur Firefox, ni d’utiliser une extention non enregistrée sur Chrome

#######################################
Préparation pour Chrome:
#######################################

Ouvrir Chrome et aller sur chrome://extensions/

Cliquer sur "Empaqueter l’extension"

    Répertoire racine de l’extension : Sélectionner le dossier REDIRECTION_VCC.
    Fichier de clé privée:
        À la première création, ne rien sélectionner
        Création suivante : Sélectionner le fichier de clé créé au 1er build

Deux fichiers sont créés au même niveau que le dossier REDIRECTION_VCC avec le même nom:

    Redirection_VCC.crx -> l’extension
    Redirection_VCC.pem -> clé de l’extension /!\ à ne surtout pas perdre /!\

Aller publier l’extension sur le Chrome Store:
Création de compte développeur Chrome Web Store: https://chrome.google.com/u/1/webstore/devconsole/register?hl=fr
Des frais de 5€ sont à payer


#######################################
Préparation pour Firefox:
#######################################

Entrer dans le dossier Redirection_VCC:
- sélectionner le contenu (Ne pas sélectionner les dossiers/fichiers de git, ils sont inutiles pour le bon fonctionnement de l’extension et ne feraient que l’alourdir pour rien.)

- Clic droit, envoyer vers dossier compressé (.zip)

Vérifier que le module est compatible FireFox sur  https://www.extensiontest.com/ 
Cela permet d’afficher les erreurs.
Firefox se contente de dire: "Le module est corrompu", sans donner plus de détail. D’ou cet outil.


C’est prêt pour être envoyé sur le store de Firefox pour y être signé.

https://addons.mozilla.org/fr/developers/ Il faut un compte, et cliquer sur "Proposez votre premier module"


Pour installer le module sur firefox (possible uniquement après signature): 
 - Dans firefox ouvrire la page "about:addons"
 - Cliquer sur la roue denté 
 	->Installer un module depuis un fichier
- Selectionner le .zip précédement créé.



#######################################
Préparation pour Safari:
#######################################