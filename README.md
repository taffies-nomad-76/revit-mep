# Revit MEP Workflow Optimalisatie

Deze repository is bedoeld voor het structureren, verbeteren en bewaken van Revit MEP-workflows.

De nadruk ligt niet alleen op modelleren, maar vooral op **planning, structuur, overzicht en herhaalbare werkprocessen**. De repo moet helpen om complexe Revit-taken kleiner, duidelijker en beter controleerbaar te maken.

## Doel

Een praktische hulptool bouwen voor Revit MEP-werk waarbij overzicht centraal staat:

- duidelijke planning
- korte checklists
- prioriteiten per fase
- visuele roadmaps
- vaste werkvolgorde
- minder losse notities
- minder contextverlies
- beter zicht op wat open, bezig of klaar is

## Overzichtsgericht uitgangspunt

Deze repo wordt opgebouwd voor werk dat snel complex, versnipperd of onoverzichtelijk kan worden.

Dat betekent:

- taken klein en afvinkbaar maken
- geen lange ongestructureerde lijsten
- prioriteiten zichtbaar houden
- één centrale checklist gebruiken
- voortgang visueel maken
- open punten expliciet benoemen
- beslissingen en revisies vastleggen
- werk opdelen in korte fases
- groepen inklapbaar maken waar dat overzicht geeft

Het doel is niet om méér administratie te maken, maar om minder mentale belasting te hebben tijdens Revit MEP-werk.

## Huidige inhoud

| Bestand / issue | Doel |
|---|---|
| [`ROADMAP.md`](./ROADMAP.md) | Hoofdfases en visuele route |
| [`docs/BOUWDELEN.md`](./docs/BOUWDELEN.md) | Voorlopige bouwdelen- en verdiepingenstructuur |
| [`docs/JOB_CHECKLIST_STRUCTUUR.md`](./docs/JOB_CHECKLIST_STRUCTUUR.md) | Job-checklist per hoofdstuk, bouwdeel en vloer |
| [`docs/ILS_AB_MATRIX.md`](./docs/ILS_AB_MATRIX.md) | AB-gerichte ILS-propertymatrix voor Revit MEP |
| [`docs/WORKFLOW_PRINCIPLES.md`](./docs/WORKFLOW_PRINCIPLES.md) | Werkprincipes en vaste workflow |
| [GitHub issue #4](https://github.com/taffies-nomad-76/revit-mep/issues/4) | Centrale interactieve master-checklist |

## Werkmethode

De basisvolgorde voor Revit MEP-werk:

1. Scope bepalen
2. Bouwdelen en verdiepingen afbakenen
3. Job-checklist per hoofdstuk/bouwdeel/vloer opbouwen
4. ILS AB-matrix controleren
5. Modelleren volgens opdracht
6. Controleren
7. Syncen
8. Annoteren
9. Revisies verwerken
10. Plotten via DiRoots
11. PDF controleren
12. Output vrijgeven

## ILS-focus

De ILS-uitwerking in deze repository is **AB-gericht**. De huidige matrix bevat:

- 51 — Warmte-opwekking
- 55 — Koude-opwekking
- 56 — Warmtedistributie
- 57 — Luchtbehandeling

De matrix bevat per categorie de eigenschap, Revit-drager, soort/type, AB-status en praktische opmerkingen.

## Bouwdelenfocus

De bouwdelenstructuur is voorlopig en wordt later aangevuld. De huidige structuur bevat:

- A: Aa, Ab, Ac, Ad
- B: Ba, Bb, Bc, Bd
- C: Ca, Cb, Cc, Cd
- D: Da, Db
- Kelder

Verdiepingen verschillen per bouwdeel. Onbekende verdiepingsaantallen blijven open punt.

## Job-checkliststructuur

De jobstructuur is opgezet met twee hoofdhoofdstukken:

- Luchtbehandeling
- Warmte en koude distributie

Daaronder volgt per hoofdstuk:

1. bouwdeel
2. vloer
3. later toe te voegen jobs

De hoofdstukken blijven inklapbaar en krijgen een globale checkbox voor “alles klaar”.

## Ontwerpprincipes voor deze repo

Bij uitbreiding van deze repository gelden de volgende principes:

- kort boven volledig
- visueel waar mogelijk
- één bron van waarheid per onderwerp
- checkboxes voor uitvoerbaar werk
- Mermaid voor flowcharts en roadmaps
- issues voor taken
- markdown-bestanden voor vaste werkwijzen
- open vragen apart benoemen
- geen aannames verwerken alsof ze besluiten zijn

## Huidige focus

Eerste focus:

- bouwdelenstructuur
- job-checkliststructuur
- Revit Basis ILS
- AB-gerichte propertycontrole
- Revisie AB
- workflowstructuur
- planning en overzicht
