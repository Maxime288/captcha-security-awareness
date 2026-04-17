# 🛡️ Fake CAPTCHA — Security Awareness Simulation

![Static Badge](https://img.shields.io/badge/Purpose-Educational-green)
![Static Badge](https://img.shields.io/badge/Security-Awareness-blue)
![Static Badge](https://img.shields.io/badge/Built%20With-HTML%20%2F%20CSS-orange)
![Static Badge](https://img.shields.io/badge/Attack%20Simulated-ClickFix-red)

> **⚠️ Projet strictement éducatif.** Ce dépôt a pour unique objectif de sensibiliser aux techniques d'ingénierie sociale. Toute utilisation malveillante est illégale et relève de la seule responsabilité de son auteur.

---

## 📝 À propos

Ce projet reproduit fidèlement l'interface visuelle d'un **faux CAPTCHA** de type *ClickFix*, une technique d'ingénierie sociale de plus en plus répandue. En imitant l'apparence d'une vérification de sécurité légitime, ce vecteur d'attaque pousse la victime à **exécuter elle-même une commande malveillante** sur sa machine.

L'objectif est de montrer concrètement, dans un cadre contrôlé, à quel point cette attaque est visuellement crédible — pour mieux apprendre à la reconnaître et à s'en protéger.

---

## 🎯 Vecteur d'attaque simulé : le *ClickFix*

La simulation reproduit les 4 étapes classiques d'une attaque ClickFix :

| Étape | Action demandée à la victime |
|-------|------------------------------|
| 1 | Appuyer sur **⊞ Win + X** pour ouvrir le menu système |
| 2 | Ouvrir le **Terminal** (ou PowerShell) |
| 3 | Coller le contenu du presse-papiers avec **Ctrl + V** |
| 4 | Valider avec **Entrée** |

> **Ce que la victime ne sait pas :** un script malveillant a été copié dans son presse-papiers par la page elle-même. En suivant ces instructions, elle l'exécute avec ses propres droits sur son système.

Après la simulation, l'utilisateur est redirigé vers une page de prévention (`prevention.html`) expliquant ce qui vient de se passer.

---

## 🛠️ Stack technique

- **HTML5** — Structure mimétique d'un widget de vérification (type Google reCAPTCHA)
- **CSS3** — Reproduction des animations de chargement, typographies et interactions (hover, clic)
- **JavaScript vanilla** — Écoute des événements clavier pour déclencher la redirection pédagogique

Aucune dépendance externe. Aucun framework. Un seul fichier `index.html`.

---

## 📁 Structure du projet

```
captcha-security-awareness/
├── index.html        # Simulation du faux CAPTCHA (ClickFix)
└── prevention.html   # Page de sensibilisation post-simulation (à créer)
```

---

## 🚀 Installation & Utilisation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/Maxime288/captcha-security-awareness.git
   cd captcha-security-awareness
   ```

2. Ouvrez `index.html` directement dans votre navigateur — aucun serveur requis.

3. Observez l'interface, suivez les étapes affichées, et constatez la redirection vers la page de prévention.

> **Conseil :** Utiliser ce projet en contexte de formation ou d'atelier de sensibilisation. Présenter la simulation *avant* d'en révéler la nature pour maximiser l'impact pédagogique.

---

## 🧐 Comment reconnaître un faux CAPTCHA ?

| Signal d'alerte | Explication |
|----------------|-------------|
| 🔗 **URL suspecte** | Tout CAPTCHA sur un domaine inconnu doit être considéré comme frauduleux |
| 📋 **Demande de coller du texte** | Aucun CAPTCHA légitime ne vous demande d'utiliser votre presse-papiers |
| 💻 **Instructions clavier inhabituelles** | Un vrai reCAPTCHA ne demande jamais d'ouvrir un terminal |
| 📥 **Téléchargement requis** | Un CAPTCHA qui demande un fichier est 100 % frauduleux |
| 🖼️ **Intégration locale** | Le vrai reCAPTCHA Google s'exécute dans une `<iframe>` hébergée par Google |

---

## 🛡️ Bonnes pratiques de protection

- Installer une extension de sécurité comme **uBlock Origin** pour bloquer les domaines malveillants
- Toujours vérifier le **certificat SSL** et le **nom de domaine** avant d'interagir
- Ne jamais exécuter du contenu copié-collé depuis une page web dans un terminal
- **Sensibiliser** régulièrement les collaborateurs aux attaques de type phishing et ClickFix

---

## ⚖️ Avertissement légal

Ce projet est développé et partagé **à des fins strictement éducatives et préventives**. L'utilisation de ce code pour tromper, nuire ou agir sans le consentement explicite des personnes ciblées est **illégale** dans la plupart des juridictions. L'auteur décline toute responsabilité en cas d'usage détourné.

---

## 👤 Auteur

**Maxime288** — [github.com/Maxime288](https://github.com/Maxime288)
