# SchoolSafe — Refonte complète du site vitrine

Date : 20 août 2026
Dépôt : `medygoo/SchoolSafe1site`
Domaine cible : `https://schoolsafe1.cc.cd`

## 1. Objectif

Transformer le site vitrine SchoolSafe actuel en une vitrine institutionnelle professionnelle, moderne, claire et crédible, sans toucher à l’application SchoolSafe elle-même.

Le site doit présenter SchoolSafe comme une solution scolaire complète centrée sur la sécurité de l’enfant, la gestion scolaire et la relation parent-école, avec la signature permanente :

**SchoolSafe by PRODELI S.A.R.L.U.**

Slogan :

**Un enfant protégé, un parent informé.**

## 2. Principes de conception

- SchoolSafe reste la marque principale.
- PRODELI S.A.R.L.U. apparaît comme société porteuse et de confiance.
- Palette principale : bleu profond, bleu électrique, or, blanc.
- Design moderne, institutionnel et accessible, sans surcharge graphique.
- Mobile-first avec rendu propre sur téléphone, tablette et ordinateur.
- FR par défaut avec bascule EN complète.
- Pas de fausse fonctionnalité interactive ni de promesse non documentée.
- Aucun prix public dans cette version.
- Aucune information technique interne, serveur, base de données, IP ou secret ne doit apparaître.

## 3. Structure de navigation

Navigation principale :

- Accueil
- Solution
- Sécurité
- Fonctionnalités
- Profils
- Digital Lab
- À propos / PRODELI
- Contact
- FR / EN

Sur mobile : menu hamburger clair, accessible, sans chevauchement.

## 4. Hero / première impression

Le premier écran doit communiquer immédiatement :

**SchoolSafe**

**Un enfant protégé, un parent informé.**

**SchoolSafe by PRODELI S.A.R.L.U.**

Titre principal proposé :

> La plateforme scolaire intelligente qui relie sécurité, gestion et parents.

Sous-texte :

> SchoolSafe aide l’école à mieux suivre les élèves, sécuriser les entrées et sorties, organiser les opérations scolaires et maintenir les parents informés avec des données validées.

Actions :

- `Découvrir SchoolSafe`
- `Demander une présentation`

Le logo SchoolSafe doit être très visible, net, sans recadrage.

## 5. Trois piliers principaux

Une section claire présente les trois axes différenciateurs :

### Sécurité de l’enfant
- QR élève
- contrôle entrée/sortie
- personnes autorisées
- historique de passage
- alertes et incidents

### Gestion scolaire
- élèves et classes
- présences
- devoirs et notes
- bulletins et documents
- finances et reçus enregistrés par l’école
- rapports et indicateurs

### Relation parent-école
- informations validées sur ses propres enfants
- alertes
- devoirs
- notes
- reçus
- suivi de présence

## 6. Section Sécurité QR

Présenter visuellement un parcours simple :

1. L’élève présente son QR.
2. Le gardien ou profil autorisé effectue le scan.
3. SchoolSafe vérifie le contexte et l’autorisation.
4. L’entrée ou la sortie est enregistrée.
5. L’école conserve l’historique utile à la traçabilité.

Inclure également les personnes autorisées et la préparation des sorties, sans exposer l’architecture technique de sécurité.

## 7. Fonctionnalités

Créer une grille professionnelle avec les grandes fonctions publiques :

- Gestion des élèves et classes
- Présences, retards et absences
- Entrées / sorties QR
- Personnes autorisées
- Devoirs et notes
- Direction pédagogique
- Caisse et reçus
- Contrôle des frais
- Rapports et indicateurs
- Notifications in-app
- Documents scolaires
- CodeCure

Les descriptions doivent rester courtes et orientées bénéfice.

## 8. Profils utilisateurs

Présenter au minimum :

### Direction
Supervision, tableaux de bord, rapports, élèves, classes, alertes, finances selon les droits.

### Enseignant
Présences, devoirs, notes, suivi pédagogique, préparation et cahier de texte.

### Parent / Tuteur
Accès aux informations validées concernant ses propres enfants uniquement.

### Caisse
Enregistrement des paiements reçus par l’école, reçus, soldes et opérations autorisées.

### Gardien / Sécurité
Scans, contrôle des entrées-sorties, personnes autorisées, incidents et journal de sécurité.

Le site ne doit jamais laisser entendre qu’un profil voit toutes les données.

## 9. Gouvernance et sécurité des accès

Une petite section institutionnelle peut expliquer sans détails techniques :

- accès selon le rôle et les autorisations ;
- séparation des responsabilités ;
- traçabilité des opérations sensibles ;
- accès parent limité aux enfants concernés ;
- contrôle des données sensibles côté système, pas uniquement dans l’interface.

