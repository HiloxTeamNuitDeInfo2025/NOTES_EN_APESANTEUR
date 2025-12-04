# 🤝 Guide de Contribution

Merci de votre intérêt pour **Notes en Apesanteur** !

Ce guide vous aidera à contribuer efficacement au projet tout en respectant son esprit minimaliste et accessible.

---

## 🎯 Philosophie du Projet

Avant de contribuer, comprenez les valeurs fondamentales :

### Principes Non Négociables

1. **Légèreté** : Le fichier final doit rester < 50 KB
2. **Accessibilité** : Navigation clavier + WCAG AA minimum
3. **Vie privée** : Zéro tracking, zéro collecte de données
4. **Autonomie** : Aucune dépendance externe (pas de CDN)
5. **Durabilité** : Code qui fonctionne dans 10 ans

### Principes Encouragés

- **Poésie** : Petites touches de magie et d'humour
- **Simplicité** : Préférer la solution la plus simple
- **Performance** : Optimiser chaque octet
- **Inclusivité** : Accessible à tous, partout

---

## 🚀 Comment Contribuer

### 1. Types de Contributions Bienvenues

#### 🐛 Corrections de Bugs

- Erreurs JavaScript
- Problèmes d'affichage
- Bugs d'accessibilité
- Incompatibilités navigateurs

#### ✨ Nouvelles Fonctionnalités

- **Petites fonctionnalités** (< 2 KB)
- Améliorations UX
- Easter eggs poétiques
- Optimisations performance

#### 📚 Documentation

- Corrections de typos
- Clarifications
- Traductions
- Exemples d'utilisation

#### 🎨 Design

- Améliorations CSS
- Nouvelles animations (subtiles)
- Thèmes alternatifs
- Responsive design

#### ♿ Accessibilité

- Améliorations ARIA
- Support screen readers
- Contrastes
- Navigation clavier

---

### 2. Processus de Contribution

#### Étape 1 : Fork & Clone

```bash
# Fork le repo sur GitHub
# Puis clonez votre fork
git clone https://github.com/votre-username/notes-apesanteur.git
cd notes-apesanteur
```

#### Étape 2 : Créer une Branche

```bash
# Créez une branche descriptive
git checkout -b feat/ma-super-fonctionnalite

# Ou pour un bug
git checkout -b fix/correction-recherche
```

**Nommage des branches :**

- `feat/` : Nouvelle fonctionnalité
- `fix/` : Correction de bug
- `docs/` : Documentation
- `style/` : CSS/Design
- `refactor/` : Refactoring
- `perf/` : Performance
- `test/` : Tests

#### Étape 3 : Développer

```bash
# Modifiez index.html
# Testez localement
# Vérifiez le poids
```

**Checklist avant commit :**

- [ ] Le fichier fait toujours < 50 KB
- [ ] Navigation clavier fonctionne
- [ ] Contrastes respectent WCAG AA
- [ ] Testé sur Chrome ET Firefox
- [ ] Testé sur mobile (responsive)
- [ ] Aucune erreur console
- [ ] Code commenté si complexe

#### Étape 4 : Commit

```bash
# Commitez avec un message descriptif
git add index.html
git commit -m "feat(notes): Add drag & drop reordering"
```

**Format des commits :**

```
type(scope): description courte

Description détaillée (optionnelle)

Poids: XX.XX KB
```

**Types :**

- `feat`: Nouvelle fonctionnalité
- `fix`: Correction de bug
- `docs`: Documentation
- `style`: CSS/Design
- `refactor`: Refactoring
- `perf`: Performance
- `test`: Tests
- `chore`: Maintenance

**Exemples :**

```
feat(search): Add fuzzy search algorithm
Poids: 34.12 KB

fix(modal): Fix escape key not closing modal
Poids: 33.33 KB

style(buttons): Improve hover animation
Poids: 33.45 KB

docs(readme): Add installation instructions
```

#### Étape 5 : Push

```bash
# Poussez vers votre fork
git push origin feat/ma-super-fonctionnalite
```

#### Étape 6 : Pull Request

1. Allez sur GitHub
2. Cliquez "New Pull Request"
3. Remplissez le template (voir ci-dessous)
4. Attendez la review

---

### 3. Template de Pull Request

```markdown
## Description

[Décrivez votre changement en quelques lignes]

## Type de Changement

- [ ] 🐛 Correction de bug
- [ ] ✨ Nouvelle fonctionnalité
- [ ] 📚 Documentation
- [ ] 🎨 Design/Style
- [ ] ♿ Accessibilité
- [ ] ⚡ Performance

## Checklist

- [ ] Le poids reste < 50 KB (actuel : XX.XX KB)
- [ ] Navigation clavier testée
- [ ] Contrastes WCAG AA respectés
- [ ] Testé sur Chrome
- [ ] Testé sur Firefox
- [ ] Testé sur mobile
- [ ] Aucune erreur console
- [ ] Documentation mise à jour si nécessaire

## Captures d'écran

[Si applicable, ajoutez des captures d'écran]

## Tests Effectués

[Décrivez comment vous avez testé]

## Notes Supplémentaires

[Informations additionnelles pour les reviewers]
```

