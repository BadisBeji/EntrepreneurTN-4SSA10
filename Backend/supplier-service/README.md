# supplier-service

Fournisseurs et commandes d'achat (B2B).

| | |
|---|---|
| Port | 8086 |
| Base de données | MySQL (phpMyAdmin) – supplier_db (montants DECIMAL(12,3)) |
| Responsable | Khaled Khalil |
| Contrat d'API | [`openapi.yaml`](openapi.yaml) (à ouvrir dans https://editor.swagger.io) |

## Interactions
- **Publie** (asynchrone) : `OrderConfirmed {projectId, orderId, totalAmount, confirmedAt}` quand une commande passe à `CONFIRMED`
- Aucun appel synchrone vers un autre service

## État
Conception validée (validation 1). Le code Spring Boot sera ajouté dans ce dossier (`pom.xml`, `src/`).
