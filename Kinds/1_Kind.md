## Event Kind 1 — Short Text Note

### Overview

Event Kind **1** defines **short text note** in Nostr.

- **Specification**: [NIP-10](https://github.com/nostr-protocol/nips/blob/master/10.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-10](https://github.com/nostr-protocol/nips/blob/master/10.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Specification requirement** — NOT be used to reply to other kinds, use [NIP-22](22
    
3. **Specification requirement** — be sorted by the reply stack from root to the direct parent
    
4. **Specification requirement** — be added as `p` tags to notify of a new reply or quote

---

### Examples

**Basic Event**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000000,
  "kind": 1,
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
