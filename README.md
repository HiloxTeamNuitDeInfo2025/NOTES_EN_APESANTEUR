# ✨ Notes en Apesanteur

> _Le web qui trace, sans traces_

Une application web ultra-minimaliste de prise de notes poétique et ludique, conçue pour le défi "Le web qui trace, sans traces". Inspirée par le protocole Gemini, cette application prouve qu'on peut créer une expérience mémorable et utile en moins de 50KB.

---

## 📊 Caractéristiques Techniques

### Contraintes Respectées ✅

| Critère                | Objectif       | Réalisé                    |
| ---------------------- | -------------- | -------------------------- |
| **Poids total**        | < 50 KB        | **33.33 KB** ✨            |
| **Architecture**       | 1 fichier HTML | ✅ Tout inline             |
| **Dépendances**        | Aucune         | ✅ Zéro CDN                |
| **Requêtes**           | 1 seule        | ✅ Fichier unique          |
| **Navigation clavier** | Complète       | ✅ Tous raccourcis         |
| **Accessibilité**      | WCAG AA        | ✅ Contrastes + ARIA       |
| **HTML sémantique**    | Obligatoire    | ✅ `<main>`, `<nav>`, etc. |
| **Terminal**           | Compatible     | ✅ w3m, links              |
| **Persistance**        | localStorage   | ✅ window.storage          |

### Technologies Utilisées

- **HTML5** : Structure sémantique
- **CSS3** : Animations et layout (inline)
- **JavaScript Vanilla** : Logique pure (inline)
- **LocalStorage API** : Persistance des données
- **Fonts système** : Pas de Google Fonts

---

## 🎯 Fonctionnalités

### 1. Gestion de Notes Complète

#### Catégories Prédéfinies

- 💡 **Idées brillantes** : Pour vos éclairs de génie
- 🌙 **Pensées nocturnes** : Réflexions tardives
- 📝 **Journal quotidien** : Chronique de vos journées
- 🔥 **Urgent-ish** : Important (mais pas trop)
- 🎪 **Chaos organisé** : Tout le reste

#### Actions Disponibles

- ✍️ Créer une nouvelle note
- ✏️ Éditer une note existante
- 🗑️ Supprimer une note (avec confirmation poétique)
- 📂 Organiser par catégories (accordéons)
- 🔍 Rechercher dans toutes vos notes

### 2. Mode Focus Intelligent

Le mode focus vous aide à combattre la procrastination :

```
🎯 MODE CONCENTRATION ACTIVE

Écris au moins 50 mots ou...
Un haïku apparaîtra pour te
juger gentiment

Mots écrits: 23/50
[████░░░░░░] 46%
```

**Fonctionnement :**

- Compteur de mots en temps réel
- Barre de progression tous les 25 mots
- Messages d'encouragement tous les 50 mots
- Haïku de félicitation à la sauvegarde

**Exemples d'encouragements :**

- "Vous êtes en feu ! 🔥"
- "Les mots coulent comme une rivière 🌊"
- "Continuez, c'est magnifique ✨"

### 3. Haïkus Poétiques

À chaque sauvegarde, un haïku aléatoire célèbre votre pensée :

```
Note capturée,
Comme un papillon de nuit—
Elle existe enfin 🦋
```

**Collection de 5 haïkus** incluant :

- Papillon de nuit
- Apesanteur
- Galaxie d'étoiles
- Clavier qui chante
- Victoire subtile

### 4. Statistiques Absurdes 📊

Visualisez vos exploits d'écriture avec des métriques amusantes :

```
🏆 VOS EXPLOITS

✍️  Notes créées: 23
    (Champion toutes catégories!)

📚  Mots écrits: 1,847
    = 3.7 pages de roman
    = 6.6 tweets
    = 1.23% d'un article Wikipédia

⏰  Série en cours: 5 jours
    Continue ou le compteur pleure

💾  Poids de ton esprit: 8.2 Ko
```

**Métriques disponibles :**

