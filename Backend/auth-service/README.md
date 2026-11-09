# auth-service

Commun : développé par toute l'équipe.

| | |
|---|---|
| Port | 8081 |
| Base de données | MySQL (phpMyAdmin) – auth_db |
| Responsable | Toute l'équipe (service commun) |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Appelé par** : l'API Gateway pour l'inscription, la connexion et la lecture des profils ; le JWT émis ici est vérifié à la gateway.
## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
