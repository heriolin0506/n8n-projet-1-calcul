Projet 1 : Moteur de Calcul de Facture (n8n + JavaScript)

 Contexte & Problème résolu
Les petites entreprises perdent un temps considérable à faire des calculs manuels, avec un risque d'erreurs humaines. Ce workflow automatise entièrement le processus de facturation en ingérant des données JSON, en calculant les taxes et en appliquant des remises conditionnelles.

✨ Fonctionnalités (Business Logic)
- Ingestion de données : Lecture d'un tableau d'articles (JSON Array) avec quantités et prix.
- Calculs automatiques : Sous-total, TVA (20%), et total final.
- Logique métier (VIP) : Application automatique d'une remise de 5% si le montant dépasse 3 000 000 Ar.
- Formatage : Conversion automatique des montants en devise locale (MGA) avec `Intl.NumberFormat`.
- Routage conditionnel : Séparation des clients VIP et des clients normaux pour le traitement final.

 🛠️ Compétences techniques (Skills)
- n8n Nodes : Manual Trigger, Edit Fields (JSON Mode), Code, If.
- JavaScript : 
  - `Array.reduce()` pour le calcul des totaux.
  - `Intl.NumberFormat()` pour le formatage monétaire.
  - Gestion des erreurs (Error handling).

🧪 Tests & Résultats
- Test Réussi : 
  - Input : 2 articles (Total brut : 3 100 000 Ar).
  - Output : Application de la remise de 155 000 Ar. Le workflow oriente correctement vers la branche "Client VIP".

## 📸 Aperçu du Workflow
*(N'oublie pas de glisser-déposer tes captures d'écran ici dans GitHub)*
