# Gradient-Descent-from-Scratch-Linear-Regression-in-Python
# 📉 - Descente du Gradient

Dans ce mini-projet, nous souhaitons prédire le **bénéfice** d'une entreprise en fonction de la **population** d'une ville à l'aide de la **régression linéaire**. Nous allons implémenter **l'algorithme de descente du gradient** et l'appliquer sur deux jeux de données :
- Univarié : population → bénéfice
- Multivarié : superficie, nombre de chambres → prix d'une maison

---

## 📁 Fichiers

- `data.csv` : données avec population et bénéfice (97 exemples)
- `dataMulti.csv` : données avec superficie, nombre de chambres, et prix (47 exemples)
- `gradient_descent.py` (ou notebook `.ipynb`) : implémentation complète

---

## 🧮 Objectifs pédagogiques

- Implémenter la **fonction de coût** pour la régression linéaire
- Implémenter la **descente du gradient** pour optimiser les paramètres `theta`
- Visualiser les résultats : ligne de régression, courbe de coût
- Normaliser les données dans le cas multivarié
- Comparer avec `scikit-learn`

---

## 📊 Partie 1 - Régression Linéaire Simple (1 variable)

**Données** : Population d'une ville (en milliers) vs Bénéfice (en milliers)

### 🔧 Étapes :

1. Chargement des données
2. Visualisation des données (`scatter plot`)
3. Implémentation de la **fonction de coût** `computeCost`
4. Implémentation de l’**algorithme de descente du gradient**
5. Affichage :
   - de la **fonction hypothèse**
   - du **coût par itération**
6. Prédictions pour :
   - une population de 35 000
   - une population de 70 000

---

## 📈 Partie 2 - Régression Linéaire Multiple (2 variables)

**Données** : Surface (ft²), Nombre de chambres → Prix (en $)

### 🔧 Étapes :

1. Chargement du fichier `dataMulti.csv`
2. Création des matrices X et y
3. **Normalisation des features**
4. Application de la descente du gradient
5. Comparaison **avec et sans normalisation**
6. **Vérification avec `scikit-learn`**

---

## ⚙️ Fonctions implémentées

- `computeCost(X, y, theta)` : calcule le coût de la fonction hypothèse
- `gradientDescent(X, y, theta, alpha, iterations)` : optimise `theta`
- `featureNormalization(X)` : normalise les données pour la régression multiple

---

## 🧠 Renforcement de l’apprentissage

Idées supplémentaires pour approfondir :
- Ajouter la **visualisation du coût en 3D** (surface ou contour)
- Comparer la vitesse de convergence avec différents `alpha`
- Appliquer un **early stopping** si le coût stagne
- Essayer d'autres techniques comme la **descente stochastique**

---

## ✅ Résultats attendus

- Réduction du coût à chaque itération
- Alignement de la ligne de régression sur les données
- Prédictions cohérentes
- Convergence plus rapide avec normalisation

---

## 📚 Bibliothèques utilisées

- `numpy` : calculs matriciels
- `matplotlib` : visualisation
- `scikit-learn` (pour la comparaison finale)

---



