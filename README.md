# hvisk

Krypteret chat i én statisk side (Chrome, Edge, Safari, Firefox; Mac, Windows, telefon).

- Nøglen står kun i linkets #-del og sendes aldrig til en server.
- HKDF -> AES-GCM-256 + kanal-id. Relæet ser kun kanal-id og støj.
- Hver enhed signerer med egen ECDSA P-256-nøgle.
- Beskeder gemmes krypteret i IndexedDB; brænd-beskeder gemmes aldrig.
