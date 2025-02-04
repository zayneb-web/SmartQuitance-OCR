# SmartQuitance-OCR
Ce projet vise à concevoir et développer une solution évolutive pour la gestion automatisée des quittances d’assurance, intégrant des fonctionnalités avancées basées sur l’OCR (Optical Character Recognition). Cette solution permettra d'extraire, traiter et intégrer les données des quittances existantes pour plusieurs compagnies d’assurance
📌 Modules nécessaires :
Module de traitement OCR
Prétraitement des images (nettoyage, correction de perspective, suppression de bruit, conversion en niveaux de gris)
Extraction des données textuelles depuis l’image via OCR (ex: Tesseract OCR, EasyOCR)
Post-traitement pour améliorer l’exactitude des résultats (correction d’erreurs, validation des données)
Module de gestion des compagnies d’assurance
Interface pour gérer plusieurs compagnies d’assurance
Configuration des spécificités par compagnie (formats de quittance différents, champs obligatoires, etc.)
Gestion des documents extraits et des métadonnées associées
Module de stockage et intégration des données
Base de données SQL (PostgreSQL, MySQL) pour stocker les quittances extraites
API REST pour permettre l'intégration avec d'autres systèmes d’assurance
Sécurisation des données
Module d’interface utilisateur (Dashboard)
Visualisation des quittances traitées
Statistiques sur le nombre de documents traités et le taux d’erreurs
Options d’exportation des données extraites (CSV, PDF, etc.)
📌 Ce que je dois apprendre (étant donné que je ne connais pas l'OCR) :
Comprendre comment fonctionne l'OCR (Tesseract est un bon point de départ)
Expérimenter avec OpenCV pour améliorer la qualité des images avant l'extraction
Tester Tesseract OCR sur des quittances d’assurance pour voir comment extraire les bonnes données
Travailler avec une base de données pour stocker les informations extraites
Construire une API pour gérer et partager ces données avec d’autres systèmes




📌 Architecture générale :
Frontend (Interface Utilisateur) → MERN Stack
React.js : Interface utilisateur
Express.js + Node.js : Gestion des requêtes API
MongoDB / cloudInary : Stockage temporaire des quittances en attente
Backend (Intelligence Artificielle & OCR) → Python/Django
Django REST Framework : API pour communiquer avec MERN
Tesseract OCR +  / OpenCV : Extraction et traitement d'image
MySQL : Base de données principale ( stockage définitif ) 
Admin Panel
Interface d’administration en React.js
Gestion des utilisateurs, statistiques, et logs
