<p align="center">
  <img src="https://sncfoundation.github.io/logos/sheedis.svg" width="96" alt="Sheedis logo">
</p>

<h1 align="center">Sheedis</h1>

<p align="center"><b>An in-spreadsheet key-value & data-structure store.</b><br>
A <a href="https://sncfoundation.github.io">Sheet-Native Computing Foundation</a> project · the spreadsheet-native <b>Redis</b></p>

---

**Status:** 📝 Unsaved Draft (design). Data & Storage TAG.

## The mapping

- key→value = a 2-column tab; **list** = a column, **set** = a dedup column, **hash** = a tab, **sorted set** = a scored+sorted column.
- **TTL/expiry** = a timestamp column + a reaper trigger; **pub/sub** = an append-only tab + pollers.

## Honest limit

Not in-memory — latency is **seconds**, not microseconds. Sheedis is Redis's *data model*, not its speed.

## Connect with real clients

Paired with [SheetWire](https://github.com/sncfoundation/sheetwire), real Redis clients can connect to a Google Sheet over the native wire protocol.

- 🗺️ [SNCF Landscape](https://sncfoundation.github.io/landscape.html) · 🧩 [Projects](https://sncfoundation.github.io/projects.html) · 🎓 [Certification](https://sncfoundation.github.io/certification.html)

---

<sub>Apache-2.0. Do not run production data on a spreadsheet. If you do, please film the query plan.</sub>
