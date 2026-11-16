# marketing-service

Veille concurrentielle et campagnes marketing.

| | |
|---|---|
| Port | 8085 |
| Base de données | MySQL (phpMyAdmin) – marketing_db (budget DECIMAL(12,3)) |
| Responsable | Ilyes Anene |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Publie** (asynchrone) : `CampaignLaunched {projectId, campaignId, launchedAt}` quand une campagne passe à `ACTIVE`
- Aucun appel synchrone vers un autre service

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
