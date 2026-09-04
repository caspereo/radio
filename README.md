# Radio Danmark Pro

En simpel dansk radiospiller (PWA) med favoritter, søgning og support for både AAC- og HLS-streams.

**Live:** https://caspereo.github.io/radio/

## Hvad er det?

Single-page webapp (`index.html`) der spiller danske radiostationer direkte i browseren. Favoritter og volumen huskes i `localStorage`. På iOS/Android kan siden tilføjes til hjemmeskærmen.

## Stationer (oversigt)

| Kategori | Eksempler |
| --- | --- |
| Populære | Nova, Radio 100, Radio Soft, The Voice, PopFM, Mix 7 |
| DR Stationer | P1–P5 |
| Retro | Radio Vinyl, VinylHits, Retro Radio |
| Mix | PartyFM, Weekend Mix, The Voice Mix/Throwback, Nova 100% Dansk, Top 100, Soft Modern/Classic |

Stream-URL’er er hardcodet i `index.html`.

## Kør lokalt

Åbn filen direkte, eller brug en lokal static server:

```bash
# Python
python3 -m http.server 8080

# Node (hvis du har npx)
npx --yes serve .
```

Gå til `http://localhost:8080`.

## Deploy (GitHub Pages)

Repoet er sat op til GitHub Pages fra `main` (site root).

1. Merge til `main`
2. Vent på Pages-build
3. Appen er live på https://caspereo.github.io/radio/

## Afhængigheder

- [hls.js](https://github.com/video-dev/hls.js) (pinned via jsDelivr) til DR’s HLS-streams i browsere uden native HLS
- Google Fonts: Outfit

## Licens

MIT — se [LICENSE](LICENSE).
