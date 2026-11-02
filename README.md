# ERP DS — Marchés publics, achats et logistique

ERP web qui suit le cycle complet des marchés publics d'un fournisseur et importateur d'équipements : de l'appel d'offres jusqu'au paiement, en passant par les achats, les conteneurs et le stock.

> Projet d'équipe chez SINAL (Algérie) — **Fayçal Gheroufella, contributeur principal**. Le code appartient à l'entreprise et reste privé ; démonstration possible en entretien.

## Fonctionnalités

- **Appels d'offres** : clients et organismes, études de faisabilité, pré-soumission et soumission, vue à 360° de chaque marché
- **Marchés** : lots, contrats et exécution, cautions de garantie, échéances et alertes
- **Bureau d'études** : revue des exigences et étude des soumissions
- **Achats et logistique** : commandes, fiches de commande par article, conteneurs maritimes et aériens, certificats, listes de colisage
- **Commercial** : livraisons, paiements partiels, visites
- **Stock** : articles, réceptions de conteneurs, dépôts, étiquettes code-barres / QR, carte 3D de l'entrepôt
- **Pilotage** : chronologie, analyses, rapport hebdomadaire, non-conformités et fiches de suivi
- **Drive documentaire** et administration

## Points techniques

- 145 tables, 18 rôles et environ 165 clés de permission, avec journal d'audit
- Import Excel avec étape de simulation, import en lecture seule des anciennes bases HFSQL via ODBC
- OCR des contrats entièrement hors ligne (Tesseract arabe / français / anglais, traduction Argos)
- API pour n8n sécurisée par jeton, alertes et rappels planifiés, worker d'emails et notifications dans l'application
- Génération PDF par Chrome sans interface, lecteur / générateur XLSX et DOCX maison

## Technologies

PHP 8 · MariaDB 11 · Docker (php-apache + MariaDB via docker-compose) · Bootstrap 5 · Chart.js · three.js · JsBarcode · PHPMailer · n8n · Python (OCR)

## Contact

gheroufellafaycal@gmail.com · [Portfolio](https://faysal12369.github.io/faysal/) · [LinkedIn](https://linkedin.com/in/faysal-gheroufella-4a7969355)
