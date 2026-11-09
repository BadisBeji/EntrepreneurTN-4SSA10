# finance-service

Facturation, comptabilité simple et gestion du capital.

| | |
|---|---|
| Port | 8084 |
| Base de données | MySQL (phpMyAdmin) – finance_db (montants DECIMAL(12,3)) |
| Responsable | Mohammed Saadallah |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Publie** (asynchrone) : `InvoiceIssued {projectId, invoiceId, issuedAt}` quand une facture passe à `SENT`
- **Appelé par** : `roadmap-service` (synchrone, bilan)

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
