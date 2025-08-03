### Cours pour maîtriser GIT

# 📘 Introduction à Git – Contrôle de versions

---

## 🧠 Qu’est-ce qu’un gestionnaire de versions ?

Un **gestionnaire de versions** est un outil qui permet de :

- 🗂️ Conserver un **historique** des fichiers (modifications, auteur, date, raison)
- 🔁 **Revenir à une version précédente** en cas d’erreur
- 🤝 **Collaborer à plusieurs** sans écraser le travail des autres

> 💡 L’action de gérer les versions est appelée **versioning** en anglais.

---

## 🧰 Pourquoi utiliser **Git** ?

Git est le système de gestion de versions **le plus utilisé** aujourd’hui. Il est :

- ✅ **Décentralisé** : chaque développeur possède **une copie complète** du projet (fichiers + historique)
- 🧱 **Stable** et rapide, utilisé dans tous les environnements professionnels
- 🛠️ **Indispensable** en entreprise (souvent demandé en entretien)

---

## 📦 Cas concret : Alice & Bob

> Alice et Bob travaillent sur un projet sans Git…

- Alice envoie des fichiers modifiés au client
- Son code **écrase** celui de Bob par erreur
- Bob perd **un mois de travail**

> ❌ Aucun historique, aucune sécurité  
> ✅ **Avec Git**, chacun aurait pu modifier, fusionner et restaurer son travail sans perte.

---

## 🧪 Ce que Git permet de faire

- `git init` : Initialiser un projet sous Git
- `git add` : Ajouter des fichiers à suivre
- `git commit` : Sauvegarder un instantané du code avec un message
- `git log` : Voir l’historique des modifications
- `git restore` : Revenir à une version précédente

---

## 🌐 Quelle est la différence entre **Git** et **GitHub** ?

|                          | **Git**                                      | **GitHub**                                       |
|--------------------------|----------------------------------------------|--------------------------------------------------|
| 🛠️ Logiciel               | Gestionnaire de versions                    | Plateforme d’hébergement de dépôts Git           |
| 💾 Local                  | Travaille sur ta machine                    | Accessible via Internet                         |
| 🔁 Gère les versions      | Oui                                          | Non                                              |
| 📡 Partage en ligne       | Non                                          | Oui (collaboration, sauvegarde distante, etc.)   |

> 🧪 **Git = tu prépares ton code localement**  
> ☁️ **GitHub = tu stockes/partages ce code en ligne**

---

## ✅ Résumé

- Un **gestionnaire de versions** comme Git garde l’historique des fichiers et permet de travailler à plusieurs sans conflit.
- **Git** est local, **GitHub** est en ligne.
- Git est **essentiel** pour tout développeur, analyste ou professionnel en cybersécurité.

---

## ▶️ Prochaine étape : comprendre la différence entre **dépôt local** et **dépôt distant**.


# 🌐 Dépôts Git : Local vs Distant

---

## 📂 Qu’est-ce qu’un dépôt ?

Un **dépôt** (ou *repository* en anglais) est un dossier de projet qui contient **toutes les versions** de ton code, ainsi que leur **historique**.

> Il peut être :
> - **Local** : sur ta machine
> - **Distant** : sur Internet (ex: GitHub)

---

## 💻 Le dépôt **local**

Un dépôt local est **créé sur ton ordinateur**. Il te permet de :

- Sauvegarder différentes **versions** de ton code
- Revenir en arrière si besoin
- Travailler **hors ligne** sans dépendance d’Internet

> 🧁 **Métaphore** : Ton dépôt local, c’est comme un **réfrigérateur** dans lequel tu stockes ton gâteau à chaque étape de sa préparation. Tu ajoutes des éléments, tu stockes, tu ajoutes encore… mais tout reste chez toi.

---

## ☁️ Le dépôt **distant**

Un dépôt distant est **hébergé sur Internet** (GitHub, GitLab, Bitbucket…). Il permet de :

- **Centraliser** le travail de tous les contributeurs
- Travailler à plusieurs sans conflit
- Garder une copie **sécurisée** (sauvegarde)
- Partager ton projet publiquement ou en privé

> 📌 **Bon réflexe** : pousse ton projet vers un dépôt distant dès le début pour éviter toute perte locale (crash disque, vol, etc.)

---

## 🤝 Local vs Distant — Comparatif

|                   | 🖥️ Dépôt Local                         | 🌍 Dépôt Distant                              |
|-------------------|----------------------------------------|-----------------------------------------------|
| Emplacement       | Sur ta machine                         | Sur un serveur distant (Internet ou réseau)   |
| Accessibilité     | Toi uniquement                         | Collaborateurs (en fonction des droits)       |
| Objectif          | Travailler, tester, valider            | Sauvegarder, partager, collaborer             |
| Dépendance        | Aucun accès Internet requis            | Requiert une connexion                        |
| Sauvegarde        | Fragile (dépend de ta machine)         | Fiable (serveurs en ligne)                    |

---

## 🧑‍💻 Pourquoi utiliser les deux ?

> **Le dépôt local est ton espace de travail**, et  
> **le dépôt distant est ton point de synchronisation** avec les autres.

Workflow classique :
1. Tu clones un projet depuis un dépôt distant (GitHub)
2. Tu travailles dessus en local
3. Tu pousses (`push`) tes modifications vers le dépôt distant

---

## 🌍 Où héberger ton code ?

Voici un comparatif des plateformes les plus utilisées :

