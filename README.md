# Automatisation de la récupération des avis de CFE

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![Selenium](https://img.shields.io/badge/selenium-3.141.0-green.svg)

Ce script Python utilise Selenium pour automatiser la récupération des avis de Contribution Foncière des Entreprises (CFE) sur le site des impôts français. Il télécharge automatiquement les documents en format PDF et les renomme en utilisant le numéro SIREN et le nom de l'entreprise, facilitant ainsi la gestion documentaire pour les professionnels et le classement dans la GED (Gestion Electronique des Données) du cabinet.

## Fonctionnalités

- Connexion automatique au site des impôts avec des identifiants pré-enregistrés dans le fichier identifiants.txt (il faut renseigner le login et mot de passe).
- Recherche et téléchargement des avis de CFE pour une liste de SIREN qui sont indiqués dans le fichier SIREN.txt
- Renommage automatique des fichiers PDF téléchargés selon le SIREN et le nom de l'entreprise indiqués dans le fichier SIREN.txt.
- Logging des actions pour un suivi facile pour le debuggage.

## Prérequis

- Python 3.8 ou supérieur.
- Selenium WebDriver.
- Google Chrome ou Chromium et ChromeDriver installés.

## Installation

1. Clonez ce dépôt GitHub sur votre machine locale.
3. Assurez-vous que ChromeDriver est installé et accessible dans votre PATH.

## Configuration

1. Modifiez le fichier `identifiants.txt` pour inclure vos identifiants de connexion au site des impôts.
2. Assurez-vous que le fichier `SIREN.TXT` contient la liste des numéros SIREN et des noms d'entreprises à traiter pour lesquels le cabinet a un accès délégué.

## Utilisation

Lancez le script en exécutant :

```shell
python nom_du_script.py
