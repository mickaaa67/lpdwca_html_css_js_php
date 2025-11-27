🎨 Chapitre 6 : Personnalisation Bootstrap (Customization)

Bootstrap est très puissant par défaut, mais il est encore plus intéressant quand on adapte son design à sa charte graphique.
Ce chapitre explique comment modifier les couleurs, les boutons, les cartes et combiner CSS perso avec Bootstrap.

🔹 Modifier les couleurs

Bootstrap utilise des variables CSS pour les couleurs et styles principaux.
Tu peux les surcharger pour personnaliser l’apparence.

Exemple :
:root {
  --bs-primary: #0dcaf0;  /* bleu clair */
  --bs-success: #198754;  /* vert */
}


Puis utiliser les classes Bootstrap comme d’habitude :

<button class="btn btn-primary">Bouton primaire personnalisé</button>

🔹 Boutons personnalisés

Tu peux créer des boutons avec dégradé, bordures arrondies, effets hover.

Exemple :
.custom-btn {
  background: linear-gradient(135deg, #0d6efd, #6610f2);
  border: none;
  color: white;
  padding: 12px 30px;
  border-radius: 25px;
  font-weight: 600;
  transition: all 0.3s ease;
}
.custom-btn:hover {
  transform: scale(1.05);
  box-shadow: 0 5px 15px rgba(13, 110, 253, 0.4);
}

<button class="custom-btn">Bouton Gradient</button>

🔹 Cartes personnalisées

Les cartes peuvent aussi être stylisées avec bordures colorées et fonds dégradés.

Exemple :
.custom-card {
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
  border: 2px solid #0d6efd;
  border-radius: 15px;
  padding: 20px;
  text-align: center;
}

<div class="custom-card">
  <h5>Carte avec style personnalisé</h5>
  <p>Cette carte a un fond dégradé et une bordure colorée.</p>
</div>

🔹 Combiner CSS perso et utilitaires Bootstrap

Tu peux mélanger les classes Bootstrap avec ton CSS personnalisé pour plus de flexibilité.

Exemple :
<p class="text-primary fw-bold text-uppercase">
  Texte stylé avec utilitaires et CSS
</p>


text-primary → couleur primaire

fw-bold → texte en gras

text-uppercase → texte en majuscules

⚠️ Bonnes pratiques

Toujours commencer par surcharger les variables Bootstrap pour garder une cohérence globale.

Créer des classes personnalisées pour les composants spécifiques, plutôt que d’écrire trop de styles inline.

Mélanger avec parcimonie les utilitaires Bootstrap pour ne pas alourdir le code.

🎯 Résumé
Élément	Rôle
:root	Définir les variables CSS Bootstrap
.custom-btn	Bouton avec style personnalisé
.custom-card	Carte avec bordure et fond dégradé
Classes utilitaires	Ajouter des effets rapides et cohérents
🚀 Exercice pratique

Personnalise la couleur primaire de Bootstrap.

Crée un bouton avec un dégradé unique.

Crée une carte avec un fond dégradé et une bordure colorée.

Utilise des classes utilitaires pour styliser un texte dans la carte.

📚 Ressources

Documentation Bootstrap - Customization

Variables CSS Bootstrap

Exemples de boutons et cartes Bootstrap personnalisés

Auteurs : Mickael Hoffer
Formation : LP DWCA 2025/2026
© 2025 - Université de Strasbourg