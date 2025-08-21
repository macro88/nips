## Event Kind 11 — Thread

### Overview

Event Kind **11** defines **thread** in Nostr.

- **Specification**: [NIP-7D](https://github.com/nostr-protocol/nips/blob/master/7D.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-7D](https://github.com/nostr-protocol/nips/blob/master/7D.md)|*TBD*|

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
  "kind": 11,
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
