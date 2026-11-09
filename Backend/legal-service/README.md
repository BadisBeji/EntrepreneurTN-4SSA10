# legal-service

Catalogue des démarches légales et administratives, suivi par projet.

| | |
|---|---|
| Port | 8083 |
| Base de données | MySQL (phpMyAdmin) – legal_db |
| Responsable | Yakine Sehli |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Publie** (asynchrone) : `ProcedureCompleted {projectId, procedureId, completedAt}` quand un suivi passe à `COMPLETED`
- **Appelé par** : `roadmap-service` (synchrone)

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
