# Appwrite GraphQL

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
