# roadmap-service

Cœur du produit : projets, feuille de route, progression.

| | |
|---|---|
| Port | 8082 |
| Base de données | MySQL (phpMyAdmin) – roadmap_db |
| Responsable | [Membre 1] |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Appelle** (synchrone, OpenFeign) : `legal-service` `GET /api/procedures?projectType=` et `finance-service` `GET /api/funding-options?projectType=`
- **Consomme** (asynchrone) : `ProcedureCompleted` (legal) et `FundingGranted` (finance) -> étape `DONE` + progression recalculée

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
