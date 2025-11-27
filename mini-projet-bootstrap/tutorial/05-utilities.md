# 🛠 Chapitre 5 : Les Utilitaires Bootstrap (Utilities)

Bootstrap propose une large gamme de **classes utilitaires** pour gérer rapidement la **mise en page**, **l'espacement**, **les couleurs**, **la typographie**, et bien plus, **sans écrire de CSS**.

---

## 🔹 Espacements : Marges et Padding

Classes principales pour gérer les marges (`m`) et le padding (`p`) :

| Classe | Description | Exemple |
|--------|------------|---------|
| `m-3`  | Marge sur tous les côtés | `margin: 1rem;` |
| `mt-5` | Marge en haut uniquement | `margin-top: 3rem;` |
| `p-2`  | Padding sur tous les côtés | `padding: .5rem;` |
| `px-4` | Padding horizontal | `padding-left/right: 1.5rem;` |

**Exemple HTML :**
```html
<div class="p-3 mb-4 bg-light border">Bloc avec padding et marge</div>
🔹 Couleurs et arrière-plans
Classes pour la couleur du texte et le fond :

Classe	Description
text-primary	Texte bleu
text-success	Texte vert
bg-warning	Fond jaune
bg-dark text-white	Fond sombre avec texte blanc

Exemple HTML :

html
Copier le code
<p class="text-success">Texte vert succès</p>
<div class="bg-warning p-3">Fond jaune avec padding</div>
🔹 Typographie et texte
Quelques utilitaires typographiques utiles :

Classe	Effet
fw-bold	Gras
fst-italic	Italique
text-uppercase	Majuscules
text-center	Centré

Exemple HTML :

html
Copier le code
<p class="fw-bold text-uppercase text-center">Texte en gras et centré</p>
🔹 Affichage et Flexbox
Gestion de l'affichage et du positionnement rapide :

Classe	Effet
d-none	Masquer un élément
d-flex	Flexbox
justify-content-between	Espacement horizontal entre éléments
align-items-center	Alignement vertical des éléments

Exemple HTML :

html
Copier le code
<div class="d-flex justify-content-between align-items-center p-3 bg-light">
  <span>Gauche</span>
  <span>Droite</span>
</div>
🎯 Résumé
Bootstrap Utilities permettent de :

Gérer espacement, couleurs, typographie rapidement

Créer des layouts flexibles sans écrire de CSS

Combiner plusieurs utilitaires pour gagner du temps

🚀 Exercice Pratique
Crée une petite page avec :

Un bloc en bg-primary et texte blanc avec padding p-4

Trois paragraphes : texte success, danger et warning

Une div d-flex justify-content-around avec trois boutons

📚 Ressources :
Documentation Bootstrap Utilities

yaml
Copier le code

---

## 🟣 `06-customization.md`

```markdown
# 🎨 Chapitre 6 : Personnalisation de Bootstrap (Customization)

Bootstrap peut être entièrement **personnalisé** pour correspondre à votre charte graphique ou vos besoins.

---

## 🔹 1. Modifier les couleurs avec CSS

Bootstrap v5 utilise des **variables CSS** :

```css
:root {
  --bs-primary: #0dcaf0;
  --bs-success: #198754;
}
Toutes les couleurs utilisant ces variables s’adaptent automatiquement.

🔹 2. Créer ses propres classes
Vous pouvez ajouter vos styles après Bootstrap pour les prioriser :

css
Copier le code
.custom-btn {
  background: linear-gradient(135deg, #0d6efd, #6610f2);
  color: white;
  border-radius: 8px;
  font-weight: bold;
}
Exemple HTML :

html
Copier le code
<button class="custom-btn">Bouton personnalisé</button>
🔹 3. Surcharge des composants
Vous pouvez également modifier :

Les bordures des cartes

Les paddings et marges par défaut

Les typographies

Exemple HTML :

html
Copier le code
<div class="custom-card p-3 border rounded">
  Carte avec style personnalisé
</div>
🔹 4. Combiner utilitaires + CSS perso
Les utilitaires Bootstrap peuvent être combinés avec vos propres classes :

html
Copier le code
<p class="text-primary fw-bold text-uppercase">
  Exemple de texte stylé
</p>
🔹 5. Personnalisation avancée (optionnelle)
Pour les développeurs avancés :

Modifier les variables SCSS avant compilation

Créer un fichier _custom.scss

Compiler via Sass ou Vite

🎯 Résumé
Variables CSS → facile pour couleurs globales

Classes perso → surcharge rapide

Flexibilité → combiner Bootstrap et CSS personnalisé

🚀 Exercice Pratique
Redéfinis la couleur primaire (--bs-primary)

Crée un bouton gradient avec .custom-btn

Personnalise une card avec bordure et fond dégradé

📚 Ressources :
Bootstrap Theming

Auteurs : Mickael Hoffer
Formation : LP DWCA 2025/2026
© 2025 - Université de Strasbourg