# SchoolSafe public website redesign — design specification

Date: 2026-08-20
Repository: `medygoo/SchoolSafe1site`
Domain: `https://schoolsafe1.cc.cd`
Brand: **SchoolSafe by PRODELI S.A.R.L.U.**
Slogan: **Un enfant protégé, un parent informé.**

## 1. Goal

Redesign the public SchoolSafe marketing website without changing the SchoolSafe application itself. The site must look institutional, modern, trustworthy and clearly explain the product to schools, parents and partners.

The redesign keeps GitHub Pages as the hosting model and stays as a static bilingual FR/EN website.

## 2. Brand hierarchy

SchoolSafe is the primary public brand. PRODELI S.A.R.L.U. is the company carrying the project and must remain clearly visible as an endorsement rather than compete with SchoolSafe visually.

Required lockup:

- SchoolSafe
- “Un enfant protégé, un parent informé”
- “by PRODELI S.A.R.L.U.”

The official SchoolSafe logo remains the principal visual identity. The official circular PRODELI logo is displayed in the company/endorsement section using `object-fit: contain`, never cropped.

## 3. Visual direction

Primary palette:

- deep navy / midnight blue for authority and security;
- electric/royal blue for digital identity;
- gold/yellow accent inspired by the SchoolSafe logo;
- white and very light blue for clarity;
- limited use of black only where needed for the SchoolSafe logo background.

The design must avoid a generic “template” appearance. It should use generous spacing, strong typography hierarchy, subtle depth, rounded but professional cards, and restrained motion.

## 4. Navigation

Sticky responsive navigation.

Desktop links:

- Accueil / Home
- Solution
- Sécurité / Security
- Fonctionnalités / Features
- Profils / Profiles
- PRODELI
- Contact

Controls:

- FR / EN language switch;
- mobile menu with accessible expanded state;
- all internal links use section anchors.

## 5. Homepage structure

### 5.1 Hero

Purpose: explain SchoolSafe in less than five seconds.

Content:

- eyebrow: “GESTION SCOLAIRE · SÉCURITÉ · CONFIANCE”;
- headline: a concise value proposition combining school organization and child safety;
- supporting paragraph describing the connection between Direction, teachers, parents, cashier and security;
- primary CTA: “Découvrir SchoolSafe”;
- secondary CTA: “Demander une présentation”;
- visible slogan;
- official SchoolSafe logo displayed cleanly and prominently;
- signature “SchoolSafe by PRODELI S.A.R.L.U.”.

### 5.2 Three pillars

Three clear benefit blocks:

1. Sécurité de l’enfant
2. Gestion scolaire
3. Relation parent–école

Each block focuses on outcome rather than technical implementation.

### 5.3 Security / QR flow

Explain the operational flow visually in simple steps:

1. identification/scan of the student QR;
2. entry registration;
3. controlled exit;
4. verification of authorized persons;
5. useful alerts and traceability.

Do not imply that every planned capability is already deployed if it is not documented as available.

### 5.4 Features

Public feature grid based only on documented SchoolSafe capabilities:

- students and classes;
- attendance, delays and absences;
- QR student cards and entry/exit tracking;
- authorized persons;
- homework and grades;
- pedagogical follow-up;
- school payment recording, balances and receipts;
- operational reports and indicators;
- alerts and parent information;
- controlled access by user profile;
- practical computing / Digital Lab, presented as an extension “selon contrat”.

No public exposure of internal architecture, server details, secrets, RLS implementation, infrastructure IPs or internal QA information.

### 5.5 Profiles

Create professional cards for:

- Direction
- Enseignant
- Parent / Tuteur
- Caisse
- Gardien / Sécurité

Each card describes what that profile can do in clear public language. The site must not imply that one profile sees all data.

### 5.6 Parent confidence section

Explain the parent benefit:

- information concerning their own children;
- attendance and delays;
- validated homework/grades where applicable;
- receipts and useful payment information;
- alerts and school communication.

Avoid presenting SchoolSafe as directly collecting school fees. The school receives payments; SchoolSafe records and tracks them.

