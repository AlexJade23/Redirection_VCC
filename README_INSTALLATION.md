# Documentation pour la publication d'une extension sur les stores d'application

Cette documentation a pour but de faciliter la préparation à la publication dans les différents stores d’application. À faire une fois le développement terminé et testé !

**/!\ il n’est pas possible d’installer une extension non signée sur Firefox, ni d’utiliser une extention non enregistrée sur Chrome**

## Préparation pour Chrome:

1. Ouvrir Chrome et aller sur chrome://extensions/
2. Cliquer sur "Empaqueter l’extension"
    - Répertoire racine de l’extension : Sélectionner le dossier REDIRECTION_VCC.
    - Fichier de clé privée:
        - À la première création, ne rien sélectionner
        - Création suivante : Sélectionner le fichier de clé créé au 1er build

Deux fichiers sont créés au même niveau que le dossier REDIRECTION_VCC avec le même nom:

- Redirection_VCC.crx -> l’extension
- Redirection_VCC.pem -> clé de l’extension /!\ à ne surtout pas perdre /!\

3. Aller publier l’extension sur le Chrome Store:
   - Création de compte développeur Chrome Web Store: [https://chrome.google.com/u/1/webstore/devconsole/register?hl=fr](https://chrome.google.com/u/1/webstore/devconsole/register?hl=fr)
   - Des frais de 5€ sont à payer

## Préparation pour Firefox:

1. Entrer dans le dossier Redirection_VCC:
   - Sélectionner le contenu (Ne pas sélectionner les dossiers/fichiers de git, ils sont inutiles pour le bon fonctionnement de l’extension et ne feraient que l’alourdir pour rien.)
   - Clic droit, envoyer vers dossier compressé (.zip)

2. Vérifier que le module est compatible FireFox sur [https://www.extensiontest.com/](https://www.extensiontest.com/)
   - Cela permet d’afficher les erreurs.
   - Firefox se contente de dire: "Le module est corrompu", sans donner plus de détail. D’où cet outil.

3. C’est prêt pour être envoyé sur le store de Firefox pour y être signé.
   - [https://addons.mozilla.org/fr/developers/](https://addons.mozilla.org/fr/developers/) Il faut un compte, et cliquer sur "Proposez votre premier module"

4. Pour installer le module sur Firefox (possible uniquement après signature) :
   - Dans Firefox, ouvrir la page "about:addons"
   - Cliquer sur la roue dentée
        - Installer un module depuis un fichier
   - Sélectionner le .zip précédemment créé.
       - Faire le test

## Préparation pour Safari:

**/!\ Cette méthode n’a pas pu être testée, elle est donc soumise à condition.**

1. Faire une copie du zip créé pour Firefox et remplacer l’extension ".zip" par ".safariextz".
2. Importer le fichier dans le navigateur Safari.

3. Pour le publier, il faut aller sur : [https://developer.apple.com/](https://developer.apple.com/) Créer un compte et s’acquitter des 99 $ d’abonnement annuel.

4. Apple restant un environnement fermé, sans iOS, il n’est pas possible de confirmer le bon fonctionnement.