# Élan Fitness — Documentation des acquis

**Projet :** Amélioration d'un site web de fitness  
**Technologies :** HTML5, CSS3  
**Organisation :** Trello  
**Durée du projet :** 4 jours (du 6 au 9 octobre 2026)

## 1. Quel était le contexte du projet et quels étaient les objectifs ?

Le site Élan Fitness était initialement composé d'une seule page (*One Page*) regroupant toutes les sections.

Mon travail consistait à transformer ce site en un site *Multi Page*. J'ai réparti le contenu existant sur trois pages distinctes : Accueil, Programmes et À propos. Ensuite, j'ai créé une quatrième page, Contact, en essayant de respecter le design et l'identité visuelle du site original.

L'objectif était d'améliorer l'organisation du contenu, de faciliter la navigation et de conserver une cohérence visuelle entre les pages.

## 2. Comment avez-vous analysé le site One Page existant ?

Avant de commencer à modifier le code, j'ai pris le temps d'explorer le site Élan Fitness afin de comprendre son organisation et les différentes sections présentes dans la page unique.

J'ai ensuite identifié les contenus à répartir et déterminé le nombre de pages nécessaires pour transformer le site One Page en site Multi Page.

Une fois cette analyse terminée, je suis passé au code source pour séparer les différentes sections et les organiser dans des fichiers HTML distincts.

## 3. Comment avez-vous organisé votre travail pendant les quatre jours ?

Pour organiser mon travail, j'ai utilisé **Trello** afin de planifier les tâches et de suivre leur avancement.

- **Jour 1 — Mardi :** analyse du projet, début de la transformation du site One Page en plusieurs pages et travail sur un problème lié à GitHub.
- **Jour 2 — Mercredi :** création du logo et travail sur la page Contact.
- **Jour 3 — Jeudi :** finalisation de la page Contact, révision du code et travail sur la documentation et les bonus prévus.
- **Jour 4 — Vendredi :** déploiement sur GitHub Pages et tests du site, avec finalisation de la documentation.

Le planning a évolué : la page Contact a été terminée le troisième jour et le déploiement sur GitHub Pages s'est fait le quatrième. Trello m'a aidé à visualiser les tâches à faire, celles en cours et celles déjà terminées, et à mieux respecter le délai.

## 4. Comment avez-vous conçu l'identité visuelle du site Élan Fitness ?

Pour créer le logo d'Élan Fitness, j'ai utilisé un outil d'**intelligence artificielle (IA)** afin de générer un visuel adapté au domaine du sport et du fitness.

J'ai essayé de respecter les couleurs et l'identité visuelle du site existant pour maintenir une cohérence graphique, notamment avec la nouvelle page Contact.

Cette étape m'a permis de mieux comprendre l'importance de l'identité visuelle et de découvrir l'IA comme outil d'aide à la conception.

## 5. Comment avez-vous structuré les quatre pages avec HTML5 ?

J'ai organisé le site en quatre fichiers HTML distincts :

- `index.html` : accueil ;
- `programmes.html` : programmes ;
- `about.html` : à propos ;
- `contact.html` : contact.

J'ai utilisé des balises sémantiques HTML5 comme `header`, `nav`, `main`, `section` et `footer` pour structurer le contenu.

La barre de navigation et le pied de page sont présents sur les quatre pages. Les liens permettent de passer d'une page à l'autre.

Cette étape m'a aidé à mieux comprendre l'organisation d'un site multipage et l'intérêt des balises sémantiques.

## 6. Comment avez-vous organisé le CSS et assuré le Responsive Design ?

Pour la page Contact, j'ai créé un fichier CSS spécifique, **`app.css`**, afin de gérer ses styles séparément.

J'ai utilisé **Flexbox** pour aligner et organiser les éléments de l'interface. Pour adapter certains styles aux différentes largeurs d'écran, j'ai utilisé des **Media Queries**, par exemple :

```css
@media (max-width: 770px) and (min-width: 410px) {
  /* Styles adaptés à cette plage de largeurs */
}
```

Pour tester les affichages mobiles, je suis passé par l'outil *Inspecter* du navigateur et par l'extension **Mobile Simulator**.

