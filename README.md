# Skellefteåbanan i Trainz

Ett hobbyprojekt som undersöker hur AI-assisterad geodatabearbetning kan göra det enklare att återskapa Skellefteåbanan i Trainz.

Målet är att få en reproducerbar kedja från höjddata, kartor och spårgeometri till ett visuellt granskat resultat i Trainz. Vi börjar med små experiment och återanvänder tidigare försök där det går.

## Börja här

1. Läs [projektbeskrivningen](docs/PROJECT.md).
2. Läs [instruktionerna till Codex](AGENTS.md).
3. Börja med [experiment 001: inventering](experiments/001-inventory/README.md) på den lokala datorn.
4. Dokumentera resultatet i experimentet och uppdatera [experimentloggen](docs/EXPERIMENTS.md).

## Struktur

| Sökväg | Innehåll |
| --- | --- |
| `docs/` | Mål, beslut, datakällor och experimentöversikt |
| `experiments/` | Ett avgränsat försök per katalog, med metod och resultat |
| `scripts/` | Verktyg för inventering, konvertering och kontroller |
| `source-data/` | Lokala kopior av underlag; själva datan versionshanteras inte |
| `generated/` | Lokala bearbetade filer och exporter; versionshanteras inte |

## Arbetsflöde

Diskutera nästa steg i ChatGPT-projektet, dokumentera uppdraget här, låt Codex bearbeta underlaget och granska resultatet i de lokala verktygen. För tillbaka observationerna till experimentloggen innan nästa försök.

Codex i en molnmiljö har inte automatiskt åtkomst till speldatorns filer eller installerade program. Lokal inventering kräver lokal körning, eller att relevant underlag lämnas över.

## Status

Projektstruktur skapad 2026-10-07. Ingen inventering eller geodatabearbetning har utförts ännu. Teststräcka, tidsperiod och programversioner återstår att fastställa.

Ingen projektlicens har valts. Villkor för externa data och assets dokumenteras separat i [datakällsregistret](docs/DATA_SOURCES.md).
