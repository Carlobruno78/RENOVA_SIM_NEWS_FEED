# RENOVA Simulator News Hub — Public Feed

Public, read-only feed consumed by **RENOVA Simulator News Hub**.

## Purpose

This repository is the public distribution layer for user-facing news that has been approved for publication.  
The private monitoring/audit repository remains separate and is **not** exposed to the Android application.

## Structure

- `feed/meta.json` — feed version and synchronization metadata
- `feed/index.json` — compact global index
- `feed/iracing.json` — iRacing news feed
- `feed/lmu.json` — Le Mans Ultimate news feed
- `schema/news-feed.schema.json` — JSON schema for published feed entries

## Security boundary

This repository must contain **no secrets**, webhook URLs, API keys, internal audit logs, private diagnostics, or protected/premium content.

The Android app reads this repository as a public source. Paid or restricted content must use a protected backend/API in a later phase.

## Publishing cadence

- Source audit: daily at 09:00 Europe/Rome
- Publication: Tuesday and Friday
- The feed is updated from the same approved publication payload used by the user-facing news pipeline.

