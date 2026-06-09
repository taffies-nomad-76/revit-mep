# ILS AB-matrix — Revit MEP

Deze matrix is de vaste bron voor de AB-gerichte ILS-controle binnen deze repo.

## Uitgangspunt

De workflow is **AB-gericht**. TO/UO is niet de primaire insteek voor deze repo. De matrix is bedoeld om Revit MEP-modellen, families, types en output controleerbaar te maken voor AB.

## Kolommen

| Kolom | Betekenis |
|---|---|
| ILS eigenschap | Naam van de gevraagde eigenschap |
| Revit-drager | Revit-parameter of drager waarin de waarde hoort |
| Soort/type | Overgenomen code uit de ILS-input: `g`, `e` of `p` |
| AB | Wel/niet verplicht voor AB volgens de aangeleverde informatie |
| Waarde / unit / opmerking | Praktische invulinstructie of beperking |

---

## 51 — Warmte-opwekking

| ILS eigenschap | Revit-drager | Soort/type | AB | Waarde / unit / opmerking |
|---|---|---:|:---:|---|
| Omschrijving | `Description` | g | yes | Korte en bondige omschrijving. Voorbeelden: rookgasafvoer, ketel, warmtepomp, warmtewisselaar. |
| Verkorte code | `Type Mark` | e | yes | Gestandaardiseerde code. Wordt gebruikt om componentcode te genereren. |
| Systeem classificatie | `System Classification` | e | yes | Type systeem, bijvoorbeeld Supply Air, Return Air. |
| Systeem naam | `System Name` | e | yes | Naam van het systeem, bijvoorbeeld `lu-t 01`, `lu-t 02`. |
| Systeem afkorting | `System Abbreviation` | e | yes | Afkorting van de systeemnaam voor tags. |
| Vermogen | `vermogen` | e | yes | Unit: W. Alleen voor energiebehoevende componenten. |
| Type omschrijving | `Type Comments` | p | yes | Typeomschrijving. |
| Isolatiedikte | `Insulation Thickness` | p | yes | Unit: mm. Van toepassing op isolatie wanneer gemodelleerd. |

## 55 — Koude-opwekking

| ILS eigenschap | Revit-drager | Soort/type | AB | Waarde / unit / opmerking |
|---|---|---:|:---:|---|
| Omschrijving | `Description` | g | yes | Korte en bondige omschrijving. Voorbeelden: koelmachine, dry-cooler, split unit binnen. |
| Tracing | exacte Revit-drager nog te bepalen | e | no | Waarde: Y/N. Exacte Revit carrier/description nog invullen. |
| Verkorte code | `Type Mark` | e | yes | Gestandaardiseerde code. Wordt gebruikt om componentcode te genereren. |
| Systeem classificatie | `System Classification` | e | yes | Systeemclassificatie invullen. |
| Systeem naam | `System Name` | e | yes | Systeemnaam invullen. |
| Systeem afkorting | `System Abbreviation` | e | yes | Afkorting voor tags. |
| Type omschrijving | `Type Comments` | p | yes | Typeomschrijving. |
| Isolatiedikte | `Insulation Thickness` | p | yes | Unit: mm. Van toepassing op isolatie wanneer gemodelleerd en/of in het veld aanwezig. Materiaal ook meenemen. |

## 56 — Warmtedistributie

| ILS eigenschap | Revit-drager | Soort/type | AB | Waarde / unit / opmerking |
|---|---|---:|:---:|---|
| Omschrijving | `Description` | g | yes | Korte en bondige omschrijving. Voorbeelden: radiator, convector, expansieautomaat, fan coil unit. |
| Tracing | exacte Revit-drager nog te bepalen | e | yes | Waarde: Y/N. Exacte Revit carrier/description nog invullen. |
| Verkorte code | `Type Mark` | e | yes | Gestandaardiseerde code. Wordt gebruikt om componentcode te genereren. |
| Systeem classificatie | `System Classification` | e | yes | Systeemclassificatie invullen. |
| Systeem naam | `System Name` | e | yes | Systeemnaam invullen. |
| Systeem afkorting | `System Abbreviation` | e | yes | Afkorting voor tags. |
| Type omschrijving | `Type Comments` | p | yes | Typeomschrijving. |
| Isolatiedikte | `Insulation Thickness` | p | yes | Unit: mm. Van toepassing op isolatie wanneer gemodelleerd. |

## 57 — Luchtbehandeling

| ILS eigenschap | Revit-drager | Soort/type | AB | Waarde / unit / opmerking |
|---|---|---:|:---:|---|
| Omschrijving | `Description` | g | yes | Korte en bondige omschrijving. Voorbeelden: toevoerrooster vloer, luchtslang, luchtkanaal rond, ventilatoren. |
| Verkorte code | `Type Mark` | e | yes | Gestandaardiseerde code. Wordt gebruikt om componentcode te genereren. |
| Systeem classificatie | `System Classification` | e | yes | Systeemclassificatie invullen. |
| Systeem naam | `System Name` | e | yes | Systeemnaam invullen. |
| Systeem afkorting | `System Abbreviation` | e | yes | Afkorting voor tags. |
| Type omschrijving | `Type Comments` | p | yes | Typeomschrijving. |
| Isolatiedikte | `Insulation Thickness` | p | yes | Unit: mm. Van toepassing op isolatie wanneer gemodelleerd en/of in het veld aanwezig. Materiaal ook meenemen. |

---

## Controleprincipes

- Controleer eerst de algemene AB-verplichte velden.
- Controleer daarna categorie-specifieke uitzonderingen, zoals `Tracing` en `Vermogen`.
- Leg onbekende Revit-dragers expliciet vast als open punt.
- Verwerk geen aannames alsof ze definitieve projectafspraken zijn.
- Gebruik deze matrix als input voor de master checklist in GitHub issue `#4`.

## Open punten

| Punt | Status |
|---|---|
| Exacte Revit-drager voor `Tracing` bij koude-opwekking | open |
| Exacte Revit-drager voor `Tracing` bij warmtedistributie | open |
| Betekenis/definitie van soort/type-codes `g`, `e`, `p` | open |
| Definitieve projectspecifieke systeemnaamconventie | open |
| Definitieve projectspecifieke verkorte-codeconventie | open |
