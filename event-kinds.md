# Event Kinds

This document provides a comprehensive table summary of all event kinds defined in the Nostr protocol.

| Event Kind | NIPs | Name | Summary |
| ---------- | ---- | ---- | ------- |
| `0` | [01](01.md) | User Metadata | User Metadata |
| `1` | [01](01.md) | Short Text Note | Short Text Note |
| `2` | 01 (deprecated) | Recommend Relay | Recommend Relay |
| `3` | [02](02.md) | Follows | Follows |
| `4` | [04](04.md) | Encrypted Direct Messages | Encrypted Direct Messages |
| `5` | [09](09.md) | Event Deletion Request | Event Deletion Request |
| `6` | [18](18.md) | Repost | Repost |
| `7` | [25](25.md) | Reaction | Reaction |
| `8` | [58](58.md) | Badge Award | Badge Award |
| `9` | [C7](C7.md) | Chat Message | Chat Message |
| `10` | 29 (deprecated) | Group Chat Threaded Reply | Group Chat Threaded Reply |
| `11` | [7D](7D.md) | Thread | Thread |
| `12` | 29 (deprecated) | Group Thread Reply | Group Thread Reply |
| `13` | [59](59.md) | Seal | Seal |
| `14` | [17](17.md) | Direct Message | Direct Message |
| `15` | [17](17.md) | File Message | File Message |
| `16` | [18](18.md) | Generic Repost | Generic Repost |
| `17` | [25](25.md) | Reaction to a website | Reaction to a website |
| `20` | [68](68.md) | Picture | Picture |
| `21` | [71](71.md) | Video Event | Video Event |
| `22` | [71](71.md) | Short-form Portrait Video Event | Short-form Portrait Video Event |
| `30` | [NKBIP-03] | internal reference | internal reference |
| `31` | [NKBIP-03] | external web reference | external web reference |
| `32` | [NKBIP-03] | hardcopy reference | hardcopy reference |
| `33` | [NKBIP-03] | prompt reference | prompt reference |
| `40` | [28](28.md) | Channel Creation | Channel Creation |
| `41` | [28](28.md) | Channel Metadata | Channel Metadata |
| `42` | [28](28.md) | Channel Message | Channel Message |
| `43` | [28](28.md) | Channel Hide Message | Channel Hide Message |
| `44` | [28](28.md) | Channel Mute User | Channel Mute User |
| `62` | [62](62.md) | Request to Vanish | Request to Vanish |
| `64` | [64](64.md) | Chess (PGN) | Chess (PGN) |
| `818` | [54](54.md) | Merge Requests | Merge Requests |
| `1018` | [88](88.md) | Poll Response | Poll Response |
| `1021` | [15](15.md) | Bid | Bid |
| `1022` | [15](15.md) | Bid confirmation | Bid confirmation |
| `1040` | [03](03.md) | OpenTimestamps | OpenTimestamps |
| `1059` | [59](59.md) | Gift Wrap | Gift Wrap |
| `1063` | [94](94.md) | File Metadata | File Metadata |
| `1068` | [88](88.md) | Poll | Poll |
| `1111` | [22](22.md) | Comment | Comment |
| `1222` | [A0](A0.md) | Voice Message | Voice Message |
| `1244` | [A0](A0.md) | Voice Message Comment | Voice Message Comment |
| `1311` | [53](53.md) | Live Chat Message | Live Chat Message |
| `1337` | [C0](C0.md) | Code Snippet | Code Snippet |
| `1617` | [34](34.md) | Patches | Patches |
| `1621` | [34](34.md) | Issues | Issues |
| `1622` | [34](34.md) | Git Replies (deprecated) | Git Replies (deprecated) |
| `1971` | [nostrocket][nostrocket] | Problem Tracker | Problem Tracker |
| `1984` | [56](56.md) | Reporting | Reporting |
| `1985` | [32](32.md) | Label | Label |
| `1986` |  | Relay reviews | Relay reviews |
| `1987` | [NKBIP-02] | AI Embeddings / Vector lists | AI Embeddings / Vector lists |
| `2003` | [35](35.md) | Torrent | Torrent |
| `2004` | [35](35.md) | Torrent Comment | Torrent Comment |
| `2022` | [joinstr][joinstr] | Coinjoin Pool | Coinjoin Pool |
| `4550` | [72](72.md) | Community Post Approval | Community Post Approval |
| `7000` | [90](90.md) | Job Feedback | Job Feedback |
| `7374` | [60](60.md) | Reserved Cashu Wallet Tokens | Reserved Cashu Wallet Tokens |
| `7375` | [60](60.md) | Cashu Wallet Tokens | Cashu Wallet Tokens |
| `7376` | [60](60.md) | Cashu Wallet History | Cashu Wallet History |
| `7516` | [geocaching][geocaching] | Geocache log | Geocache log |
| `7517` | [geocaching][geocaching] | Geocache proof of find | Geocache proof of find |
| `9041` | [75](75.md) | Zap Goal | Zap Goal |
| `9321` | [61](61.md) | Nutzap | Nutzap |
| `9467` | [Tidal-nostr] | Tidal login | Tidal login |
| `9734` | [57](57.md) | Zap Request | Zap Request |
| `9735` | [57](57.md) | Zap | Zap |
| `9802` | [84](84.md) | Highlights | Highlights |
| `10000` | [51](51.md) | Mute list | Mute list |
| `10001` | [51](51.md) | Pin list | Pin list |
| `10002` | [65](65.md), [51](51.md) | Relay List Metadata | Relay List Metadata |
| `10003` | [51](51.md) | Bookmark list | Bookmark list |
| `10004` | [51](51.md) | Communities list | Communities list |
| `10005` | [51](51.md) | Public chats list | Public chats list |
| `10006` | [51](51.md) | Blocked relays list | Blocked relays list |
| `10007` | [51](51.md) | Search relays list | Search relays list |
| `10009` | [51](51.md), [29](29.md) | User groups | User groups |
| `10012` | [51](51.md) | Favorite relays list | Favorite relays list |
| `10013` | [37](37.md) | Private event relay list | Private event relay list |
| `10015` | [51](51.md) | Interests list | Interests list |
| `10019` | [61](61.md) | Nutzap Mint Recommendation | Nutzap Mint Recommendation |
| `10020` | [51](51.md) | Media follows | Media follows |
| `10030` | [51](51.md) | User emoji list | User emoji list |
| `10050` | [51](51.md), [17](17.md) | Relay list to receive DMs | Relay list to receive DMs |
| `10063` | [Blossom][blossom] | User server list | User server list |
| `10096` | [96](96.md) | File storage server list | File storage server list |
| `10166` | [66](66.md) | Relay Monitor Announcement | Relay Monitor Announcement |
| `10312` | [53](53.md) | Room Presence | Room Presence |
| `10377` | [Nostr Epoxy][nostr-epoxy] | Proxy Announcement | Proxy Announcement |
| `11111` | [Nostr Epoxy][nostr-epoxy] | Transport Method Announcement | Transport Method Announcement |
| `13194` | [47](47.md) | Wallet Info | Wallet Info |
| `17375` | [60](60.md) | Cashu Wallet Event | Cashu Wallet Event |
| `21000` | [Lightning.Pub][lnpub] | Lightning Pub RPC | Lightning Pub RPC |
| `22242` | [42](42.md) | Client Authentication | Client Authentication |
| `23194` | [47](47.md) | Wallet Request | Wallet Request |
| `23195` | [47](47.md) | Wallet Response | Wallet Response |
| `24133` | [46](46.md) | Nostr Connect | Nostr Connect |
| `24242` | [Blossom][blossom] | Blobs stored on mediaservers | Blobs stored on mediaservers |
| `27235` | [98](98.md) | HTTP Auth | HTTP Auth |
| `30000` | [51](51.md) | Follow sets | Follow sets |
| `30001` | 51 (deprecated) | Generic lists | Generic lists |
| `30002` | [51](51.md) | Relay sets | Relay sets |
| `30003` | [51](51.md) | Bookmark sets | Bookmark sets |
| `30004` | [51](51.md) | Curation sets | Curation sets |
| `30005` | [51](51.md) | Video sets | Video sets |
| `30007` | [51](51.md) | Kind mute sets | Kind mute sets |
| `30008` | [58](58.md) | Profile Badges | Profile Badges |
| `30009` | [58](58.md) | Badge Definition | Badge Definition |
| `30015` | [51](51.md) | Interest sets | Interest sets |
| `30017` | [15](15.md) | Create or update a stall | Create or update a stall |
| `30018` | [15](15.md) | Create or update a product | Create or update a product |
| `30019` | [15](15.md) | Marketplace UI/UX | Marketplace UI/UX |
| `30020` | [15](15.md) | Product sold as an auction | Product sold as an auction |
| `30023` | [23](23.md) | Long-form Content | Long-form Content |
| `30024` | [23](23.md) | Draft Long-form Content | Draft Long-form Content |
| `30030` | [51](51.md) | Emoji sets | Emoji sets |
| `30040` | [NKBIP-01] | Curated Publication Index | Curated Publication Index |
| `30041` | [NKBIP-01] | Curated Publication Content | Curated Publication Content |
| `30063` | [51](51.md) | Release artifact sets | Release artifact sets |
| `30078` | [78](78.md) | Application-specific Data | Application-specific Data |
| `30166` | [66](66.md) | Relay Discovery | Relay Discovery |
| `30267` | [51](51.md) | App curation sets | App curation sets |
| `30311` | [53](53.md) | Live Event | Live Event |
| `30312` | [53](53.md) | Interactive Room | Interactive Room |
| `30313` | [53](53.md) | Conference Event | Conference Event |
| `30315` | [38](38.md) | User Statuses | User Statuses |
| `30388` | [Corny Chat][cornychat-slideset] | Slide Set | Slide Set |
| `30402` | [99](99.md) | Classified Listing | Classified Listing |
| `30403` | [99](99.md) | Draft Classified Listing | Draft Classified Listing |
| `30617` | [34](34.md) | Repository announcements | Repository announcements |
| `30618` | [34](34.md) | Repository state announcements | Repository state announcements |
| `30818` | [54](54.md) | Wiki article | Wiki article |
| `30819` | [54](54.md) | Redirects | Redirects |
| `31234` | [37](37.md) | Draft Event | Draft Event |
| `31388` | [Corny Chat][cornychat-linkset] | Link Set | Link Set |
| `31890` | [NUD: Custom Feeds][NUD: Custom Feeds] | Feed | Feed |
| `31922` | [52](52.md) | Date-Based Calendar Event | Date-Based Calendar Event |
| `31923` | [52](52.md) | Time-Based Calendar Event | Time-Based Calendar Event |
| `31924` | [52](52.md) | Calendar | Calendar |
| `31925` | [52](52.md) | Calendar Event RSVP | Calendar Event RSVP |
| `31989` | [89](89.md) | Handler recommendation | Handler recommendation |
| `31990` | [89](89.md) | Handler information | Handler information |
| `32267` |  | Software Application | Software Application |
| `34550` | [72](72.md) | Community Definition | Community Definition |
| `38172` | [87](87.md) | Cashu Mint Announcement | Cashu Mint Announcement |
| `38173` | [87](87.md) | Fedimint Announcement | Fedimint Announcement |
| `37516` | [geocaching](geocaching) | Geocache listing | Geocache listing |
| `38383` | [69](69.md) | Peer-to-peer Order events | Peer-to-peer Order events |
| `39000-9` | [29](29.md) | Group metadata events | Group metadata events |
| `39089` | [51](51.md) | Starter packs | Starter packs |
| `39092` | [51](51.md) | Media starter packs | Media starter packs |
| `39701` | [B0](B0.md) | Web bookmarks | Web bookmarks |
