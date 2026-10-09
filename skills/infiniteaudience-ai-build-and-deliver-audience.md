---
name: build-and-deliver-audience
description: Size a population, save it as a segment, compose an audience, quote and deliver it with Infinite Audience.
api: infiniteaudience-ai:infinite-audience-api
generated: '2026-10-09'
method: generated
operations: [discoveryCount, quoteDelivery, createSegment, createAudience, getCatalogFields]
---
1. Browse filter fields with the attribute catalog before building filters.
2. Size the unsaved population with a discovery count.
3. Save the filters as a segment, then compose an audience from saved segments.
4. Request a delivery quote (counts are records, not prices), then create the delivery.
5. Wait for the delivery webhook (verify X-IA-Signature) or poll the delivery.
Writes accept Idempotency-Key only on match operations; do not blindly retry delivery creation.