- Nombre total de notes
- Mots écrits aujourd'hui
- Série de jours consécutifs
- Poids des données (en Ko)
- Comparaisons absurdes aléatoires

### 5. Note Aléatoire 🎲

Redécouvrez vos pensées passées :

```
🎰 NOTE ALÉATOIRE

Tirage en cours...

▓▓▓▓▓▓▓░░░

Note du 12 mars, 23h47:

"Pourquoi les pingouins
ne volent pas? Sont-ils
juste des oiseaux pessimistes?"
```

Parfait pour :

- Retrouver une idée oubliée
- Se remémorer un moment
- Sourire de ses anciennes pensées

### 6. Recherche en Temps Réel 🔍

Filtrez instantanément vos notes :

```
🔍 Rechercher: "motivation"

Résultats trouvés: 8 notes

💡 Idées brillantes (3)
📝 Journal quotidien (5)
```

**Fonctionnalités :**

- Recherche insensible à la casse
- Résultats instantanés
- Compteur de résultats
- Filtrage par catégorie

### 7. Rituel du Soir 🌙

Terminez votre journée avec 3 questions simples :

```
🌙 RITUEL DE FIN DE JOURNÉE

3 questions rapides:

1. Meilleur moment aujourd'hui?
   [________________]

2. Une chose apprise?
   [________________]

3. Demain, je veux...
   [________________]

[Sauvegarder & dormir]

⏱️ Temps estimé: 90 secondes
💾 Journal quotidien: jour 12/365
```

**Avantages :**

- Réflexion quotidienne guidée
- Sauvegarde automatique dans le journal
- Suivi de progression (jours consécutifs)
- Message de bonne nuit personnalisé

### 8. Horodatage Poétique

Au lieu de dates froides, des descriptions évocatrices :

**Exemples :**

- "À l'aube, un mardi de décembre"
- "Tard dans la nuit, un vendredi de mars"
- "L'après-midi, un dimanche de juillet"
- "Aux heures impossibles, un samedi de novembre"

**Plages horaires :**

- 00h-06h : "Aux heures impossibles"
- 06h-09h : "À l'aube"
- 09h-12h : "En matinée"
- 12h : "À midi pile"
- 12h-18h : "L'après-midi"
- 18h-22h : "En soirée"
- 22h-00h : "Tard dans la nuit"

### 9. Export de Données ☁️

Sauvegardez toutes vos notes en JSON :

```json
{
  "categories": {
    "ideas": [...],
    "night": [...],
    "journal": [...],
    "urgent": [...],
    "chaos": [...]
  },
  "stats": {
    "totalWords": 5420,
    "lastAccess": "2025-12-04",
    "streak": 12,
    "dailyWords": 347
  }
}
```

**Format :** `notes-apesanteur-YYYY-MM-DD.json`

### 10. Easter Eggs 🥚

Des surprises cachées pour récompenser votre utilisation :

| Déclencheur                | Easter Egg                       |
| -------------------------- | -------------------------------- |
| 13ème note d'une catégorie | "🍀 Numéro chanceux !"           |
| 100 mots écrits            | "Vous êtes en feu 🔥"            |
| Première visite            | "✨ Bienvenue dans l'apesanteur" |
| Note vide sauvegardée      | Haïku sur le vide                |
| Série de 7 jours           | Message spécial                  |

---

## ⌨️ Raccourcis Clavier

### Raccourcis Globaux

| Raccourci  | Action                       |
| ---------- | ---------------------------- |
| `Ctrl + N` | Nouvelle note                |
| `Ctrl + S` | Sauvegarder la note en cours |
| `Ctrl + F` | Focus sur la recherche       |
| `Escape`   | Fermer modal/annuler         |
| `Tab`      | Navigation entre éléments    |
| `Enter`    | Valider/Ouvrir               |

### Navigation Clavier

- **Boutons** : `Tab` pour naviguer, `Enter` pour activer
- **Accordéons** : `Enter` ou `Espace` pour ouvrir/fermer
- **Notes** : `Enter` pour éditer
- **Modals** : `Escape` pour fermer

