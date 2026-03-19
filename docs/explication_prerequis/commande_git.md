## 🚀 Commandes Essentielles Git

### ♻️ Récupérer et Mettre à jour

- **Cloner un dépôt distant :**

```bash
# Récupérer un code depuis Github ou un lab
git clone <lien_du_repo>
```

- **Mettre à jour le code local :**

```bash
# Mettre à jour la branche actuelle avec les nouveautés du repo
git pull
```

```bash
# Préciser la destination manuellement (optionnel)
git pull origin <la_branche>
```

---

### ➕ Ajouter et Envoyer du code

- **Le cycle de sauvegarde classique :**
    
    ```bash
    # 1. Ajouter le contenu modifié (mettre "." pour prendre tout depuis la racine)
    git add <le_contenu>
    ```
    
    ```bash
    # 2. Enregistrer la modification avec un message
    git commit -m "le commentaire"
    ```
    
    ```bash
    # 3. Pousser le code vers le dépôt distant 
    git push origin <la_destination>
    	# 3.1 Pour push sur la branch main
    	git push
    ```
    

---

### ☑️ Vérifier l'état de son dépôt

- **Gérer ses branches :**
    
    ```bash
    # Lister les branches locales et vérifier sur laquelle on se trouve
    git branch
    ```
    
- **Vérifier l'état de l'espace de travail :**
    
    ```bash
    # Voir les fichiers modifiés, ajoutés ou non suivis avant de faire un commit
    git status
    ```
    

---

### 🧹 Nettoyer les fichiers non suivis

- **Faire du tri en toute sécurité :**
    
    ```bash
    # Simulation : voir quels fichiers/dossiers vont être supprimés (à faire en premier)
    git clean -nd
    ```
    
    ```bash
    # Exécution : nettoyer définitivement les fichiers et dossiers non suivis par Git
    git clean -fd
    ```