---

## 🛠️ Guidelines Techniques

### Poids du Fichier

**Impératif :** Rester < 50 KB

**Vérification :**

```powershell
# Windows
Get-Item index.html | Select-Object Name, @{Name="Size(KB)";Expression={[math]::Round($_.Length/1KB,2)}}

# Linux/Mac
ls -lh index.html
```

**Techniques d'optimisation :**

- Minifier le CSS (noms courts, pas d'espaces)
- Minifier le JS (variables courtes)
- Supprimer commentaires inutiles
- Réutiliser les classes CSS
- Éviter la duplication de code

### HTML

**À faire :**

```html
✅
<main>
  ✅
  <nav>
    ✅
    <section>
      ✅ <button aria-label="Fermer">✕</button> ✅
      <div role="dialog" aria-modal="true"></div>
    </section>
  </nav>
</main>
```

**À éviter :**

```html
❌
<div class="main">
  ❌
  <div class="button">
    ❌ <span onclick="..."> ❌ Balises non sémantiques</span>
  </div>
</div>
```

### CSS

**À faire :**

```css
✅ Variables CSS (--accent, --bg, etc.)
✅ Noms de classes courts (.btn, .modal)
✅ Transitions subtiles (0.2s ease)
✅ Mobile-first (@media)
```

**À éviter :**

```css
❌ Noms longs (.my-super-long-class-name)
❌ !important (sauf exception)
❌ Animations lourdes (> 0.5s)
❌ Styles inline dans le HTML
```

### JavaScript

**À faire :**

```javascript
✅ Vanilla JS pur
✅ Fonctions courtes et claires
✅ Noms de variables explicites
✅ Gestion d'erreurs (try/catch)
✅ Commentaires pour code complexe
```

**À éviter :**

```javascript
❌ eval()
❌ innerHTML avec input utilisateur
❌ Variables globales inutiles
❌ Code dupliqué
❌ Dépendances externes
```

### Accessibilité

**Checklist :**

- [ ] Tous les boutons ont un label
- [ ] Navigation au clavier fonctionne
- [ ] Focus visible (outline)
- [ ] Contrastes ≥ 4.5:1 (WCAG AA)
- [ ] Attributs ARIA appropriés
- [ ] Rôles sémantiques
- [ ] Pas de piège clavier

**Test :**

```
1. Débranchez votre souris
2. Naviguez avec Tab, Enter, Escape
3. Toutes les fonctionnalités doivent être accessibles
```

### Performance

**Objectifs :**

- Time to Interactive : < 100ms
- Opérations : < 50ms
- Recherche : < 50ms
- Rendu : < 100ms

**Profiling :**

```javascript
console.time("operation");
// Votre code
console.timeEnd("operation");
```

---

## 🧪 Tests

### Tests Manuels Obligatoires

#### Fonctionnalités

- [ ] Créer une note
- [ ] Éditer une note
- [ ] Supprimer une note
- [ ] Rechercher
- [ ] Voir statistiques
- [ ] Note aléatoire
- [ ] Rituel du soir
- [ ] Exporter données

#### Navigation Clavier

- [ ] Tab : Navigation fluide
- [ ] Ctrl+N : Nouvelle note
- [ ] Ctrl+S : Sauvegarder
- [ ] Escape : Fermer modal
- [ ] Enter : Valider

#### Navigateurs

- [ ] Chrome (dernière version)
- [ ] Firefox (dernière version)
- [ ] Safari (si possible)
- [ ] Edge (si possible)

#### Responsive

- [ ] Desktop (1920x1080)
- [ ] Tablette (768x1024)
- [ ] Mobile (375x667)

#### Accessibilité

- [ ] Lighthouse Accessibility : 100/100
- [ ] Contrastes : WCAG AA minimum
- [ ] Screen reader (NVDA/JAWS si possible)

### Tests Navigateurs Textuels

```bash
# w3m
w3m index.html

# links
links index.html

# Vérifiez que le contenu est lisible
```

---

## 📝 Style de Code

### HTML

```html
<!-- Indentation : 2 espaces -->
<main>
  <section class="categories">
    <div class="category">
      <button>Cliquez-moi</button>
    </div>
  </section>
</main>
```

### CSS

```css
/* Ordre alphabétique des propriétés */
.button {
  background: var(--accent);
  border: none;
  border-radius: 4px;
  color: #fff;
  cursor: pointer;
  padding: 0.6rem 1.2rem;
  transition: all 0.2s ease;
}

/* Mobile-first */
@media (max-width: 600px) {
  .button {
    width: 100%;
  }
}
```

### JavaScript

```javascript
// Fonctions courtes et claires
function countWords(text) {
  return text
    .trim()
    .split(/\s+/)
    .filter((w) => w.length > 0).length;
}

// Commentaires pour code complexe
// Calcule la série de jours consécutifs
function calculateStreak(lastAccess) {
  const today = new Date().toDateString();
  if (lastAccess === today) return streak;

  const lastDate = new Date(lastAccess);
  const todayDate = new Date(today);
  const diffDays = Math.floor((todayDate - lastDate) / (1000 * 60 * 60 * 24));

  return diffDays === 1 ? streak + 1 : 1;
}
```

---

## 🎨 Ajout de Fonctionnalités

### Petites Fonctionnalités (< 2 KB)

**Exemples acceptables :**

- Nouveau haïku
- Nouvel encouragement
- Nouvelle plage horaire poétique
- Nouveau raccourci clavier
- Amélioration animation existante
- Nouveau easter egg

**Process :**

1. Vérifier que ça rentre dans 50 KB
2. Implémenter
3. Tester
4. Pull Request

### Grandes Fonctionnalités (> 2 KB)

**Exemples :**

- Mode sombre
- Import de données
- Tags personnalisés
- Graphiques de stats

**Process :**

1. **Ouvrir une Issue** d'abord pour discussion
2. Attendre validation de la communauté
3. Vérifier impact sur le poids
4. Implémenter si approuvé
5. Pull Request

---

## 🐛 Rapport de Bugs

### Template d'Issue

```markdown
## Description du Bug

[Description claire et concise]

## Étapes pour Reproduire

1. Aller sur '...'
2. Cliquer sur '...'
3. Voir l'erreur

## Comportement Attendu

[Ce qui devrait se passer]

## Comportement Actuel

[Ce qui se passe réellement]

## Captures d'écran

[Si applicable]

## Environnement

- OS: [Windows 11 / macOS 14 / Ubuntu 22.04]
- Navigateur: [Chrome 120 / Firefox 121]
- Version: [1.0.0]

## Console Errors

[Copier les erreurs de la console F12]

## Informations Supplémentaires

[Contexte additionnel]
```

---

## 💡 Demande de Fonctionnalité

### Template d'Issue

```markdown
## Fonctionnalité Demandée

[Description claire]

## Problème Résolu

[Quel problème cette fonctionnalité résout-elle ?]

## Solution Proposée

[Comment l'implémenter ?]

## Alternatives Considérées

[Autres approches possibles]

## Impact sur le Poids

[Estimation : +X KB]

## Compatibilité

- [ ] Respecte la limite de 50 KB
- [ ] Accessible au clavier
- [ ] Fonctionne sur mobile
- [ ] Pas de dépendance externe

## Informations Supplémentaires

[Contexte, exemples, maquettes]
```

---

## 🏆 Reconnaissance

Les contributeurs seront listés dans :

- `README.md` (section Contributeurs)
- `CHANGELOG.md` (pour chaque version)

**Merci à tous les contributeurs !** 🎉

---

## 📞 Questions ?

- **Issues** : Pour bugs et fonctionnalités
- **Discussions** : Pour questions générales
- **Email** : [Si applicable]

---

## 📜 Code de Conduite

### Notre Engagement

Nous nous engageons à faire de la participation à ce projet une expérience exempte de harcèlement pour tout le monde.

### Standards

**Comportements encouragés :**

- ✅ Langage accueillant et inclusif
- ✅ Respect des points de vue différents
- ✅ Acceptation des critiques constructives
- ✅ Focus sur ce qui est meilleur pour la communauté
- ✅ Empathie envers les autres

**Comportements inacceptables :**

- ❌ Langage ou images sexualisés
- ❌ Trolling, insultes, attaques personnelles
- ❌ Harcèlement public ou privé
- ❌ Publication d'informations privées
- ❌ Autre conduite inappropriée

### Application

Les mainteneurs ont le droit de supprimer, éditer ou rejeter les contributions qui ne respectent pas ce code de conduite.

---

## 🙏 Merci !

Merci de contribuer à **Notes en Apesanteur** et de nous aider à créer un web plus léger, plus accessible, plus humain.

Chaque ligne de code compte. Chaque octet compte. Chaque utilisateur compte.

**Ensemble, faisons la différence.** ✨

---

<div align="center">

**🤝 Guide de Contribution v1.0**

_Pour un web meilleur_

</div>