| Plateforme | Avantages | Inconvénients |
|------------|-----------|----------------|
| **GitHub** | ⭐ Très populaire, interface moderne, réseau social pour devs, parfait pour les portfolios | Propriété Microsoft (certains n’aiment pas) |
| **GitLab** | 🔐 Peut être auto-hébergé, open-source, très complet | Moins grand public que GitHub |
| **Bitbucket** | 📁 Intégration Atlassian (Jira, Trello…), bon pour les équipes | Moins utilisé dans l’open source |

> 💡 **GitHub** est le plus utilisé pour les projets open source et le recrutement.

---

## 🧾 Résumé

- Un **dépôt** est un dossier contenant **le code + l’historique complet** du projet.
- Un **dépôt local** est sur ta machine.
- Un **dépôt distant** est sur Internet (ex : GitHub) — essentiel pour travailler à plusieurs ou sauvegarder ton travail.
- Les **plateformes populaires** sont GitHub, GitLab, Bitbucket.

---

### 🚀 À suivre : Créons ton premier projet **GitHub** pas à pas !


# 🚀 Démarrer un projet avec **GitHub**

---

## 👤 Créer un compte GitHub

GitHub est un service en ligne qui permet d’**héberger tes dépôts distants**.

1. Va sur [github.com](https://github.com)
2. Clique sur **Sign up**
3. Renseigne :
   - Ton **email**
   - Un **mot de passe**
   - Un **nom d'utilisateur**
4. Un code de vérification te sera envoyé par email pour confirmer ton identité.

> 💡 GitHub propose un plan **gratuit** par défaut. Des offres payantes existent pour plus de fonctionnalités (privatisation, équipes, sécurité, etc.).

---

## 🧭 Découvrir l’interface de GitHub

### 🏠 Tableau de bord

Depuis le tableau de bord, tu peux :
- Suivre les **issues** et **pull requests** (modifications proposées)
- Accéder rapidement à tes **repositories**
- Voir l'activité de ta **communauté** (organisations, contributeurs, projets suivis)

---

### 📁 Interface des dépôts

L'onglet **Repositories** te permet de :
- Créer un nouveau dépôt → bouton **Start a project**
- Accéder à tes projets existants

---

### 🙋‍♂️ Profil utilisateur

Tu peux y :
- Modifier tes informations
- Voir un résumé de tes **contributions** (modifications de code, commits, pull requests, etc.)
- Accéder à ton **historique public** d'activité sur GitHub

---

### 🔄 Pull Requests

Les **pull requests** permettent de :
- Proposer des **modifications sur le code**
- Discuter et valider avant de les **fusionner** avec la branche principale

> 📌 Très utile pour le **travail collaboratif** ou l’open source.

---

### 🔍 Explorer des projets

L’onglet **Explore** permet de :
- Trouver des projets open source populaires
- Rechercher des dépôts par **technologie, sujet ou étiquette**
- S’impliquer dans la **communauté GitHub**

---

## 🔐 Sécuriser ton compte avec **Push Protection**

Avant de créer ton premier dépôt, active la fonctionnalité de sécurité GitHub :

1. Clique sur ta **photo de profil** > `Settings`
2. Va dans `Code security and analysis`
3. Active :
   - ✅ **Dependabot alerts**
   - ✅ **Secret scanning**
   - ✅ **Push Protection**

> GitHub analysera automatiquement ton code pour détecter d’éventuelles **informations sensibles** (clés API, secrets, mots de passe).

---

## 🆕 Créer ton premier **repository**

1. Clique sur le bouton ➕ en haut à droite > `New repository`
2. Choisis :
   - **Nom** du dépôt (ex : `OpenclassroomsProject`)
   - **Public** ou **privé**
3. (Facultatif mais recommandé) Coche :
   - ✅ **Add a README**
   - ✅ **Add .gitignore** (selon ton langage)
4. Clique sur `Create repository`

> 🧾 Le fichier **README.md** sert de **présentation du projet** (description, prérequis, installation…).

---

## 🧾 Résumé

- Crée un **compte GitHub** gratuit pour héberger tes projets
- Apprends à naviguer dans l’interface : tableau de bord, dépôts, profil, pull requests
- Active les **fonctionnalités de sécurité**
- Crée ton **premier repository** public ou privé avec un `README.md`
- Prêt pour synchroniser ton code avec **Git**

---

🎉 **Félicitations !** Tu viens de créer ton premier dépôt GitHub.

👉 Prochaine étape : **installer Git sur ton ordinateur et le connecter à GitHub**.

# 🛠️ Installation de Git et création d’un dépôt local

---

## 📥 1. Télécharger et installer Git

👉 Rendez-vous sur [git-scm.com](https://git-scm.com/) pour télécharger Git.

Choisissez la version selon votre système :

- 💻 Windows
- 🍎 macOS
- 🐧 Linux / Unix

### ✅ Étapes d’installation

1. Exécutez le fichier téléchargé
2. Cliquez sur **"Suivant"** à chaque étape
3. Laissez les **options par défaut**
4. Cliquez sur **"Installer"**

> 💡 Sous **Windows**, cochez l’option `Launch Git Bash` à la fin de l’installation  
> Sous **macOS** et **Linux**, utilisez directement votre **terminal**

---

## 💡 2. Git Bash, c’est quoi ?

- **Git Bash** est un terminal pour Windows qui permet d’utiliser Git en ligne de commande.
- Si tu es sur Linux/macOS, ton terminal habituel suffit.

---

## ⚙️ 3. Configurer Git après l’installation

### 👤 Définir ton identité (obligatoire)

```bash
git config --global user.name "Ton Nom"
git config --global user.email "ton@email.com"
