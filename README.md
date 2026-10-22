# TP2 Cybersécurité
- Nom: (Lucresse Jouonang Kwagwe)
- Matricule: (6301154)
- Groupe: (1010)

## Attaque (exploit)

Voici les étapes détaillées pour pouvoir modifier le courriel / téléphone sur la page demandée:

### Étape 1 : Reconnaissance réseau avec Nmap

 **Commande utilisée :** `nmap 192.168.0.15`
 **Objectif et effet :** Scanner la machine cible depuis le poste Windows afin d'identifier les services actifs et les ports TCP ouverts à distance. Le scan a permis de découvrir que le service HTTP (port 80) et le service SSH (port 22) étaient ouverts et accessibles.
![alt text](image.png)

### Étape 2 : Authentification distante via SSH (Réutilisation de mot de passe)

 **Commande utilisée** : `ssh bob@192.168.0.15`
 **Objectif et effet** : Tenter une connexion à distance sur le serveur Linux en utilisant les informations collectées . À partir des prénoms et années de naissance des enfants de Bob, le mot de passe `Sophie2014!` a permis de valider l'authentification SSH et d'obtenir un accès à distance sur la machine hôte.

![alt text](image-1.png) et j'ai pu me connecter  ![alt text](image-2.png)

### Étape 3 : Exploration du répertoire Web

 **Commandes utilisées :** ``cd /var/www/html` et `ls -la`
  **Objectif et effet** : Se déplacer dans le répertoire racine du serveur Web Apache (/var/www/html) pour lister le contenu et repérer la structure des fichiers de l'application Web. La commande a révélé la présence du fichier contact.html.

![alt text](image-3.png)

### Étape 4 : Altération de la page de contact 

**Commande utilisée** : `nano contact.html`
**Objectif et effet** : Ouvrir le fichier de la page de contact pour y apporter les modifications requises. Le numéro de téléphone de l'entreprise a été remplacé par 555-555-9876 et le courriel de contact client a été remplacé par ouch.hacked@cem.ca. Les modifications ont ensuite été enregistrées
![alt text](image-4.png)




## Correctif 1

Commandes à effectuer ou étapes à mettre en place. 

Capture d'écran de l'exploit qui ne fonctionne plus.

## Correctif 2

Commandes à effectuer ou étapes à mettre en place.

Capture d'écran de l'exploit qui ne fonctionne plus. 

## Correctif 3

Commandes à effectuer ou étapes à mettre en place. 

Capture d'écran de l'exploit qui ne fonctionne plus.
