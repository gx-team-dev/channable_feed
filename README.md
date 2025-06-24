# Gallerix Channable Feeds

Detta repo innehåller produktfeeds för Channable-integrationer för olika marknader.

## 📁 Struktur

```
germany/          # Tyskland market feeds
sweden/           # Sverige market feeds (framtida)
norway/           # Norge market feeds (framtida)
poland/           # Polen market feeds (framtida)
```

## 🇩🇪 Tyskland (Core Pro Test)

**Aktuell feed:** `germany/channable_germany_exact_copy_20250624_0948.csv`
- **Produkter:** 250 items (exakt kopia från GMC Tyskland)
- **Format:** Channable CSV-standard
- **Uppdaterad:** 2025-06-24
- **Status:** Test-feed för Core Pro setup

### Raw URL för Channable:
```
https://raw.githubusercontent.com/gx-team-dev/channable_feed/main/germany/channable_germany_exact_copy_20250624_0948.csv
```

## 📊 Feed-specifikationer

### Obligatoriska kolumner:
- `id`, `title`, `description`, `link`, `image_link`
- `price`, `availability`, `condition`, `brand`
- `google_product_category`, `target_country`

### Gallerix-specifika:
- `custom_label_0` (produktkategori)
- `mpn` (produktnummer)
- `color` (där tillgängligt)
- `sale_price` (kampanjpris)

## 🔄 Uppdateringsprocess

1. Generera ny CSV från GMC
2. Testa lokalt
3. Commit och push till detta repo
4. Uppdatera URL i Channable
5. Verifiera import

## 🎯 Framtida optimeringar

Se `Fas_2_produktoptimering_channable.md` i huvudprojektet för detaljerad plan.