### 5.7 Digital Lab

Present the practical computing extension without making it appear mandatory for every deployment.

Suggested wording: “Digital Lab — extension de formation informatique pratique, selon le contrat et le projet de l’établissement.”

### 5.8 PRODELI endorsement

Dedicated section:

- “SchoolSafe by PRODELI S.A.R.L.U.”;
- official PRODELI logo, entire seal visible, no crop;
- short description of PRODELI as the Congolese company carrying the SchoolSafe project;
- optional link to `https://prodeli-sarlu.cc.cd` opening in a new tab with `rel="noopener noreferrer"`.

### 5.9 Contact / CTA

Primary public contact:

- `contact@schoolsafe1.cc.cd`
- `0828432689`
- Kinshasa, République Démocratique du Congo

CTA wording:

- “Demander une présentation”
- “Nous contacter”

No fake online form backend. If a form remains, it must either use mailto preparation or be clearly non-server based.

### 5.10 Footer

Include:

- SchoolSafe logo;
- “SchoolSafe by PRODELI S.A.R.L.U.”;
- slogan;
- contact email;
- copyright year;
- link to PRODELI site.

## 6. Bilingual behavior

French remains the default language. English is available via the existing language switch.

All new visible text must have matching FR and EN translations. Switching language must update all relevant labels without reloading the page.

Language choice may remain stored in `localStorage`.

## 7. Responsive behavior

The site must be designed mobile-first and tested for:

- small Android phones;
- modern mobile widths;
- tablets;
- desktop/laptop.

Requirements:

- no horizontal overflow;
- no cropped logos;
- readable CTA buttons;
- cards become one column on narrow screens;
- mobile navigation remains usable;
- hero artwork does not dominate the first screen excessively.

## 8. Accessibility

Required:

- semantic HTML landmarks;
- descriptive image alt text;
- keyboard-focus styles;
- sufficient color contrast;
- accessible mobile-menu state;
- reduced-motion support;
- buttons/links with clear labels;
- no essential information conveyed by color alone.

## 9. SEO and public metadata

Keep canonical domain `https://schoolsafe1.cc.cd/`.

Improve:

- page title;
- meta description;
- Open Graph title/description/image;
- theme color;
- favicon based on SchoolSafe logo;
- `robots.txt`;
- `sitemap.xml`;
- structured metadata where appropriate, without invented pricing or claims.

## 10. 404 page

Replace the minimal 404 with a branded SchoolSafe page containing:

- SchoolSafe logo;
- clear “Page introuvable” message;
- button back to home;
- same palette and typography as the main site.

## 11. Files expected to change

- `index.html`
- `assets/css/styles.css`
- `assets/js/main.js`
- `404.html`
- `robots.txt` only if required
- `sitemap.xml` only if required
- image assets only when necessary for official logo quality

`CNAME` must remain `schoolsafe1.cc.cd` and must not be changed during the redesign.

## 12. Safety / scope boundaries

This redesign MUST NOT:

- modify the SchoolSafe application repository;
- modify Supabase, database schema, RLS or backend APIs;
- publish secrets or internal infrastructure information;
- add unsupported functionality claims;
- add public pricing unless separately approved;
- alter DNS or GitHub Pages custom-domain configuration.

## 13. Acceptance criteria

The redesign is accepted when:

1. SchoolSafe is immediately identifiable as the primary brand.
2. “by PRODELI S.A.R.L.U.” is visible but subordinate to SchoolSafe.
3. Both official logos render completely without cropping.
4. The hero clearly communicates school management + child safety + parent information.
5. QR/security, features and five public profiles are clearly explained.
6. FR/EN switching works for all redesigned content.
7. Mobile navigation and layout work without horizontal overflow.
8. Contact information is correct and visible.
9. No internal/private technical information appears publicly.
10. `CNAME` remains untouched.
11. HTML/CSS/JS pass basic syntax and link checks before publication.
12. The deployed site is visually reviewed on mobile and desktop after GitHub Pages publishes the commit.
