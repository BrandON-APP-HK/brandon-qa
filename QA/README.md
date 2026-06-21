# Brandon Mobile Manual QA Scenarios

These files contain manual QA flows for the implemented app behavior. Each scenario uses tester commands plus assertions for observable app state.

## Recommended execution order

1. Authentication and guest access: files `01` to `08`.
2. Feed, deals, search, map, brand, and check-in: files `09` to `18`.
3. User-owned flows: files `19` to `27`.
4. Static pages and resilience: files `28` to `29`.

## Common test data

- A logged-out clean app session.
- A verified email/password user.
- An unverified email/password user.
- Google login test account.
- iOS Apple ID for Apple login testing.
- Brands with and without active promotions.
- Campaigns with products, stores, opening hours, check-in range, and promotion rules.
- Deals that are liked, unliked, flagged, unflagged, and searchable.
- Rewards that are available, unavailable due to points, sold out, and requiring full address.

## Notes

- Apple login is iOS-only.
- Permission tests depend on OS state; reset permissions before each permission scenario.
- Backend-dependent states may require seeded accounts or API fixtures.
- QR/scanner check-in is intentionally excluded because no implementation was found in the current source code.
