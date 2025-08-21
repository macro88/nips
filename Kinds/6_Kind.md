## Event Kind 6 — Repost

### Overview

Event Kind **6** defines **repost** in Nostr.

- **Specification**: [NIP-18](https://github.com/nostr-protocol/nips/blob/master/18.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-18](https://github.com/nostr-protocol/nips/blob/master/18.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Specification requirement** — include an `e` tag with the `id` of the note that is
    
3. **Specification requirement** — include a relay URL as its third entry
    
4. **Specification requirement** — include the [NIP-21](21

---

### Examples

**Basic Event**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000000,
  "kind": 6,
  "tags": [],
  "content": "...",
  "sig": "..."
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
