## Event Kind 3 — Follows

### Overview

Event Kind **3** defines **follows** in Nostr.

- **Specification**: [NIP-02](https://github.com/nostr-protocol/nips/blob/master/02.md)
    
- **Replaceability**: Follows [NIP-16](https://github.com/nostr-protocol/nips/blob/master/16.md). Only the most recent event per pubkey (by `created_at`) is valid.

---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-02](https://github.com/nostr-protocol/nips/blob/master/02.md)|*TBD*|

---

### Validation Rules

1. **Replaceable** — replaceable event rules apply.
    
2. **Specification requirement** — contain all entries
    
3. **Specification requirement** — delete past following lists as soon as they receive a new one
    
4. **Specification requirement** — publish a follow list with good relays for each of their follows so other clients may use these to update their internal relay lists if needed, increasing censorship-resistance

---

### Examples

**Example Event**

```json
{
  "kind": 3,
  "tags": [
    ["p", "91cf9..4e5ca", "wss://alicerelay.com/", "alice"],
    ["p", "14aeb..8dad4", "wss://bobrelay.com/nostr", "bob"],
    ["p", "612ae..e610f", "ws://carolrelay.com/ws", "carol"]
  ],
  "content": "",
  // other fields...
}
```

---

### Security & Pitfalls

- **Input validation**: validate all user-provided content.
    
- **Spam prevention**: implement appropriate rate limiting.
    
- **Privacy considerations**: be aware of metadata leakage.

---

### Client Checklist

-  Parse event content safely.
    
-  Verify UTF-8 encoding.
    
-  Follow replaceability rules.
    
-  Validate against NIP specifications.
    
-  Implement proper error handling.
