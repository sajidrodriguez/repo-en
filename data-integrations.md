# Data and integrations

[← Back to the overview](./README.md)

## What I solve

I connect external services without giving them complete authority over data
or operations. I design layers that validate, normalize and make information
usable across the business.

Mobilec project status refers to my employment there, which has ended;
it does not imply that I currently maintain those systems.

## Selected implementations

### Secure integration layer and middleware · production

Secure, isolated middleware between the conversational experience and critical
integrations. It centralizes validation and allows the rest of the system to
evolve without directly exposing operational services.
The layer includes JWT/OAuth 2.0 authentication, Zod validation, webhook
verification, and permission and error handling.

### Shared operational data source · production

A dedicated data layer consolidating information from different providers.
It reduces coupling, preserves a consistent representation and supports gradual
service replacement while maintaining a coherent data model.
I implemented it with Supabase and PostgreSQL.

## Decisions and trade-offs

- Protect critical integrations outside the conversational channel.
- Unify external information before using it in operations.
- Expose only the minimum capabilities required between components.
- Support gradual independence from providers without requiring a complete
  migration before delivering value.

## Public boundary

This document explains professional decisions. It omits table names, endpoints,
credentials, internal rules, network configurations and any information that
could be used to reconstruct the production topology.
