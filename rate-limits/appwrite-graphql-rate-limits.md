# Appwrite GraphQL Rate Limits

Appwrite applies rate limits to protect the platform from abuse and to ensure fair usage across all projects and organizations. Rate limits apply to all API endpoints including the GraphQL endpoint at `/v1/graphql`.

## General Rate Limits

Appwrite enforces rate limiting on a per-project basis. Specific numeric thresholds are not publicly documented in detail, but the following general principles apply:

- Rate limits are applied per project, not per organization
- Limits vary by plan tier (Free, Pro, Enterprise)
- Exceeding rate limits returns a `429 Too Many Requests` HTTP response

## Resource Limits by Plan

The following resource quotas act as effective rate ceilings:

| Resource | Free | Pro |
|---|---|---|
| Monthly Active Users | 75,000 | 200,000 |
| Function Executions/month | 750,000 | 3,500,000 |
| Bandwidth/month | 5 GB | 2 TB |
| Storage | 2 GB | 150 GB |
| Projects | 2 (shared) | Unlimited (dedicated) |

## GraphQL-Specific Notes

- The GraphQL endpoint (`/v1/graphql`) is subject to the same rate limits as REST endpoints
- Query batching (sending multiple operations in one request) counts as a single request from a rate-limit perspective but each operation is evaluated individually for resource consumption
- File uploads via `multipart/form-data` are subject to storage quotas

## Self-Hosted Deployments

For self-hosted Appwrite instances, rate limits can be configured by the administrator. The default configuration may differ from the Appwrite Cloud settings.

**Source:** https://appwrite.io/docs/apis/graphql
