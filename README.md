# Planning Ménage Partagé — Zone B 🧹

Un planning collaboratif et synchronisé pour gérer un **ménage tournant à 5 personnes** sur **6 mois**, avec **suivi et émargement** en temps réel.

## 🚀 Lien en Direct

**👉 [Ouvrir le planning](https://yaurisey-maker.github.io/Planning-m-nage/)**

## ✨ Fonctionnalités

- 🔄 **Rotation automatique** — Chaque personne change de semaine chaque mois
- 📱 **Responsive** — Fonctionne sur téléphone, tablette, desktop
- 🔗 **Synchronisé en temps réel** — Vos changements apparaissent sur tous les appareils en ~4 secondes
- 💾 **Offline-first** — Marche même sans internet (cache local)
- ✅ **Suivi détaillé** — Date, émargement (initiales), commentaires
- 📋 **Checklist** — ~30 tâches de nettoyage par semaine
- 🖨️ **Imprimable** — Format A4, style print optimisé
- 📤 **Exportable** — Télécharge les données en JSON
- 📥 **Importable** — Charge une sauvegarde précédente

## 👥 Personnes

- **YE** 🟦
- **YA** 🟦
- **AE** 🟦
- **RE** 🟦
- **SE** 🟦

## 🧼 Zone B — Salle de Bain & WC

Le planning couvre le nettoyage de la salle de bain et des WC avec 6 catégories :

| Catégorie | Tâches |
|-----------|--------|
| **Lavabo & robinetterie** | Cuve, rebords, robinets, miroir, tablette |
| **WC** | Cuvette, abattant, extérieur, bouton, balai |
| **Douche / baignoire** | Parois, bac, robinet, joints, porte-savon |
| **Sols** | Balayage, lavage, contour, plinthes |
| **Vitres & surfaces** | Fenêtre, interrupteurs, sèche-serviette |
| **Finitions** | Poubelle, PQ, savon, poussière |

**Conseil** : Ordre recommandé = du plus propre au plus sale (lavabo → surfaces → cuvette → sol). Chiffon dédié WC !

## 📊 Rotation des Mois

| Mois | Sem. 1 | Sem. 2 | Sem. 3 | Sem. 4 | Sem. 5 |
|------|--------|--------|--------|--------|--------|
| 1 | YE | YA | AE | RE | SE |
| 2 | YA | AE | RE | SE | YE |
| 3 | AE | RE | SE | YE | YA |
| 4 | RE | SE | YE | YA | AE |
| 5 | SE | YE | YA | AE | RE |
| 6 | YE | YA | AE | RE | SE |

Chacun change chaque mois, personne ne reste bloqué ! ✨

## 🛠️ Comment Utiliser

### Sur le site
1. Ouvre [le planning](https://yaurisey-maker.github.io/Planning-m-nage/)
2. **Remplis tes infos** :
   - Clique sur « Réalisé le » → entre la date (jj/mm)
   - Clique sur « Émargement » → entre tes initiales
   - Ajoute un commentaire si besoin
3. **Coche les tâches** que tu as faites
4. Les autres verront tes changements en ~4 secondes ✅

### Hors-ligne
- Tout fonctionne sans internet
- Les changements se synchro quand tu reviens en ligne

### Imprimer
- Clique sur **Imprimer** → format A4
- Parfait pour une version papier de référence

### Exporter / Importer
- **Exporter** → télécharge un fichier JSON (sauvegarde)
- **Importer** → recharge une sauvegarde

### Réinitialiser
- Clique sur **Tout effacer** → efface pour tout le monde (confirmation requise)

## 🔧 Stack Technique

- **Frontend** : HTML5 + CSS3 + JavaScript Vanilla (aucune dépendance)
- **Backend** : Supabase PostgreSQL + REST API
- **Déploiement** : GitHub Pages (gratuit, statique)
- **Sync** : Polling toutes les 4s + localStorage

👉 Voir [PROJECT_SUMMARY.md](./PROJECT_SUMMARY.md) pour la documentation technique complète.

## 🎯 État de la Synchronisation

Regarde la pastille en haut à droite :

| Pastille | Sens |
|----------|------|
| 🟢 **Synchronisé** | Connecté à Supabase, données live |
| ⚪ **Local (non partagé)** | Pas de clés Supabase = mode local uniquement |
| 🟡 **Hors-ligne — réessai auto** | Pas d'internet, garde les changements locaux |

## 💡 FAQ

**Q: Quand mes changements sont-ils visibles aux autres ?**  
A: En ~4 secondes max (polling toutes les 4s). Si tu modifies un champ, c'est instantané en local.

**Q: Et si deux personnes éditent en même temps ?**  
A: Le système détecte la dernière édition et n'écrase pas les champs en cours de frappe.

**Q: Mes données sont-elles sauvegardées ?**  
A: Oui ! Dans Supabase (cloud) et en cache local. Elles survivent aux rechargements.

**Q: Puis-je utiliser ça offline ?**  
A: Oui, tout fonctionne avec localStorage. Les changements se synchro quand tu reviens en ligne.

**Q: Comment ça coûte ?**  
A: 0€ ! Supabase free tier + GitHub Pages gratuit.

## 🐛 Problèmes ?

- **Pastille grise (Local)** → Ajoute les clés Supabase dans `index.html`
- **Erreurs console** → Ouvre les DevTools (F12) et regarde la console
- **Données pas synchro** → Attends ~4s, puis rafraîchis

## 📄 Licence

À utiliser librement pour l'équipe ! 🎉

---

**Créé avec ❤️ pour simplifier le ménage partagé.**