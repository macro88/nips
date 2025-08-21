## Event Kind 0 — Profile Metadata

### Overview

Event Kind **0** defines **user profile metadata** in Nostr.

- **Specification**: [NIP-01](https://github.com/nostr-protocol/nips/blob/master/01.md)
    
- **Extensions**: [NIP-05](https://github.com/nostr-protocol/nips/blob/master/05.md), [NIP-57](https://github.com/nostr-protocol/nips/blob/master/57.md)
    
- **Replaceability**: Follows [NIP-16](https://github.com/nostr-protocol/nips/blob/master/16.md). Only the most recent event per pubkey (by `created_at`) is valid.
    

Clients use Kind 0 to display profiles. Relays typically store only the latest version per pubkey.

---

### Schema Reference

|Key|Type|Max|Req|Format / Constraints|NIP Ref|Status|
|---|---|---|---|---|---|---|
|`name`|string|100|N|Display handle. Any UTF-8.|NIP-01|Standard|
|`display_name`|string|100|N|Human-readable name.|NIP-01|Standard|
|`about`|string|2000|N|Bio text.|NIP-01|Standard|
|`picture`|string|—|N|Absolute URI. Prefer `https://`.|NIP-01|Standard|
|`banner`|string|—|N|Absolute URI. Prefer `https://`.|NIP-01|Standard|
|`website`|string|—|N|Absolute URI to personal site.|NIP-01|Standard|
|`nip05`|string|320|N|`localpart@domain` (DNS-based ID).|NIP-05|Standard|
|`lud16`|string|320|N|Lightning address `name@domain`.|NIP-57|Standard|
|`lud06`|string|—|N|LNURL (bech32) or `https://` URL.|NIP-57|Standard|
|`username`|string|100|N|Optional alias; no enforced semantics.|—|Unofficial|
|`extra_*`|any|—|N|Clients may define extensions; ignore if unknown.|—|Extension|

---

### Validation Rules

1. **Replaceable** — latest `created_at` wins for each pubkey.
    
2. **One active event per pubkey** — relays should keep only the latest Kind 0 per pubkey.
    
3. **Ignore unknown keys** — clients must not fail if extra fields are present.
    
4. **UTF-8** — all string fields must be valid UTF-8.
    
5. **Absolute URIs** — enforce `https://` for security where possible.
    
6. **NIP-05 resolution** — clients may verify ownership via DNS TXT records.
    

---

### Examples

**Minimal Metadata**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000000,
  "kind": 0,
  "tags": [],
  "content": "{\"name\":\"alice\"}",
  "sig": "..."
}
```

**Full Metadata**

```json
{
  "id": "...",
  "pubkey": "abc123...",
  "created_at": 1670000100,
  "kind": 0,
  "tags": [],
  "content": "{ 
    \"name\": \"alice\",
    \"display_name\": \"Alice Wonderland\",
    \"about\": \"Decentralized dreamer.\",
    \"picture\": \"https://example.com/alice.jpg\",
    \"banner\": \"https://example.com/banner.png\",
    \"website\": \"https://alice.example\",
    \"nip05\": \"alice@example.com\",
    \"lud16\": \"alice@lightning.com\"
  }",
  "sig": "..."
}
```

---

### Security & Pitfalls

- **HTML/script injection**: sanitize `about`, `display_name`.
    
- **DNS spoofing**: `nip05` verification depends on DNS TXT records.
    
- **Phishing**: malicious `website`, `picture`, or `banner` URIs.
    
- **Image safety**: clients should proxy/resize images.
    
- **Lightning URIs**: validate format before rendering payment actions.
    

---

### Client Checklist

-  Parse `content` JSON safely.
    
-  Verify UTF-8.
    
-  Enforce "latest event wins."
    
-  Ignore unknown keys.
    
-  Validate `https://` URIs.
    
-  Verify NIP-05 (optional, for trust).
