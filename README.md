# 🔐 Projet : Infrastructure Sécurisée avec Ansible

Ce projet a pour objectif d’automatiser le déploiement, la sécurisation et la maintenance d’un serveur Linux à l’aide d’Ansible.

Il s’inscrit dans une démarche de professionnalisation orientée DevOps, Cloud et Cybersécurité.

---

## 📌 Présentation

L’objectif principal est de mettre en place une infrastructure prête pour un environnement de production.

Le projet permet notamment de :

- Sécuriser l’accès SSH
- Mettre en place un pare-feu
- Protéger contre les attaques par force brute
- Gérer les utilisateurs et privilèges
- Automatiser les sauvegardes
- Superviser les performances système
- Déployer Docker
- Renforcer la sécurité du noyau
- Gérer les fichiers de logs

Toutes ces actions sont automatisées via des playbooks Ansible.

---

## 📁 Architecture du projet

ansible-secure-infra/
├── ansible.cfg
├── group_vars/
├── inventory/
├── playbooks/
│ ├── 01-update.yml
│ ├── 02-ssh-hardening.yml
│ ├── 03-users.yml
│ ├── 04-fail2ban.yml
│ ├── 05-firewall.yml
│ ├── 06-backup-files.yml
│ ├── 07-backup-database.yml
│ ├── 08-docker.yml
│ ├── 09-monitoring.yml
│ ├── 10-disable-services.yml
│ ├── 11-kernel-hardening.yml
│ ├── 12-logrotate.yml
│ └── site.yml
├── roles/
├── scripts/
├── screenshots/
└── README.md


---

## ⚙️ Technologies utilisées

- Ansible
- Linux (Ubuntu / WSL)
- Docker
- Git / GitHub
- UFW
- Fail2Ban
- rsync
- sysstat
- logrotate

---

## 🚀 Installation et utilisation

1.Cloner le dépôt
```bash
git clone https://github.com/SergesBuitoni/ansible-secure-infra.git
cd ansible-secure-infra

2. Installer Ansible
sudo apt update
sudo apt install ansible -y

3. Lancer le déploiement complet
ansible-playbook playbooks/site.yml --ask-become-pass
Cette commande configure automatiquement l’ensemble de l’infrastructure.

📸 Captures d’écran
Déploiement Ansible

Supervision système (htop)

Test Docker

✅ Fonctionnalités principales
Sécurisation complète du serveur

Automatisation des tâches système

Sauvegarde des données

Supervision des performances

Déploiement de conteneurs

Renforcement de la sécurité réseau

Gestion centralisée des logs

📈 Compétences mises en œuvre
Ce projet démontre mes compétences en :

Infrastructure as Code (IaC)

Administration système Linux

Cybersécurité opérationnelle

Automatisation DevOps

Gestion d’environnements cloud

👤 Auteur
Joseph Mboui
Ingénieur Junior DevOps / Cloud / Cybersécurité
