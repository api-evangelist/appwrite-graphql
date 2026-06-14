# Appwrite GraphQL

Appwrite GraphQL is a powerful API layer that exposes the full Appwrite backend-as-a-service platform through a GraphQL interface, allowing developers to query and mutate any resource type including databases, storage, users, and functions. It mirrors the complete Appwrite REST API (except OAuth) with GraphQL advantages such as selection sets and query batching, enabling precise data fetching and multiple operations in a single request.

## Links

- **Website:** https://appwrite.io
- **GraphQL Documentation:** https://appwrite.io/docs/apis/graphql
- **API Reference:** https://appwrite.io/docs/references
- **Pricing:** https://appwrite.io/pricing
- **GitHub Organization:** https://github.com/appwrite
- **LinkedIn:** https://www.linkedin.com/company/appwrite

## GraphQL Endpoint

- **Cloud:** `https://cloud.appwrite.io/v1/graphql`
- **Self-hosted:** `https://{YOUR_DOMAIN}/v1/graphql`

## About

Appwrite is an open-source backend-as-a-service platform that provides Auth, Databases, Storage, Functions, Messaging, Hosting, Realtime, and more. The GraphQL API exposes all of these capabilities through a single `/v1/graphql` endpoint.

Key features of the GraphQL API:
- Full coverage of the REST API surface (except OAuth)
- Selection sets for targeted field retrieval to reduce bandwidth
- Query batching for multiple operations in a single HTTP request
- File uploads via multipart/form-data
- Authentication via Appwrite sessions and API keys