J'ai ainsi approfondi ma compréhension de Flexbox, des Media Queries et des tests responsives.

## 7. Quelles fonctionnalités et interactions avez-vous développées ?

J'ai travaillé sur plusieurs éléments destinés à améliorer l'expérience utilisateur :

- **Formulaire de contact :** interface permettant de saisir des informations et un message ;
- **Google Maps :** intégration d'une carte pour situer la salle ;
- **Navigation mobile :** menu responsive sous forme de sidebar ;
- **Effets CSS :** interactions visuelles avec `:hover` et transitions ;
- **État des éléments :** utilisation de la pseudo-classe `:checked` pour gérer certaines interactions de l'interface.

Ces éléments m'ont permis de pratiquer les interactions réalisables avec HTML et CSS.

> **Précision :** la présence du formulaire est confirmée, mais l'envoi effectif des messages vers un service n'a pas été vérifié.

## 8. Comment avez-vous amélioré l'accessibilité, le SEO et les performances du site ?

J'ai appliqué plusieurs bonnes pratiques :

- ajout d'attributs `alt` aux images ;
- utilisation de balises sémantiques HTML5 ;
- association de `label` aux champs du formulaire ;
- ajout d'un attribut `title` à l'`iframe` Google Maps.

J'ai utilisé **Google Lighthouse** pour évaluer le site et repérer les éléments à améliorer. Voici les scores communiqués pendant le développement :

| Catégorie Lighthouse | Score observé |
| --- | ---: |
| Performance | 95/100 |
| Accessibility | 96/100 |
| Best Practices | 100/100 |
| SEO | 100/100 |

Ces scores proviennent des résultats partagés à différents moments : ils ne correspondent pas nécessairement à un audit unique. Ils ne prouvent pas non plus, à eux seuls, une conformité complète aux normes WCAG ou W3C.

Cette phase m'a appris à utiliser les audits pour identifier des problèmes concrets et mesurer les progrès.

## 9. Quelles difficultés techniques avez-vous rencontrées et comment les avez-vous résolues ?

La principale difficulté a été d'améliorer les résultats de **Lighthouse**, surtout le score d'**accessibilité**. Je cherchais à obtenir les meilleurs scores possibles, idéalement 100/100.

Les audits ont signalé des problèmes, notamment des champs de formulaire sans labels associés, une iframe sans titre et un contraste insuffisant pour certains éléments.

J'ai apporté des corrections au HTML, notamment en ajoutant des labels aux champs concernés et un titre à l'iframe Google Maps. Au cours des tests, le score d'accessibilité est passé de **84/100 à 96/100**.

J'ai compris qu'un site web de qualité ne se limite pas à son apparence : son accessibilité doit aussi être vérifiée.

## 10. Quelles compétences avez-vous acquises et que pourriez-vous améliorer ?

Ce premier projet HTML/CSS m'a surtout permis de progresser dans trois domaines :

- **Accessibilité et Lighthouse :** j'ai appris à lire les résultats d'un audit, à repérer certains problèmes et à améliorer le code en conséquence.
- **Recherche et résolution de problèmes :** j'ai pris l'habitude d'examiner les erreurs et de chercher des corrections adaptées.
- **Organisation du travail avec Trello :** j'ai mieux compris l'intérêt de découper un projet en tâches et de suivre leur état d'avancement.

Pour mes prochains projets, je souhaite surtout **améliorer ma gestion du temps**. Trello m'a été utile pour savoir précisément quelles tâches étaient à faire, lesquelles étaient en cours et lesquelles étaient terminées. Cette visibilité m'a aidé à mieux organiser mon travail et à respecter les délais. Je souhaite continuer à utiliser cette méthode pour anticiper les tâches restantes et mieux gérer les imprévus.

---

## Liens du projet

- **Dépôt GitHub :*https://github.com/AstaAT1/elan-fitness* à renseigner.
- **Site déployé sur GitHub Pages :*https://astaat1.github.io/elan-fitness/* à renseigner.

*Documentation rédigée à partir de mon retour d'expérience sur le projet Élan Fitness.*
