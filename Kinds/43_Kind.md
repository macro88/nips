## Event Kind 43 — Channel Hide Message

### Overview

Event Kind **43** defines **channel hide message** in Nostr.

- **Specification**: [NIP-28](https://github.com/nostr-protocol/nips/blob/master/28.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-28](https://github.com/nostr-protocol/nips/blob/master/28.md)|*TBD*|

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
  "kind": 43,
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
