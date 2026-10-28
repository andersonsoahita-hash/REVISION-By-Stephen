# REVISION By Stephen

Dépôt de l'application **Carnet de révision MSc1** (INSEEC, Marketing, Communication et Stratégie de Marque).

## Contenu
- `index.html` : l'app qui fonctionne directement sur GitHub Pages (création de cours, import de PDF / Word / texte, leçons modifiables, création de questions, tests /20, examen blanc, correction ; tout est enregistré dans le navigateur).
- `app/carnet-de-revision.html` : version Claude (base partagée, génération de questions, correction des questions ouvertes par Claude).
- `courses/<cours>/questions.json` : banque de questions de chaque cours.
- `courses/<cours>/lessons.json` : leçons structurées (notions, exemples, points à retenir).
- `courses/<cours>/cards.json` : cartes mémoire.
- `CHANGELOG.md` : historique des mises à jour.

## Important
La version GitHub ne génère pas de questions toute seule : les nouvelles questions sont ajoutées dans `courses/<cours>/questions.json`. La progression reste dans le navigateur utilisé (téléphone et ordinateur ne partagent pas la leur).
Les supports de cours des professeurs (slides, transcriptions) ne sont pas dans ce dépôt public.

## Ajouter un nouveau cours
1. Un **fichier de cours (.json, format `carnet-pack-1`)** contient les leçons (une page par section), les questions et les cartes. Exemple : `modeles/exemple-pack-shopper.json`.
2. Sur l'accueil de l'app : « Importer un cours » puis choisir le fichier. Le cours est créé d'un coup.
3. Re-importer un fichier du même cours (même `id`) le met à jour : nouvelles leçons, questions et cartes ajoutées, progression conservée.
4. Le fichier est produit par Claude, ou par n'importe quelle IA avec la consigne du bouton « Copier la consigne ».
5. Les cours du dépôt (dossier `courses/`) se mettent à jour avec le bouton « Mettre à jour » : la version est dans `courses/index.json`.
