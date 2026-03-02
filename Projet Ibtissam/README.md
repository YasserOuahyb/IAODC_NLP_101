# Système d’Extraction de Texte PDF et Correction Grammaticale

## Aperçu
Ce projet implémente un pipeline complet de traitement automatique du langage naturel (NLP) qui extrait le texte à partir de documents PDF, le prétraite et applique une correction grammaticale automatique à l’aide d’un modèle de type transformer séquence-à-séquence.

Le système inclut également une interface interactive permettant la correction de texte en temps réel. Il est adapté au nettoyage de documents, à la normalisation linguistique et au traitement de grands volumes de texte.

---

## Fonctionnalités principales
- Extraction automatique de texte à partir de documents PDF multi-pages  
- Prétraitement et segmentation des textes longs  
- Correction grammaticale via un modèle préentraîné  
- Reconstruction de documents complets corrigés  
- Interface interactive pour la saisie utilisateur en temps réel  
- Architecture modulaire et extensible  

---

## Architecture du système

### 1. Traitement des documents
- Chargement et traitement de documents PDF  
- Extraction du contenu textuel brut  
- Prise en charge des documents multi-pages  

### 2. Prétraitement du texte
- Découpage du texte en segments compatibles avec le modèle  
- Normalisation et nettoyage du contenu  
- Préparation des entrées pour l’inférence  

### 3. Modèle de correction grammaticale
- Architecture transformer séquence-à-séquence  
- Génération du texte corrigé avec décodage par beam search  
- Agrégation des segments corrigés en documents complets  

### 4. Interface utilisateur
- Interface interactive pour test et démonstration  
- Saisie de texte par l’utilisateur  
- Affichage du texte corrigé en temps réel  

---

## Technologies utilisées

### Traitement du langage naturel
- Transformers  
- Sentence Transformers  
- PyTorch  

### Traitement de documents
- PyPDF2  

### Traitement vectoriel et données
- FAISS  

### Interface applicative
- Gradio  

### Environnement de développement
- Python 3  
- Jupyter Notebook  

---

## Structure du projet

project/
│
├── Projet_ibtissam.ipynb      # Notebook principal  
├── data/                      # Jeux de données (PDF et TXT)  
├── models/                    # Modèles sauvegardés  
└── README.md                  # Documentation du projet  

---

## Installation

### 1. Cloner le dépôt
git clone <url-du-repository>  
cd <dossier-du-projet>

### 2. Installer les dépendances
pip install PyPDF2 faiss-cpu sentence-transformers transformers torch gradio

---

## Utilisation
1. Ouvrir le notebook principal : Projet_ibtissam.ipynb  
2. Exécuter toutes les cellules pour initialiser le système  
3. Lancer l’interface interactive  
4. Saisir un texte pour obtenir la version corrigée  

---

## Exemple de workflow
1. Charger les documents PDF  
2. Extraire le contenu textuel  
3. Prétraiter et segmenter le texte  
4. Appliquer le modèle de correction grammaticale  
5. Afficher le résultat corrigé  

---

## Considérations de conception
- Gestion des documents longs par segmentation  
- Séparation claire entre prétraitement, modèle et interface  
- Extensible à d’autres tâches NLP  
- Conçu pour un usage académique et expérimental  

---

## Améliorations futures
- Prise en charge multilingue  
- Téléversement direct de documents via l’interface  
- Export automatique des documents corrigés  
- Ajustement du modèle sur des corpus spécifiques  
- Intégration d’une recherche sémantique  
- Déploiement en tant que service web  

---

## Auteur
Ibtissam

---

## Licence
Projet destiné à des fins académiques et de recherche.
