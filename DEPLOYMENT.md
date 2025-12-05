# 🚀 GUIDE DE DÉPLOIEMENT - GITHUB PAGES

## Déployer "Notes en Apesanteur" en Ligne

---

## 📋 ÉTAPES DE DÉPLOIEMENT

### Étape 1 : Accéder aux Paramètres

1. Allez sur votre dépôt GitHub :  
   🔗 **https://github.com/Kaisoueriemmi/N8TINFO_NOTES_EN_APESANTEUR**

2. Connectez-vous à votre compte GitHub si ce n'est pas déjà fait.

3. Cliquez sur l'onglet **"Settings"** (en haut à droite du dépôt).

---

### Étape 2 : Activer GitHub Pages

1. Dans la barre latérale gauche, trouvez et cliquez sur **"Pages"**.

2. Dans la section **"Build and deployment"** :

   - Sous **"Source"**, sélectionnez **"Deploy from a branch"**
   - Sous **"Branch"**, sélectionnez :
     - **Branch** : `main`
     - **Folder** : `/ (root)`
   - Cliquez sur **"Save"**

3. Attendez quelques minutes (généralement 1-3 minutes).

4. Rafraîchissez la page. Vous verrez un message :
   ```
   ✅ Your site is live at https://kaisoueriemmi.github.io/N8TINFO_NOTES_EN_APESANTEUR/
   ```

---

### Étape 3 : Vérifier le Déploiement

1. Cliquez sur le lien fourni par GitHub Pages.

2. Vous devriez voir votre application **"Notes en Apesanteur"** s'afficher immédiatement !

3. Testez les fonctionnalités pour vous assurer que tout fonctionne.

---

## 🎯 URL FINALE

Une fois déployé, votre application sera accessible à :

🌐 **https://kaisoueriemmi.github.io/N8TINFO_NOTES_EN_APESANTEUR/**

---

## 📝 ALTERNATIVE : DÉPLOIEMENT MANUEL

Si vous préférez déployer manuellement via la ligne de commande :

```bash
# Créer une branche gh-pages
git checkout -b gh-pages

# Pousser la branche
git push origin gh-pages

# Retourner sur main
git checkout main
```

Puis activez GitHub Pages en sélectionnant la branche `gh-pages` dans les paramètres.

---

## 🔧 CONFIGURATION AVANCÉE (Optionnel)

### Ajouter un Domaine Personnalisé

Si vous avez un nom de domaine :

1. Dans **Settings → Pages**
2. Sous **"Custom domain"**, entrez votre domaine
3. Configurez les DNS de votre domaine pour pointer vers GitHub Pages

### Forcer HTTPS

GitHub Pages active automatiquement HTTPS. Assurez-vous que la case **"Enforce HTTPS"** est cochée.

---

## 🎨 PERSONNALISATION DU README

Une fois déployé, mettez à jour votre `README.md` pour inclure le lien :

```markdown
## 🌐 Démo en Ligne

Essayez l'application directement :  
🔗 **https://kaisoueriemmi.github.io/N8TINFO_NOTES_EN_APESANTEUR/**
```

---

## 🐛 DÉPANNAGE

### Problème : "404 - Page not found"

**Solution** :

- Vérifiez que la branche `main` est bien sélectionnée dans les paramètres Pages
- Vérifiez que `index.html` est bien à la racine du dépôt
- Attendez quelques minutes supplémentaires

### Problème : "Build failed"

**Solution** :

- Vérifiez les logs dans l'onglet **"Actions"** de votre dépôt
- Assurez-vous qu'il n'y a pas d'erreurs dans `index.html`

### Problème : "Changes not reflected"

**Solution** :

- GitHub Pages met en cache. Attendez 5-10 minutes
- Videz le cache de votre navigateur (Ctrl+Shift+R)
- Vérifiez que vos derniers commits sont bien pushés

---

## ✅ CHECKLIST DE DÉPLOIEMENT

- [ ] Dépôt GitHub créé et code pushé
- [ ] Settings → Pages accessible
- [ ] Source configurée sur "Deploy from a branch"
- [ ] Branch `main` et folder `/ (root)` sélectionnés
- [ ] Bouton "Save" cliqué
- [ ] Attendre 1-3 minutes
- [ ] URL GitHub Pages accessible
- [ ] Application fonctionne correctement
- [ ] README.md mis à jour avec le lien

---

## 🎉 APRÈS LE DÉPLOIEMENT

### Partager le Lien

Vous pouvez maintenant partager :

```
🌐 Application en ligne :
https://kaisoueriemmi.github.io/N8TINFO_NOTES_EN_APESANTEUR/

📦 Code source :
https://github.com/Kaisoueriemmi/N8TINFO_NOTES_EN_APESANTEUR
```

### Mettre à Jour l'Application

Pour mettre à jour l'application déployée :

1. Modifiez `index.html` localement
2. Commitez et pushez :
   ```bash
   git add index.html
   git commit -m "Update application"
   git push
   ```
3. GitHub Pages se mettra à jour automatiquement (1-3 minutes)

---

## 📊 STATISTIQUES DE DÉPLOIEMENT

Une fois déployé, vous pourrez voir dans **Settings → Pages** :

- Nombre de visites
- Dernière mise à jour
- Statut du déploiement

---

## 🏆 AVANTAGES DE GITHUB PAGES

✅ **Gratuit** : Hébergement illimité  
✅ **Rapide** : CDN mondial  
✅ **HTTPS** : Certificat SSL automatique  
✅ **Simple** : Aucune configuration serveur  
✅ **Fiable** : Uptime de 99.9%

---

## 🎯 POUR LE JURY

Une fois déployé, ajoutez le lien dans votre présentation :

```markdown
## 🌐 Démo Live

Testez l'application directement sans installation :
https://kaisoueriemmi.github.io/N8TINFO_NOTES_EN_APESANTEUR/

Aucun serveur. Aucune base de données. Juste du HTML.
C'est ça, la résistance numérique.
```

---

<div align="center">

# 🚀 BONNE MISE EN LIGNE !

**Notes en Apesanteur**

_Le web qui trace, sans traces_

---

Une fois déployé, votre application sera accessible **partout dans le monde** en **< 50ms**.

**14.58 KB. Zéro serveur. 100% en ligne.**

</div>

---

**FIN DU GUIDE DE DÉPLOIEMENT**

_Préparé par Hilox Team - Décembre 2025_
