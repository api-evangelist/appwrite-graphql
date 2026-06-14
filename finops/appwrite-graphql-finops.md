# Appwrite GraphQL FinOps

This document provides cost optimization guidance for teams using the Appwrite GraphQL API.

## Cost Structure

Appwrite charges are based on resource consumption at the organization level, with resources allocated per project. The GraphQL API itself does not carry a separate cost — usage is metered through the underlying resources it accesses (database reads/writes, function executions, storage, bandwidth).

## GraphQL-Driven Cost Factors

### Bandwidth
- Every GraphQL query/mutation response consumes bandwidth
- **Free:** 5 GB/month per project
- **Pro:** 2 TB/month per project; $15 per additional 100 GB
- **Optimization:** Use GraphQL selection sets to request only needed fields, reducing payload size and bandwidth consumption

### Database Operations
- Pro plan overage: $0.06 per 100,000 reads; $0.10 per 100,000 writes
- **Optimization:** Batch multiple queries into a single GraphQL request using query batching to reduce round-trip overhead; use filters and limits to avoid full-table scans

### Function Executions
- **Free:** 750,000/month; **Pro:** 3,500,000/month
- **Optimization:** Avoid triggering unnecessary function-backed resolvers; cache responses at the client layer where possible

### Storage
- **Free:** 2 GB; **Pro:** 150 GB ($2.80 per additional 100 GB)
- File uploads via GraphQL multipart consume storage quota

## Cost Control Features

- **Budget caps and alerts** are available on the Pro plan to prevent unexpected overages
- Resource allocation is per project, so isolating high-traffic projects on Pro prevents shared resource exhaustion
- Self-hosting Appwrite eliminates SaaS costs at the expense of infrastructure management

## Recommendations

1. Start on the Free plan for development and low-traffic projects
2. Use GraphQL selection sets aggressively to minimize data transfer
3. Enable budget caps on Pro to avoid surprise overage bills
4. Monitor monthly active users — this is often the first limit hit on the Free tier
5. Consider self-hosting for predictable, high-volume workloads where infrastructure costs are lower than SaaS overages

**Source:** https://appwrite.io/pricing
