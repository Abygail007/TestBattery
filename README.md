# 🔋 TestBattery - Diagnostic Professionnel de Batterie Windows

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Downloads](https://img.shields.io/github/downloads/Abygail007/TestBattery/total.svg)

**Outil portable autonome pour mesurer l'autonomie réelle de votre batterie et suivre son état de santé**

[📥 Télécharger](#-téléchargement) • [📖 Documentation](#-documentation) • [🚀 Démarrage rapide](#-démarrage-rapide) • [💼 Cas d'usage](#-cas-dusage-professionnels)

![TestBattery Dashboard](https://via.placeholder.com/800x450/667eea/ffffff?text=TestBattery+Dashboard)

</div>

---

## ✨ Pourquoi TestBattery ?

### Le problème

- ❓ Votre batterie se vide trop vite ?
- 🤔 Windows affiche "2h restantes" mais vous n'avez que 45 minutes ?
- 😠 Impossible de savoir si votre batterie est vraiment HS ?
- 💼 Vous devez diagnostiquer des batteries de PC clients/reconditionnés ?

### La solution

**TestBattery** vous donne des **mesures objectives et précises** de l'autonomie réelle de votre batterie, avec un dashboard professionnel et un historique complet.

---

## 🎯 Fonctionnalités

### Dashboard moderne

<table>
<tr>
<td width="50%">

#### 📊 Statistiques en temps réel
- **Santé globale** de la batterie (%)
- **Capacité d'origine** vs actuelle
- **Nombre de cycles** de charge
- **Dernière durée** de test mesurée

</td>
<td width="50%">

#### 📈 Graphiques visuels
- Charge actuelle en temps réel
- Évolution de la santé
- Perte de capacité calculée
- Historique des tests

</td>
</tr>
</table>

### Test d'autonomie complet

1. **Démarrage en un clic** - Lancez le test depuis le dashboard
2. **Mesure automatique** - Chrono qui démarre dès que vous déb ranchez le secteur
3. **Snapshots PDF** - Captures automatiques de l'état tout au long du test
4. **Résultats précis** - Durée totale et durée pure sur batterie

### Historique et suivi

- 📁 **Un dossier par machine** (nom PC + serial BIOS)
- 💾 **Stockage JSON** pour export/analyse
- 📄 **Snapshots PDF** horodatés
- 🗑️ **Gestion de l'historique** (suppression sélective)

---

## 💻 Captures d'écran

<details>
<summary>🖼️ Voir les captures</summary>

### Dashboard principal
![Dashboard](https://via.placeholder.com/800x450/667eea/ffffff?text=Dashboard+Principal)

*Interface moderne avec gradient violet, cards arrondies, et statistiques claires*

### Overlay de test
![Test Overlay](https://via.placeholder.com/800x450/667eea/ffffff?text=Test+en+cours)

*Écran de test plein écran avec chrono géant et infos batterie en direct*

### Historique détaillé
![Historique](https://via.placeholder.com/800x450/667eea/ffffff?text=Historique+des+tests)

*Tous vos tests et snapshots avec actions rapides*

</details>

---

## 📥 Téléchargement

### Version portable (recommandée)

**Télécharger la dernière version** : [TestBattery.exe](https://github.com/Abygail007/TestBattery/releases/latest)

📦 **Taille** : ~1.4 MB
✅ **Aucune installation requise**
✅ **Aucune dépendance externe**
✅ **100% portable**

### Configuration minimale

- **OS** : Windows 10 ou Windows 11
- **Architecture** : 64-bit
- **RAM** : 512 MB minimum
- **Espace disque** : 10 MB

---

## 🚀 Démarrage rapide

### Installation

1. **Télécharger** `TestBattery.exe`
2. **Créer un dossier** (ex: `C:\Tools\TestBattery\`)
3. **Placer l'EXE** dans le dossier
4. **Double-cliquer** sur l'EXE

C'est tout ! 🎉

### Premier test

```
1. Branchez votre PC sur secteur
2. Chargez la batterie à 100%
3. Lancez TestBattery.exe
4. Cliquez sur "Démarrer le test"
5. Débranchez l'alimentation secteur
6. Laissez le PC se décharger complètement
7. Rebranchez et consultez les résultats !
```

### Paramètres avancés

```powershell
# Mode simulation (pour tests sans débrancher)
TestBattery.exe -ForceBattery

# Désactiver les snapshots automatiques
TestBattery.exe -NoHtml

# Modifier l'intervalle des snapshots (en secondes)
TestBattery.exe -HtmlEverySeconds 10
```

---

## 📖 Documentation

### Interprétation des résultats

| Santé globale | État | Action |
|--------------|------|--------|
| **90-100%** | ✅ Excellente | Batterie comme neuve |
| **70-89%** | 🟢 Bonne | Dégradation normale |
| **50-69%** | 🟡 Moyenne | Surveiller l'évolution |
| **30-49%** | 🟠 Faible | Remplacement à prévoir |
| **< 30%** | 🔴 Critique | Remplacement urgent |

### Raccourcis clavier

- **F12** - Snapshot manuel pendant le test
- **Échap** - Retour au dashboard (annule le test)

### Organisation des fichiers

```
TestBattery.exe           # Exécutable portable
History/                  # Dossier créé automatiquement
└── [NomPC_Serial]/      # Un dossier par machine
    ├── machine.json     # Informations machine
    ├── Entries/         # Tests et snapshots
    │   ├── test1.json
    │   └── snapshot1.json
    └── battery-report.html  # Rapport Windows
```

---

## 💼 Cas d'usage professionnels

### 🔧 Techniciens SAV

**Diagnostic batterie objectif pour clients**
- Mesure précise de l'autonomie réelle
- Génération de rapports PDF professionnels
- Historique complet pour suivi garantie

### 🏢 Reconditionnement PC

**Tri et valorisation des batteries**
- Test rapide de l'état de chaque batterie
- Classification automatique (bon/moyen/mauvais)
- Export des données pour inventaire

### 🏭 Parc informatique

**Maintenance préventive des laptops**
- Suivi régulier de l'état des batteries
- Anticipation des remplacements
- Rapports d'état consolidés

### 🔬 Laboratoires de test

**Tests comparatifs et benchmarks**
- Protocole standardisé reproductible
- Mesures objectives et traçables
- Documentation complète des tests

---

## 🎨 Interface

### Design moderne

- **Gradient violet** (#667eea → #764ba2) élégant
- **Cards blanches** arrondies avec ombres portées
- **Typographie Segoe UI** claire et lisible
- **Emojis** pour visualisation rapide
- **Responsive** et adaptable

### Expérience utilisateur

- ✅ Interface intuitive
- ✅ Feedback visuel en temps réel
- ✅ Actions rapides (1 clic)
- ✅ Navigation fluide
- ✅ Pas de configuration complexe

---

## ❓ FAQ

<details>
<summary><strong>Dois-je installer quelque chose ?</strong></summary>

Non ! TestBattery est **100% portable**. Il suffit de télécharger l'EXE et de double-cliquer dessus. Aucune installation, aucun setup, aucune dépendance.
</details>

<details>
<summary><strong>Le test abîme-t-il ma batterie ?</strong></summary>

Non. Le test consiste simplement à mesurer le temps de décharge naturelle. C'est exactement ce qui se passe quand vous utilisez normalement votre PC sur batterie.
</details>

<details>
<summary><strong>Combien de temps dure un test ?</strong></summary>

Ça dépend de l'autonomie de votre batterie ! Entre 1h (batterie très dégradée) et 10h+ (batterie neuve avec faible utilisation). Le test se termine automatiquement quand la batterie est vide.
</details>

<details>
<summary><strong>Puis-je utiliser mon PC pendant le test ?</strong></summary>

Oui ! Mais pour des résultats reproductibles, il est recommandé d'avoir une charge de travail constante (ex: navigation web légère).
</details>

<details>
<summary><strong>Où sont stockées mes données ?</strong></summary>

Dans le dossier `History/` créé automatiquement à côté de l'EXE. Toutes les données sont en local, rien n'est envoyé sur internet.
</details>

<details>
<summary><strong>Puis-je supprimer l'historique ?</strong></summary>

Oui, chaque test et snapshot a un bouton "Suppr" dans le dashboard. Vous pouvez aussi simplement supprimer le dossier `History/` pour tout effacer.
</details>

<details>
<summary><strong>Le logiciel est-il gratuit ?</strong></summary>

Oui, TestBattery est **100% gratuit** et open-source (licence MIT). Vous pouvez l'utiliser librement, même en contexte professionnel.
</details>

---

## 🔗 Liens utiles

- 📦 **Releases** : [Télécharger l'EXE](https://github.com/Abygail007/TestBattery/releases)
- 💻 **Code source** : [GitHub](https://github.com/Abygail007/TestBattery-Source)
- 🐛 **Signaler un bug** : [Issues](https://github.com/Abygail007/TestBattery/issues)
- 💬 **Discussions** : [GitHub Discussions](https://github.com/Abygail007/TestBattery/discussions)

---

## 📜 Licence

MIT License - Copyright (c) 2025 Logicia / Jean-Mickael Thomas

Vous êtes libre de :
- ✅ Utiliser le logiciel à des fins commerciales
- ✅ Modifier le code source
- ✅ Distribuer le logiciel
- ✅ Utiliser en privé

---

## 🙏 Remerciements

- **PowerShell** - Langage de développement
- **WPF** - Framework d'interface graphique
- **ps2exe** - Compilation PowerShell → EXE
- **wkhtmltopdf** - Génération des PDF

---

## 📊 Stats

![GitHub all releases](https://img.shields.io/github/downloads/Abygail007/TestBattery/total)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/Abygail007/TestBattery)
![GitHub stars](https://img.shields.io/github/stars/Abygail007/TestBattery?style=social)

---

<div align="center">

**Développé avec ❤️ par [Logicia Informatique](https://github.com/Abygail007)**

[⬆ Retour en haut](#-testbattery---diagnostic-professionnel-de-batterie-windows)

</div>
