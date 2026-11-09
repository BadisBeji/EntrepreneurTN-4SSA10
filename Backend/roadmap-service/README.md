# roadmap-service

Cœur du produit : projets, feuille de route, progression.

| | |
|---|---|
| Port | 8082 |
| Base de données | MySQL (phpMyAdmin) – roadmap_db |
| Responsable | Badis Beji |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Appelle** (synchrone, OpenFeign) : `legal-service` `GET /api/procedures?projectType=` (démarches) et `finance-service` `GET /api/projects/{id}/summary` (bilan du tableau de bord)
- **Consomme** (asynchrone) : `ProcedureCompleted` (legal) et `InvoiceIssued` (finance) -> étape `DONE` + progression recalculée

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
