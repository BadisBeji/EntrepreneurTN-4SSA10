# api-gateway

Spring Cloud Gateway (port **8080**) : point d'entrée unique des clients. Route `/api/auth/**`, `/api/users/**` vers auth-service, `/api/projects/**` et `/api/steps/**` vers roadmap-service,
`/api/procedures/**` et `/api/trackings/**` vers legal-service, `/api/transactions/**`, `/api/funding-*/**` vers finance-service. Vérifie le JWT et transmet l'identité de l'utilisateur.

État : conception validée ; code à ajouter.