Ne pas exposer les règles RLS, noms de tables ou architecture interne.

## 10. Digital Lab

Section distincte :

**Digital Lab — informatique pratique**

Présenter le principe d’équipement informatique et d’apprentissage pratique selon les partenariats et contrats applicables.

Éviter de présenter un nombre de machines comme une garantie universelle si cela dépend du contrat.

## 11. Section PRODELI

Afficher clairement le logo officiel PRODELI fourni par l’utilisateur, sans recadrage.

Texte :

> SchoolSafe est un projet porté par PRODELI S.A.R.L.U., société congolaise engagée dans l’innovation, l’organisation et la transformation numérique.

Signature visuelle :

**SchoolSafe by PRODELI S.A.R.L.U.**

Un lien vers `https://prodeli-sarlu.cc.cd` peut être ajouté dans un nouvel onglet avec `rel="noopener noreferrer"`.

## 12. Contact

Présenter :

- `contact@schoolsafe1.cc.cd`
- `0828432689`
- Kinshasa, République Démocratique du Congo

CTA principal :

**Demander une présentation de SchoolSafe**

Le formulaire, s’il est conservé, ne doit pas prétendre stocker ou envoyer réellement des données côté serveur si aucun backend de formulaire n’existe. Une approche `mailto:` claire est acceptable.

## 13. Footer

Inclure :

- logo SchoolSafe
- `SchoolSafe by PRODELI S.A.R.L.U.`
- slogan
- contact
- lien PRODELI
- copyright dynamique
- lien vers politique de confidentialité / mentions si une page dédiée est ajoutée

## 14. Bilingue FR / EN

Toutes les chaînes visibles doivent être traduites, pas seulement la navigation.

Exigences :

- FR par défaut ;
- mémoriser la langue dans `localStorage` ;
- texte alternatif et labels accessibles cohérents ;
- traduction complète des CTA, sections, profils, Digital Lab, contact et footer.

## 15. Responsive et accessibilité

- aucune coupure du logo SchoolSafe ou PRODELI ;
- navigation utilisable à 320 px de largeur ;
- boutons tactiles d’au moins 44 px de hauteur ;
- contraste suffisant ;
- `:focus-visible` sur liens et boutons ;
- menu mobile avec `aria-expanded` ;
- `prefers-reduced-motion` respecté ;
- images avec `alt` pertinents ;
- pas de débordement horizontal.

## 16. SEO et partage

Mettre à jour :

- `<title>`
- meta description
- canonical
- Open Graph
- Twitter cards
- favicon
- `robots.txt`
- `sitemap.xml`
- données structurées `SoftwareApplication` / `Organization` si pertinentes

URL canonique : `https://schoolsafe1.cc.cd/`

## 17. Performance

- aucun framework lourd nécessaire ;
- HTML/CSS/JS statiques adaptés à GitHub Pages ;
- images optimisées ;
- pas de dépendance externe critique ;
- JS léger et défensif ;
- pas d’erreur si `localStorage` est indisponible ;
- pas de layout shift majeur.

## 18. Fichiers concernés

Principalement :

- `index.html`
- `assets/css/styles.css`
- `assets/js/main.js`
- `assets/images/schoolsafe-logo.jpg`
- `assets/images/prodeli-logo.jpg`
- `404.html`
- `robots.txt`
- `sitemap.xml`
- `README.md`

Le fichier `CNAME` doit rester `schoolsafe1.cc.cd`.

## 19. Critères de validation

La refonte est considérée terminée lorsque :

1. le site affiche clairement `SchoolSafe by PRODELI S.A.R.L.U.` ;
2. le slogan officiel est visible ;
3. les deux logos sont nets, entiers et non recadrés ;
4. toutes les sections clés sont présentes ;
5. FR et EN couvrent tout le contenu visible ;
6. le site est propre à 320 px, tablette et desktop ;
7. aucun lien interne important n’est cassé ;
8. le lien PRODELI ouvre le site PRODELI dans un nouvel onglet ;
9. le SEO pointe uniquement vers `schoolsafe1.cc.cd` ;
10. `CNAME` reste inchangé ;
11. aucun secret ni détail technique interne n’est exposé ;
12. le site reste un pur site vitrine et ne modifie pas l’application SchoolSafe.

## 20. Hors périmètre

Cette refonte ne doit pas :

- modifier le dépôt de l’application SchoolSafe ;
- modifier Supabase ;
- modifier les migrations ;
- ajouter un système de paiement ;
- implémenter une authentification ;
- publier des prix non validés ;
- inventer des fonctionnalités non documentées ;
- modifier les DNS ou le domaine sans instruction séparée.
