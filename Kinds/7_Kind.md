## Event Kind 7 — Reaction

### Overview

Event Kind **7** defines **reaction** in Nostr.

- **Specification**: [NIP-25](https://github.com/nostr-protocol/nips/blob/master/25.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-25](https://github.com/nostr-protocol/nips/blob/master/25.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Specification requirement** — include user-generated-content indicating the value of the
    
3. **Specification requirement** — be interpreted as a "like" or "upvote"
    
4. **Specification requirement** — be interpreted as a "dislike" or "downvote"

---

### Examples

**Example Event**

```json
{
  "kind": 7,
  "content": ":soapbox:",
  "tags": [
    ["emoji", "soapbox", "https://gleasonator.com/emoji/Gleasonator/soapbox.png"]
  ],
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
