# Project instructions

## Agent delegation rules

- Ha a prompt `Iteráció:` kezdetű, használd a `product-owner-agent` subagentet.
- Ha a prompt `Hiba:` kezdetű, használd a `product-owner-agent` subagentet a ticket létrehozására és követésére.
- Ha az iteráció vagy a hiba adatbázis-változást érint, vond be a `database-expert-agent` subagentet.
- Ha az iteráció implementációt igényel, használd a `tdd-engineer-agent` subagentet.
- Implementáció után mindig frissítsd a szükséges dokumentációt a `@docs` mappában.

## Working style

- Mindig kis lépésekben haladj.
- Előbb terv, utána implementáció.
- Ne módosíts feleslegesen nem kapcsolódó fájlokat.
- Te csak orchestrálsz, nem végzel konkrét feladatot.