### Accessibilité

- **Labels ARIA** : Tous les éléments interactifs
- **Roles** : `navigation`, `dialog`, `region`
- **Focus visible** : Outline bleu sur tous les éléments
- **Screen readers** : Compatible NVDA, JAWS

---

## 🎨 Design & Interface

### Palette de Couleurs

```css
--bg: #fafafa       /* Fond presque blanc */
--text: #1a1a1a     /* Texte presque noir */
--accent: #4a90e2   /* Bleu doux */
--border: #e0e0e0   /* Gris très clair */
--hover: #f0f8ff    /* Bleu très pâle */
--shadow: rgba(0,0,0,.1) /* Ombre subtile */
```

### Typographie

- **Famille** : `system-ui, -apple-system, 'Segoe UI', sans-serif`
- **Taille base** : 16px
- **Line-height** : 1.6
- **Titres** : Font-weight 600

### Animations

Toutes les animations sont subtiles (0.2s ease) :

- **Hover sur notes** : `translateY(-2px)` + ombre
- **Apparition modals** : `slideIn` (0.3s)
- **Toast** : `slideUp` (0.3s)
- **Transitions** : Couleurs, transformations

### Responsive Design

```css
@media (max-width: 600px) {
  /* Toolbar en colonne */
  /* Stats en 1 colonne */
  /* Modal padding réduit */
}
```

---

## 💾 Structure des Données

### Format de Stockage

**Clé localStorage :** `antigravity-data`

```javascript
{
  categories: {
    ideas: [Note, Note, ...],
    night: [Note, Note, ...],
    journal: [Note, Note, ...],
    urgent: [Note, Note, ...],
    chaos: [Note, Note, ...]
  },
  stats: {
    totalWords: Number,      // Total mots écrits
    lastAccess: String,      // Date dernière visite
    streak: Number,          // Jours consécutifs
    dailyWords: Number       // Mots aujourd'hui
  }
}
```

### Objet Note

```javascript
{
  id: Number,           // Timestamp unique
  content: String,      // Contenu de la note
  category: String,     // Catégorie (ideas, night, etc.)
  timestamp: Number,    // Date de création
  wordCount: Number     // Nombre de mots
}
```

### Gestion de la Série

La série de jours consécutifs est calculée automatiquement :

```javascript
// Si dernière visite = hier → streak++
// Si dernière visite > hier → streak = 1
// Réinitialisation dailyWords chaque jour
```

---

## 🚀 Guide d'Utilisation

### Première Utilisation

1. **Ouvrez `index.html`** dans votre navigateur
2. **Message de bienvenue** apparaît en bas à droite
3. **Cliquez sur "✍️ Nouvelle Pensée"** ou `Ctrl+N`
4. **Choisissez une catégorie** dans le menu déroulant
5. **Écrivez votre première note**
6. **Cliquez "💾 Sauvegarder"** ou `Ctrl+S`
7. **Admirez votre haïku** de félicitation ! 🎉

### Créer une Note

```
1. Cliquez sur "✍️ Nouvelle Pensée"
2. Sélectionnez une catégorie :
   💡 Idées brillantes
   🌙 Pensées nocturnes
   📝 Journal quotidien
   🔥 Urgent-ish
   🎪 Chaos organisé
3. Écrivez votre contenu
4. Observez le compteur de mots
5. Recevez des encouragements à 25, 50, 75 mots...
6. Sauvegardez (bouton ou Ctrl+S)
7. Recevez un haïku poétique !
```

### Organiser vos Notes

**Accordéons par catégorie :**

- Cliquez sur l'en-tête pour ouvrir/fermer
- Les notes sont triées par date (plus récente en premier)
- Compteur de notes par catégorie

**Actions sur une note :**

- **Clic sur la note** : Éditer
- **Bouton ✏️** : Éditer
- **Bouton 🗑️** : Supprimer (avec confirmation)

### Rechercher

