# echographe.ma
📄 Échographe.ma - Automatisation des Attributs Produits dans Odoo
🚀 Description du Projet
Ce dépôt contient un ensemble de scripts et outils permettant de gérer et d’automatiser la mise à jour des attributs et valeurs des produits (échographes) dans un environnement Odoo. Le projet facilite l'intégration de données réelles provenant de sources officielles (constructeurs) et s'adapte dynamiquement aux nouveaux attributs ou caractéristiques des produits.

⚙️ Fonctionnalités Principales
Mise à jour automatique des attributs

Extraction et mise à jour des attributs produits à partir d’un fichier Excel.
Recherche ou Création Dynamique

Création ou mise à jour des attributs et valeurs de produits dynamiquement via l'API XML-RPC d’Odoo.
Adaptabilité Dynamique

Gestion flexible des colonnes pour s’adapter à de nouvelles caractéristiques ajoutées dans le fichier source.
Optimisation des données

Récupération de données réelles depuis des sources validées (constructeurs).
📂 Structure du Projet
scripts/ : Contient les scripts d'intégration et de mise à jour des attributs.

update_product_attributes.py : Script principal pour l'API XML-RPC.
import_excel_to_odoo.py : Script pour le traitement des fichiers Excel.
data/ : Contient les fichiers Excel source.

product_attributes.xlsx : Exemple de fichier avec attributs produits.
config/ : Configuration des paramètres.

odoo_conf.json : Informations d’authentification et de connexion à Odoo.
logs/ : Fichiers de logs pour le suivi des tâches automatisées.

🔧 Prérequis
Environnement Odoo (Version 13 ou 15 recommandée)

Python 3.8+

Librairies Python :

bash
Copy code
pip install pandas xlrd xmlrpc-client
Fichier Excel contenant les attributs produits. Exemple :

yaml
Copy code
| Product Name | Attribute 1 | Attribute 2 | Value 1 | Value 2 |
🛠️ Installation et Configuration
Clonez le dépôt :

bash
Copy code
git clone https://github.com/echographe-ma/odoo_product_update.git
cd odoo_product_update
