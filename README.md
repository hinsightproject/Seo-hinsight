# 🔍 Hinsight Audit SEO Tool

Outil d'audit SEO développé pour le MBA2 Expert Marketing Digital — Hinsight.

## 🚀 Installation en 3 commandes

```bash
# 1. Créer un environnement virtuel (recommandé)
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer l'application
streamlit run app.py
```

L'application s'ouvre automatiquement dans le navigateur sur **http://localhost:8501**

---

## ✅ Ce que l'outil analyse

| Axe | Données collectées |
|-----|-------------------|
| **SEO On-Page** | Title (présence, longueur), H1 (présence, unicité), Méta-description, Canonical, Score SEO /100 |
| **Technique** | Statuts HTTP (200/301/302/404), Redirections, Pages noindex, Temps de chargement |
| **Contenu** | Images sans attribut ALT, Nombre de mots, Liens internes/externes |
| **Maillage** | Pages les plus liées, Pages orphelines (0 lien entrant) |
| **Performance** | Score PageSpeed, LCP, CLS, TBT (nécessite une clé API Google gratuite) |

---

## 🔑 Clé API PageSpeed (optionnel mais recommandé)

1. Aller sur [console.cloud.google.com](https://console.cloud.google.com)
2. Créer un projet (gratuit)
3. Activer l'API "PageSpeed Insights API"
4. Créer une clé API dans "Identifiants"
5. Coller la clé dans le champ dédié dans la sidebar

**Quota gratuit** : 25 000 requêtes/jour — largement suffisant.

---

## 📊 Rapport de sortie

- **Excel (.xlsx)** : toutes les données dans un tableau, compatible avec les filtres Excel
- **HTML** : rapport visuel prêt à présenter ou à envoyer au client

---

## ⚙️ Paramètres

| Paramètre | Description | Recommandation |
|-----------|-------------|----------------|
| URL de départ | URL racine du site | https://exemple.fr |
| Nb max d'URLs | Pas de limite ! | 100-500 pour un audit rapide |
| Délai entre requêtes | Respecter le serveur | 0.5s minimum |
| Extensions exclues | Fichiers à ne pas crawler | .pdf,.jpg,.png... |
| Patterns exclus | Parties d'URL à ignorer | /wp-admin,/feed... |

---

## 🛠 Développé par

**Loïs ARMAND — Hinsight**  
lois.armand@hinsight.fr · hinsight.fr