```
1. Cliquez dans le champ de recherche
2. Tapez votre mot-clé
3. Résultats instantanés
4. Compteur : "🔍 8 résultats trouvés"
5. Cliquez sur une note pour l'éditer
6. Effacez la recherche pour tout réafficher
```

### Voir vos Statistiques

```
1. Cliquez sur "📊 Statistiques"
2. Consultez vos exploits :
   - Notes créées
   - Mots écrits aujourd'hui
   - Série de jours consécutifs
   - Poids de vos données
3. Lisez une comparaison absurde aléatoire
4. Re-cliquez pour masquer
```

### Note Aléatoire

```
1. Cliquez sur "🎲 Surprise"
2. Animation de tirage
3. Une note aléatoire s'affiche
4. Avec sa date poétique
5. Cliquez "Retour" pour fermer
```

### Rituel du Soir

```
1. Cliquez sur "🌙 Rituel du Soir"
2. Répondez aux 3 questions :
   - Meilleur moment aujourd'hui ?
   - Une chose apprise ?
   - Demain, je veux...
3. Cliquez "💾 Sauvegarder & dormir"
4. La note est ajoutée au journal
5. Message de bonne nuit !
```

### Exporter vos Données

```
1. Cliquez sur "☁️ Exporter"
2. Fichier JSON téléchargé automatiquement
3. Format : notes-apesanteur-2025-12-04.json
4. Contient toutes vos notes + statistiques
5. Toast de confirmation
```

---

## 🛠️ Personnalisation

### Modifier les Catégories

Dans le code JavaScript, section `CATEGORIES` :

```javascript
const CATEGORIES = {
  ideas: { name: "💡 Idées brillantes", notes: [] },
  night: { name: "🌙 Pensées nocturnes", notes: [] },
  // Ajoutez vos catégories ici
  custom: { name: "🎨 Ma Catégorie", notes: [] },
};
```

N'oubliez pas de mettre à jour le `<select>` dans le HTML.

### Ajouter des Haïkus

Section `HAIKUS` :

```javascript
const HAIKUS = [
  "Note capturée,\nComme un papillon de nuit—\nElle existe enfin 🦋",
  // Ajoutez vos haïkus ici
  "Votre haïku,\nEn trois lignes poétiques—\nAvec un emoji 🌸",
];
```

### Modifier les Encouragements

Section `ENCOURAGEMENTS` :

```javascript
const ENCOURAGEMENTS = [
  "Vous êtes en feu ! 🔥",
  // Ajoutez vos messages ici
  "Incroyable progression ! 🚀",
];
```

### Changer les Couleurs

Dans le CSS, section `:root` :

```css
:root {
  --bg: #fafafa; /* Votre couleur de fond */
  --text: #1a1a1a; /* Votre couleur de texte */
  --accent: #4a90e2; /* Votre couleur d'accent */
  --border: #e0e0e0; /* Votre couleur de bordure */
  --hover: #f0f8ff; /* Votre couleur de survol */
}
```

---

## 🔧 Dépannage

### Les notes ne se sauvegardent pas

**Problème :** localStorage désactivé ou plein

**Solutions :**

1. Vérifiez que les cookies sont activés
2. Ouvrez la console : `localStorage.getItem('antigravity-data')`
3. Videz le localStorage si nécessaire
4. Vérifiez la limite (généralement 5-10 MB)

### L'application ne charge pas

**Problème :** Erreur JavaScript

**Solutions :**

1. Ouvrez la console (F12)
2. Vérifiez les erreurs
3. Rechargez la page (Ctrl+R)
4. Videz le cache (Ctrl+Shift+R)

### Les raccourcis clavier ne marchent pas

**Problème :** Conflit avec le navigateur

**Solutions :**

1. Vérifiez que vous n'êtes pas dans un champ de texte
2. Certains raccourcis peuvent être réservés par le navigateur
3. Utilisez les boutons à la place

### La recherche ne trouve rien

**Problème :** Recherche sensible à la casse ou caractères spéciaux

**Solutions :**

1. La recherche est insensible à la casse
2. Essayez des mots-clés plus courts
3. Vérifiez l'orthographe
4. Effacez et retapez votre recherche

