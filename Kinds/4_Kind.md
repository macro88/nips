## Event Kind 4 — Encrypted Direct Messages

### Overview

Event Kind **4** defines **encrypted direct messages** in Nostr.

- **Specification**: [NIP-04](https://github.com/nostr-protocol/nips/blob/master/04.md)
    


---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|*To be documented*|*TBD*|*TBD*|*TBD*|*TBD*|[NIP-04](https://github.com/nostr-protocol/nips/blob/master/04.md)|*TBD*|

---

### Validation Rules

1. **Regular** — regular event rules apply.
    
2. **Specification requirement** — contain an entry identifying the receiver of the message (such that relays may naturally forward this event to them), in the form `["p", "<pubkey, as a hex string>"]`
    
3. **Specification requirement** — be passed as the `hashfp` argument in `secp256k1_ecdh`
    
4. **Specification requirement** — not* search and replace public key or note references from the `

---

### Examples

**Basic Event**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000000,
  "kind": 4,
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
