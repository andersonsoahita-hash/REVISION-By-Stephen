# REVISION By Stephen

Dépôt de l'application **Carnet de révision MSc1** (INSEEC, Marketing, Communication et Stratégie de Marque).

## Contenu
- `index.html` : l'app qui fonctionne directement sur GitHub Pages (création de cours, import de PDF / Word / texte, leçons modifiables, création de questions, tests /20, examen blanc, correction ; tout est enregistré dans le navigateur).
- `app/carnet-de-revision.html` : version Claude (base partagée, génération de questions, correction des questions ouvertes par Claude).
- `courses/<cours>/questions.json` : banque de questions de chaque cours.
- `CHANGELOG.md` : historique des mises à jour.

## Important
La version GitHub ne génère pas de questions toute seule : les nouvelles questions sont ajoutées dans `courses/<cours>/questions.json`. La progression reste dans le navigateur utilisé (téléphone et ordinateur ne partagent pas la leur).
Les supports de cours des professeurs (slides, transcriptions) ne sont pas dans ce dépôt public.
