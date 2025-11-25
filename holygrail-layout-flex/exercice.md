# Exercices Progressifs

## Exercice 1 : Conversion d'une Card Statique

**Objectif** : 
Convertir une card produit traditionnelle utilisant des Media Queries en une version utilisant les Container Queries.
**Contexte** : 
Vous disposez d'une card produit qui fonctionne correctement en responsive grâce aux Media Queries, mais qui pose problème lorsqu'elle est placée dans une sidebar étroite sur un grand écran.
**Consignes** :
Identifier les breakpoints Media Query existants
Convertir chaque breakpoint en Container Query équivalente
Définir le conteneur parent avec container-type: inline-size
Remplacer les @media par des @container
Tester la card dans plusieurs contextes de largeur différents

Code de départ :

```css
css.card {
  padding: 1rem;
  display: flex;
  flex-direction: column;
}

/* Media Query globale basée sur le viewport */
@media (min-width: 768px) {
  .card {
    flex-direction: row;
    padding: 2rem;
  }
}
```