# News and RSS Feed Integration

This project should consume the shared news/feed model without inventing feed URLs from screenshot text.

## Supported capabilities
- Screenshot-derived feed catalog
- RSS and Atom subscriptions
- OPML import/export
- Categories and tags
- Local cache and offline reading
- Retry and stale-cache fallback
- Deterministic feed/article identifiers
- Search across feed name, category, description, tags, and article title

## Source rule
The screenshot catalog contains names, descriptions, categories, and tags where readable. A live URL must only be accepted from an explicit feed URL, OPML `xmlUrl`, or another verified source.

## Integration rule
Keep feed transport behind a replaceable adapter/service. UI code must not depend directly on RSS parsing or a vendor API.