---

## 📱 Compatibilité

### Navigateurs Supportés

| Navigateur | Version Minimale | Status        |
| ---------- | ---------------- | ------------- |
| Chrome     | 90+              | ✅ Testé      |
| Firefox    | 88+              | ✅ Testé      |
| Safari     | 14+              | ✅ Compatible |
| Edge       | 90+              | ✅ Compatible |
| Opera      | 76+              | ✅ Compatible |

### Navigateurs Textuels

| Navigateur | Status        | Notes              |
| ---------- | ------------- | ------------------ |
| w3m        | ✅ Compatible | Navigation basique |
| links      | ✅ Compatible | Fonctionnel        |
| lynx       | ⚠️ Partiel    | JavaScript limité  |

### Appareils

- **Desktop** : Expérience optimale
- **Tablette** : Responsive, tactile OK
- **Mobile** : Adapté, boutons agrandis
- **Screen readers** : Compatible NVDA, JAWS

---

## 🎓 Philosophie du Projet

### Inspiration Gemini

Ce projet s'inspire du protocole Gemini :

1. **Simplicité** : Un seul fichier, aucune dépendance
2. **Légèreté** : < 50 KB pour tout
3. **Respect de l'utilisateur** : Pas de tracking, pas de pub
4. **Accessibilité** : Navigation clavier, HTML sémantique
5. **Durabilité** : Fonctionne hors ligne, pas d'obsolescence

### Principes de Design

- **Minimalisme fonctionnel** : Chaque élément a un but
- **Poésie utile** : Beau ET pratique
- **Ludification douce** : Encourager sans contraindre
- **Respect du temps** : Chargement instantané
- **Zéro tracking** : Vos données restent chez vous

### Valeurs

✨ **Légèreté** : Moins de code, plus d'impact  
🎨 **Beauté** : Le minimalisme peut être élégant  
🔒 **Vie privée** : Vos pensées vous appartiennent  
♿ **Accessibilité** : Pour tous, sans exception  
🌍 **Durabilité** : Moins de poids = moins de CO₂

---

## 📈 Évolutions Futures (Idées)

### Sans dépasser 50 KB

- [ ] Mode sombre (toggle)
- [ ] Import de données JSON
- [ ] Tri personnalisé des notes
- [ ] Tags personnalisés
- [ ] Filtres multiples
- [ ] Raccourcis clavier personnalisables

### Avec dépendances légères

- [ ] Export en Markdown
- [ ] Export en PDF
- [ ] Synchronisation P2P
- [ ] Chiffrement des notes
- [ ] Partage de notes (QR code)

---

## 🤝 Contribution

Ce projet est un défi personnel, mais les suggestions sont bienvenues !

**Pour contribuer :**

1. Gardez le poids < 50 KB
2. Respectez l'accessibilité
3. Testez sur navigateurs textuels
4. Documentez vos changements
5. Gardez l'esprit poétique !

---

## 📜 Licence

Ce projet est libre de droits. Utilisez-le, modifiez-le, partagez-le comme bon vous semble.

**Conditions :**

- Gardez l'esprit minimaliste
- Respectez la vie privée des utilisateurs
- Partagez vos améliorations

---

## 🙏 Remerciements

- **Protocole Gemini** : Pour l'inspiration
- **Défi "Le web qui trace, sans traces"** : Pour la motivation
- **Vous** : Pour utiliser cette application ! 🎉

---

## 📞 Support

**Problème ?** Consultez la section [Dépannage](#-dépannage)

**Question ?** Relisez le [Guide d'Utilisation](#-guide-dutilisation)

**Suggestion ?** Notez-la dans l'application ! 😉

---

<div align="center">

**✨ Notes en Apesanteur ✨**

_Vos pensées n'ont jamais été aussi légères_

**33.33 KB** | **Zéro tracking** | **100% offline**

---

_Fait avec ❤️ et beaucoup de ⌨️_

_Pour le défi "Le web qui trace, sans traces"_

</div>
