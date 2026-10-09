# Leasingoverblik.dk – data om privatleasing i Danmark

Åbne data fra [Leasingoverblik.dk](https://leasingoverblik.dk/), et uafhængigt prisindeks for privatleasing i Danmark. Tallene bygger på de privatleasingpriser, bilimportørerne selv offentliggør, målt hver morgen siden 19. juli 2026.

*Open data on private car leasing prices in Denmark (Danish column names). Daily measurements of importer-published offers since 19 July 2026. Licence: CC BY 4.0.*

## Filer

| Fil | Indhold |
| --- | --- |
| `data/leasingindeks.csv` | Leasingindekset dag for dag (100 = 19. juli 2026). Kædet prisindeks på præcis de samme aftaler. |
| `data/standardkurv.csv` | Billigste aftale pr. model ved 15.000 km om året – grundlaget for markedets nøgletal. |
| `data/alle-aftaler.csv` | Alle aktuelle aftaler med ydelse, førstegangsydelse, kendte gebyrer, totalpris, gennemsnitlig månedspris, nypris og karakter. |
| `data/prisaendringer.csv` | Målte prisændringer på samme aftale med uændrede vilkår (to faktiske målinger). |
| `data/elbilafgift-2027.csv` | Elbil-varianter med beregnet registreringsafgift 2026 og 2027. |
| `arkiv/<år-måned>/` | Udtræk fra månedens sidste måling. Mappen for indeværende måned er foreløbig. |

Alle CSV-filer er UTF-8 med semikolon som skilletegn og komma som decimaltegn (dansk Excel).

## Vigtige begreber

- **Gennemsnitlig månedspris** (`gns_maanedspris_kr`): ydelser, førstegangsydelse og kendte gebyrer fordelt over aftalens måneder.
- **Annonceret ydelse** (`annonceret_ydelse_kr`): den månedlige ydelse, udbyderen viser.
- **Karakter A–E**: årlig leasingpris i procent af vejledende nypris, bygget på FDM's 15 %-tommelfingerregel.
- **Leasingindekset**: geometrisk gennemsnit af prisændringer på samme aftale pr. model, derefter gennemsnit over modellerne, kædet dag for dag.

Hele metoden og forbeholdene: https://leasingoverblik.dk/metode.html

## Dækning og forbehold

Data dækker de mærker, Leasingoverblik måler (se https://leasingoverblik.dk/datadaekning.html) – ikke alle tilbud i Danmark. Enkelte mærker aflæses manuelt én gang om ugen. Priser kan være ændret, siden de blev målt. Tidligere måneder kan blive rettet, hvis en fejlmåling trækkes tilbage; rettelser står i metodens ændringslog.

## Licens og kildeangivelse

Creative Commons Navngivelse 4.0 International (CC BY 4.0). Du må dele og bearbejde data, også kommercielt, når du angiver kilden:

> Kilde: Leasingoverblik.dk · [målingens dato] · CC BY 4.0

gerne med link til https://leasingoverblik.dk/.

## Opdatering

De nyeste tal ligger altid på https://leasingoverblik.dk/data/ og opdateres hver morgen. Dette arkiv opdateres ved månedsskifte.
