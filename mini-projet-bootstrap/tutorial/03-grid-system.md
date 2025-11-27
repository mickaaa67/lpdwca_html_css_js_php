# 🧱 Chapitre 3 : Le Système de Grille (Grid System)

Le **système de grille** est le cœur du framework **Bootstrap**.  
C’est lui qui rend le **responsive design** si simple à mettre en place.

Grâce à lui, tu peux facilement créer des **mises en page flexibles** s’adaptant à toutes les tailles d’écran — du smartphone à l’écran 4K.

---

## 🔍 Principe de Base

Bootstrap utilise une **grille de 12 colonnes**.

Chaque ligne (`.row`) peut contenir jusqu’à **12 unités** de largeur totale.  
Si la somme dépasse 12, la colonne suivante passe automatiquement à la ligne.

### Exemple :
```html
<div class="container">
  <div class="row">
    <div class="col-4 bg-primary text-white">Col 1 (4)</div>
    <div class="col-4 bg-success text-white">Col 2 (4)</div>
    <div class="col-4 bg-danger text-white">Col 3 (4)</div>
  </div>
</div>
✅ Résultat : 3 colonnes de taille égale (4 + 4 + 4 = 12).
Si tu mettais col-6 col-6 col-6, la 3e passerait automatiquement à la ligne.

🧩 Les Classes Principales
Classe	Description
.container	Conteneur principal qui centre le contenu
.container-fluid	S’étend sur toute la largeur
.row	Crée une ligne de la grille
.col	Crée une colonne flexible
.col-*	Définit une largeur fixe (1 à 12)
.col-sm-*, .col-md-*, .col-lg-*, .col-xl-*	Définissent les tailles selon les écrans

📱 Les Points de Rupture (Breakpoints)
Taille d’écran	Classe	Exemple	Description
Extra small	col-	.col-12	Téléphones (<576px)
Small	col-sm-	.col-sm-6	Tablettes (>576px)
Medium	col-md-	.col-md-4	Ordinateurs portables (>768px)
Large	col-lg-	.col-lg-3	Écrans larges (>992px)
Extra large	col-xl-	.col-xl-2	Très grands écrans (>1200px)

🧮 Exemple Complet Responsive
html
Copier le code
<div class="container text-center mt-4">
  <div class="row">
    <div class="col-sm-12 col-md-6 col-lg-3 bg-primary text-white p-3">Bloc 1</div>
    <div class="col-sm-12 col-md-6 col-lg-3 bg-success text-white p-3">Bloc 2</div>
    <div class="col-sm-12 col-md-6 col-lg-3 bg-warning text-dark p-3">Bloc 3</div>
    <div class="col-sm-12 col-md-6 col-lg-3 bg-danger text-white p-3">Bloc 4</div>
  </div>
</div>
✅ Sur mobile : 4 lignes empilées
✅ Sur tablette : 2 colonnes par ligne
✅ Sur PC : 4 colonnes côte à côte

🧭 Espacement et Alignement
🔸 Marges internes et externes
Bootstrap utilise les classes utilitaires pour la marge (m) et le padding (p) :

Classe	Signification	Exemple
m-3	Marge sur tous les côtés	margin: 1rem;
mt-5	Marge en haut uniquement	margin-top: 3rem;
p-2	Padding sur tous les côtés	padding: .5rem;
px-4	Padding horizontal	padding-left/right: 1.5rem;

🔸 Alignement vertical et horizontal
Tu peux aligner facilement tes colonnes avec Flexbox intégré à la grille :

html
Copier le code
<div class="row align-items-center justify-content-between">
  <div class="col-4 bg-primary text-white p-3">Bloc A</div>
  <div class="col-4 bg-success text-white p-3">Bloc B</div>
</div>
align-items-center → aligne verticalement

justify-content-between → espace horizontalement

🧰 Grille imbriquée (Nested Grid)
Tu peux imbriquer une grille à l’intérieur d’une autre colonne :

html
Copier le code
<div class="container">
  <div class="row">
    <div class="col-8 bg-light border">
      <div class="row">
        <div class="col-6 bg-info p-2">Sous-col 1</div>
        <div class="col-6 bg-secondary text-white p-2">Sous-col 2</div>
      </div>
    </div>
    <div class="col-4 bg-warning p-2">Colonne latérale</div>
  </div>
</div>
🧭 Exemple Pratique : Mise en page de base
html
Copier le code
<div class="container mt-5">
  <header class="row bg-dark text-white p-3">
    <div class="col">En-tête</div>
  </header>

  <main class="row">
    <aside class="col-md-3 bg-light p-3">Menu</aside>
    <section class="col-md-9 p-3">Contenu principal</section>
  </main>

  <footer class="row bg-secondary text-white p-3">
    <div class="col">Pied de page</div>
  </footer>
</div>
💡 Astuce : Cette structure est parfaite pour un site vitrine ou un blog.

⚠️ Erreurs Courantes
Erreur	Correction
Oublier .row avant les colonnes	Toujours placer les .col dans une .row
Mettre plus de 12 colonnes dans une ligne	Respecter la règle : somme ≤ 12
Oublier .container	Sans lui, la grille ne sera pas centrée
Mélanger les tailles (col-md et col-sm) sans cohérence	Toujours du plus petit au plus grand

🎯 Résumé
Élément	Rôle
.container / .container-fluid	Conteneur principal
.row	Ligne de la grille
.col / .col-*	Colonnes flexibles
col-sm, col-md, col-lg	Responsive adaptatif
m-*, p-*	Marges et espacements

🚀 Exercice Pratique
Crée une page de profil responsive :

1 ligne d’en-tête sur toute la largeur

2 colonnes : photo (4/12) + texte (8/12)

3 cartes de projets en dessous (col-md-4 chacune)

👉 Vérifie que sur mobile, tout s’empile correctement.

📚 Ressources
Documentation officielle Bootstrap Grid

Flexbox sur MDN Web Docs

Exemples de grilles Bootstrap sur CodePen

Auteurs : Mickael Hoffer
Formation : LP DWCA 2025/2026
© 2025 - Université de Strasbourg