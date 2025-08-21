## Event Kind 818 — Merge Requests

### Overview

Event Kind **818** defines **merge requests** in Nostr.

- **Specification**: [NIP-54](https://github.com/nostr-protocol/nips/blob/master/54.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-54](https://github.com/nostr-protocol/nips/blob/master/54.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Follow NIP specifications** — adhere to the referenced NIP requirements.
    
3. **UTF-8** — all string fields must be valid UTF-8.

---

### Examples

**Basic Event**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000000,
  "kind": 818,
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
