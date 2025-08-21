## Event Kind 5 — Event Deletion Request

### Overview

Event Kind **5** defines **event deletion request** in Nostr.

- **Specification**: [NIP-09](https://github.com/nostr-protocol/nips/blob/master/09.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-09](https://github.com/nostr-protocol/nips/blob/master/09.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Specification requirement** — validate that each event `pubkey` referenced in the `e` tag of the deletion request is identical to the deletion request `pubkey`, before hiding or deleting any event
    
3. **Specification requirement** — include a `k` tag for the kind of each event being requested for deletion
    
4. **Specification requirement** — delete or stop publishing any referenced events that have an identical `pubkey` as the deletion request

---

### Examples

**Example Event**

```json
{
  "kind": 5,
  "pubkey": <32-bytes hex-encoded public key of the event creator>,
  "tags": [
    ["e", "dcd59..464a2"],
    ["e", "968c5..ad7a4"],
    ["a", "<kind>:<pubkey>:<d-identifier>"],
    ["k", "1"],
    ["k", "30023"]
  ],
  "content": "these posts were published by accident",
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
