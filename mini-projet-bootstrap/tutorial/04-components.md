# 🧩 Chapitre 4 : Les Composants Bootstrap (Components)

Bootstrap fournit une large gamme de **composants prêts à l'emploi** pour créer rapidement des interfaces modernes et responsives.  
Ils sont stylisés et interactifs sans écrire beaucoup de CSS ou JavaScript.

---

## 🔹 Buttons (Boutons)

### Classes principales
| Classe | Description |
|--------|-------------|
| `.btn` | Classe de base pour tous les boutons |
| `.btn-primary` | Bouton principal (bleu) |
| `.btn-secondary` | Bouton secondaire (gris) |
| `.btn-success` | Bouton succès (vert) |
| `.btn-danger` | Bouton danger (rouge) |
| `.btn-warning` | Bouton avertissement (jaune) |
| `.btn-info` | Bouton info (cyan) |
| `.btn-light` | Bouton clair |
| `.btn-dark` | Bouton sombre |

### Exemple
```html
<button class="btn btn-primary">Bouton Principal</button>
<button class="btn btn-success">Succès</button>
<button class="btn btn-danger">Danger</button>
🔹 Cards (Cartes)
Les cards permettent d’afficher des contenus regroupés avec style.

Exemple simple
html
Copier le code
<div class="card" style="width: 18rem;">
  <img src="images/photo.jpg" class="card-img-top" alt="Image">
  <div class="card-body">
    <h5 class="card-title">Titre de la Card</h5>
    <p class="card-text">Texte descriptif de la card.</p>
    <a href="#" class="btn btn-primary">Action</a>
  </div>
</div>
Exemple grille de cartes
html
Copier le code
<div class="row row-cols-1 row-cols-md-3 g-4">
  <div class="col">
    <div class="card h-100">
      <img src="images/img1.jpg" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Projet 1</h5>
        <p class="card-text">Description du projet.</p>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card h-100">
      <img src="images/img2.jpg" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Projet 2</h5>
        <p class="card-text">Description du projet.</p>
      </div>
    </div>
  </div>
</div>
🔹 Navbar (Barre de navigation)
La navbar permet de créer des menus responsives facilement.

Exemple
html
Copier le code
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">MonSite</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" href="#">Accueil</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">À propos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
🔹 Forms (Formulaires)
Bootstrap fournit des styles automatiques pour les formulaires :

Exemple simple
html
Copier le code
<form>
  <div class="mb-3">
    <label for="email" class="form-label">Adresse Email</label>
    <input type="email" class="form-control" id="email" placeholder="nom@exemple.com">
  </div>
  <div class="mb-3">
    <label for="message" class="form-label">Message</label>
    <textarea class="form-control" id="message" rows="3"></textarea>
  </div>
  <button type="submit" class="btn btn-primary">Envoyer</button>
</form>
Validation intégrée
html
Copier le code
<form class="needs-validation" novalidate>
  <input type="text" class="form-control" required>
  <div class="invalid-feedback">
    Ce champ est obligatoire.
  </div>
  <button class="btn btn-success" type="submit">Valider</button>
</form>
🔹 Modals (Fenêtres Modales)
Les modales permettent d’afficher du contenu en popup.

Exemple
html
Copier le code
<button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Ouvrir Modal
</button>

<div class="modal fade" id="exampleModal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Titre Modal</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        Contenu de la modal.
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fermer</button>
        <button type="button" class="btn btn-primary">Sauvegarder</button>
      </div>
    </div>
  </div>
</div>
🔹 Alerts, Badges, Breadcrumb
Alerts (Messages)
html
Copier le code
<div class="alert alert-success" role="alert">
  Succès ! Opération effectuée.
</div>
Badges (Étiquettes)
html
Copier le code
<span class="badge bg-primary">Nouveau</span>
Breadcrumb (Fil d’Ariane)
html
Copier le code
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Accueil</a></li>
    <li class="breadcrumb-item"><a href="#">Catégorie</a></li>
    <li class="breadcrumb-item active" aria-current="page">Page</li>
  </ol>
</nav>
🚀 Exercice Pratique
Crée une page avec :

Une navbar en haut

3 cartes avec image et texte

Un formulaire de contact

Un bouton qui ouvre une modal

Test sur mobile, tablette et ordinateur pour vérifier le responsive.

📚 Ressources
Documentation officielle Bootstrap Components

Exemples de Modals Bootstrap

Exemples de Cards Bootstrap

Auteurs : Mickael Hoffer
Formation : LP DWCA 2025/2026
© 2025 - Université de Strasbourg