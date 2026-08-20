# SchoolSafe Website — Design de refonte complète

Date : 2026-08-20

## Objectif

Refondre le site vitrine public SchoolSafe sans toucher à l’application métier SchoolSafe. Le site doit présenter SchoolSafe comme une solution professionnelle de gestion scolaire, sécurité des élèves et relation parent-école, avec une identité forte et une signature visible : **SchoolSafe by PRODELI S.A.R.L.U.**

Le site reste statique, hébergé sur GitHub Pages, accessible via `schoolsafe1.cc.cd`, rapide, responsive, bilingue FR/EN et sans dépendance lourde.

## Principes de marque

- Marque principale : **SchoolSafe**.
- Signature institutionnelle : **SchoolSafe by PRODELI S.A.R.L.U.**
- Slogan : **Un enfant protégé, un parent informé.**
- Palette : bleu profond / bleu électrique / or / blanc.
- Le logo SchoolSafe reste dominant.
- Le logo PRODELI apparaît comme société porteuse, sans concurrencer visuellement SchoolSafe.
- Les deux logos doivent être affichés sans recadrage destructif (`object-fit: contain`).

## Architecture de la page

### 1. Navigation

Navigation sticky, compacte et lisible :
- Accueil
- Solution
- Sécurité
- Profils
- PRODELI
- Contact
- Sélecteur FR / EN

Sur mobile : menu hamburger accessible, fermeture automatique après sélection.

### 2. Hero / accueil

Le hero doit immédiatement répondre à trois questions :
- Qu’est-ce que SchoolSafe ?
- À qui cela sert ?
- Pourquoi est-ce différent ?

Contenu principal :
- SchoolSafe
- « Un enfant protégé, un parent informé. »
- « SchoolSafe by PRODELI S.A.R.L.U. »
- Titre principal : gestion scolaire + sécurité + relation parent-école
- CTA principal : « Découvrir SchoolSafe »
- CTA secondaire : « Demander une présentation »

Le logo SchoolSafe doit être bien visible sans être recadré.

### 3. Piliers de la solution

Quatre cartes :
- Gestion scolaire
- Sécurité des élèves
- Suivi pédagogique
- Relation parent-école

Les descriptions doivent rester factuelles et correspondre aux fonctionnalités réellement documentées.

### 4. Sécurité et QR

Section visuelle forte expliquant :
- QR élève
- entrée
- sortie
- personnes autorisées
- historique / traçabilité
- alertes et incidents

Aucun discours ne doit laisser entendre qu’un contrôle visuel frontend constitue la sécurité : cette section reste une présentation produit publique.

### 5. Profils utilisateurs

Présenter clairement :
- Direction
- Enseignant
- Parent / Tuteur
- Caisse
- Gardien / Sécurité

Chaque carte décrit uniquement les fonctions utiles à ce profil.

### 6. Fonctionnalités complémentaires

Ajouter une section plus structurée pour montrer l’étendue de SchoolSafe :
- élèves et classes
- présences et retards
- devoirs et notes
- reçus et suivi des paiements enregistrés par l’école
- contrôle des frais par QR
- personnes autorisées
- sorties et historique
- rapports opérationnels
- notifications in-app
- documents scolaires
- Digital Lab / informatique pratique, présenté comme dispositif selon contrat

Éviter les promesses non encore garanties techniquement.

### 7. PRODELI

Section institutionnelle :
- nouveau logo PRODELI officiel
- « SchoolSafe by PRODELI S.A.R.L.U. »
- PRODELI présentée comme société porteuse du projet
- lien externe vers `https://prodeli-sarlu.cc.cd` dans un nouvel onglet avec `rel="noopener noreferrer"`

### 8. Contact

CTA final professionnel :
- `contact@schoolsafe1.cc.cd`
- téléphone public `0828432689`
- Kinshasa, République Démocratique du Congo

Les boutons téléphone et e-mail doivent fonctionner sur mobile.

### 9. Footer

Le footer doit contenir :
- logo SchoolSafe
- SchoolSafe by PRODELI S.A.R.L.U.
- slogan
- lien vers PRODELI
- copyright dynamique ou mis à jour

## Bilingue FR / EN

Tous les textes visibles hors noms propres doivent être traduits via `assets/js/main.js` ou un module de traduction dédié.

Exigences :
- FR par défaut
- choix mémorisé dans `localStorage`
- boutons FR/EN accessibles
- aucun texte important laissé uniquement en français lors du passage en anglais

## Responsive

Le site doit être utilisable à partir de 320 px de largeur.

Points à vérifier :
- logo non coupé
- titre non débordant
- boutons pleine largeur sur petit mobile lorsque nécessaire
- cartes empilées proprement
- navigation mobile utilisable au doigt
- aucune barre de défilement horizontale

## Accessibilité

- `lang` correct sur `<html>`
- contrastes suffisants
- textes alternatifs pour logos
- focus clavier visible
- `aria-expanded` sur menu mobile
- liens et boutons distinguables
- support `prefers-reduced-motion`

## SEO et partage

Mettre à jour :
- `<title>`
- meta description
- canonical `https://schoolsafe1.cc.cd/`
- Open Graph
- favicon
- `robots.txt`
- `sitemap.xml`
- page `404.html`

Les métadonnées doivent présenter SchoolSafe comme une solution de gestion scolaire et de sécurité portée par PRODELI S.A.R.L.U.

## Fichiers concernés

- `index.html`
- `assets/css/styles.css`
- `assets/js/main.js`
- `assets/images/schoolsafe-logo.jpg`
- `assets/images/prodeli-logo.jpg`
- `404.html`
- `robots.txt`
- `sitemap.xml`
- `README.md` si nécessaire

Le fichier `CNAME` doit rester `schoolsafe1.cc.cd`.

## Contraintes de sécurité et de périmètre

- Ne toucher à aucun dépôt de l’application SchoolSafe.
- Ne modifier aucune base de données, Supabase, RLS, migration ou backend.
- Ne déployer que le site vitrine dans `medygoo/SchoolSafe1site`.
- Ne publier aucun secret, identifiant privé ou donnée d’élève.
- Ne pas afficher de prix sur le site tant qu’il n’est pas explicitement validé pour publication.
- Ne pas inventer de fonctionnalité non documentée.

## Validation attendue

Après implémentation :
1. vérifier la syntaxe JavaScript ;
2. vérifier que les deux langues fonctionnent ;
3. vérifier les liens e-mail, téléphone et PRODELI ;
4. vérifier l’absence de débordement mobile évident ;
5. vérifier la présence du domaine dans `CNAME`, `canonical`, `robots.txt` et `sitemap.xml` ;
6. vérifier que les logos sont affichés avec un rendu non recadré ;
7. vérifier que le site reste statique et compatible GitHub Pages.
