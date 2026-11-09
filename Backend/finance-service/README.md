# finance-service

Comptabilité simple, aides et financements.

| | |
|---|---|
| Port | 8084 |
| Base de données | MySQL (phpMyAdmin) – finance_db (montants DECIMAL(12,3)) |
| Responsable | Mohammed Saadallah |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Publie** (asynchrone) : `FundingGranted {projectId, applicationId, amount}` quand une demande passe à `ACCEPTED`
- **Appelé par** : `roadmap-service` (synchrone)

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
