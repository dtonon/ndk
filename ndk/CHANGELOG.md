# @nostr-dev-kit/ndk

## 1.3.1

### Patch Changes

-   Fix issue when publishing to an explicit relay set where one of the relays is offline

## 1.3.0

### Minor Changes

-   cf4a648: Support fetching events from NIP-33 `a` tags
-   3946078: User npub/hexpubkey become optional. This means that if you refer to aser by their
    hexpubkey, npub won't be computed until it's necessary.

    This is a breaking change since hexpubkey goes from being called as function (`hexpubkey()`) to a getter (`hexpubkey`).

-   3440768: User profile dedicated cache

### Patch Changes

-   88df10a: Throw when a user is instantiated without both an npub and pubkey
-   c225094: Fetching a relay list from a user will now also inspect kind:3 if the user doesn't have a NIP-65 set
