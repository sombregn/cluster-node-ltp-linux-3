# Nom et Prenom: BAH Alpha Souleymane
# 🚀 Linux, Vagrant, Nginx

Ce projet vise a mettre en place en place de deux VM (web et db) respectivement une bd et et une app spring Boot
Les inter-connecte apres cela installation de toutes les dépendances nécessaires.
Et s'y connecter afin de faire de test !!

---


## 🎯 Objectif
L'objectif de ce projet est de deux VM (web et db) respectivement une Bd et et une app springboot. 

---

## 📦 Prérequis
Avant de commencer, assurez-vous d'avoir les éléments suivants installés sur votre machine :

- **VirtualBox** (Pour la VM) ou tout autres ... 
- **Vagrant** (Pour la gestion de la VM)
- **Git Bash** (Pour exécuter les commandes plus facilement sous Windows) ou autres **PowerShell** etc

---


### 1. Créer un dossier de travail
- **mkdir le nom que vous  voulez**
- **Par exemple: mkdir vagrant-linux**
-**cd nom creer**
- **Par exemple: cd vagrant-linux**
 
 ### 2. Setup du VagrantFile 
 Ajouter le fichier Vagrantfile
- **cmd> vagrant init**
- **Un file vagrant vous sera initialisé automatiquement dans ce file vous travailler.**

### 3. Validation du Vagrant file
-**cmd> vagrant validate**

### 4. Démarrage du Vagrant File:
-**cmd> vagrant up**

### 📌 Ce que fait cette commande :
- **Télécharge l’image Ubuntu 20.04 ou selon la version précisé si elle n’existe pas encore.**
-**Crée et configure la VM.**
-**Installe Nginx et MySQL automatiquement.**
-**Configure Nginx pour servir notre application Angular.**
-**Configure MySQL pour accepter des connexions depuis l’extérieur**

### 🎯 Vérifications après l’installation
**-🔗 1. Se connecter à la VM via SSH**
-**cmd> vagrant ssh**
-**🔥 2. Tester Nginx**
-**Ouvrez un navigateur et entrez** 
-**http://localhost:9190** n'oublions pas le nom de notre port 
-**🗄 3. Accéder à MySQL**
-**mysql -u root -p -h 127.0.0.1 -P 3306**

### 📌 Conclusion**
-**✅ Nous avez maintenant une machine virtuelle sous Ubuntu 20.04 avec Nginx et MySQL configurés**
-**✅ Notre application Angular est servie via Nginx**
-**✅ MySQL est accessible depuis l’extérieur sur le port 3306**
-**✅ Vous pouvez gérer votre serveur avec Vagrant facilement**
-**📝 Remarque**
-**Voir toutes captures dans le dossier captures**

![Capture d’écran 2025-02-25 100418](https://github.com/user-attachments/assets/dc826652-8bd3-49f1-be8b-e4a026a62287)
![image-02 2025-02-18 161856](https://github.com/user-attachments/assets/7c839aef-5af1-440f-8d8f-4b4ca751b8af)
![image-01 2025-02-18 124511](https://github.com/user-attachments/assets/38d189ed-e487-4a71-bc2d-226112020c92)
![Capture d’écran 2025-02-25 104423](https://github.com/user-attachments/assets/b6259327-2686-4c14-bcff-0bbd37771884)

