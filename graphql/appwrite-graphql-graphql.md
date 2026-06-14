# Appwrite GraphQL GraphQL API

The Appwrite GraphQL API exposes the full Appwrite backend-as-a-service platform through a single unified GraphQL endpoint. It mirrors the complete Appwrite REST API (excluding OAuth flows) and supports all major resource types: accounts, sessions, databases, documents, storage buckets and files, teams, memberships, cloud functions, executions, and localization data. The schema is dynamically generated from Appwrite's route definitions, so query and mutation names follow a `{namespace}{MethodName}` convention (e.g., `accountGet`, `databasesListDocuments`, `storageCreateFile`).

Authentication is provided via HTTP headers on every request: `X-Appwrite-Project` (required — your project ID), and one of `X-Appwrite-Key` (server API key), `X-Appwrite-JWT` (JWT token), or a session cookie (`a_session_{projectId}`). Introspection is disabled on production instances; the schema is built from published source and example files.

**Endpoint:** https://cloud.appwrite.io/v1/graphql

**Documentation:** https://appwrite.io/docs/apis/graphql

**References:**

- Documentation: https://appwrite.io/docs/apis/graphql
- GettingStarted: https://appwrite.io/docs/quick-starts
- GitHub: https://github.com/appwrite/appwrite
