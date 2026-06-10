# Installatie-codestructuur per bouwdeel

Deze pagina legt de werkpakket-/code-opbouw vast per bouwdeel, verdieping en installatiegroep.

## Naamgevingspatroon

```text
{Bouwdeel}-VL-{Verdieping}-{Installatiecode}
```

Voorbeelden:

```text
Aa-VL-00-5556
Aa-VL-01-5556
Aa-VL-00-5700
Aa-VL-01-5700
```

## Installatiegroepen

| Code | Omschrijving | Gebruik |
|---:|---|---|
| 5556 | CV-installaties | Werkpakketten / controle per bouwdeel en verdieping |
| 5700 | Luchtinstallaties | Werkpakketten / controle per bouwdeel en verdieping |

## Bouwdelen waarop dit geldt

| Hoofdgroep | Bouwdelen |
|---|---|
| A | Aa, Ab, Ac, Ad |
| B | Ba, Bb, Bc, Bd |
| C | Ca, Cb, Cc, Cd |
| D | Da, Db |
| Kelder | Kelder |

## Bekende verdiepingsreeksen

| Bouwdeel | Verdiepingen | Reeks |
|---|---:|---|
| Aa | 5 | `00` t/m `04` |
| Ab | onbekend | `XX` placeholder |
| Ac | 7 | `00` t/m `06` |
| Ad | 7 | `00` t/m `06` |
| Ba | onbekend | `XX` placeholder |
| Bb | onbekend | `XX` placeholder |
| Bc | onbekend | `XX` placeholder |
| Bd | onbekend | `XX` placeholder |
| Ca | 7 | `00` t/m `06` |
| Cb | 4 | `00` t/m `03` |
| Cc | onbekend | `XX` placeholder |
| Cd | onbekend | `XX` placeholder |
| Da | onbekend | `XX` placeholder |
| Db | onbekend | `XX` placeholder |
| Kelder | onbekend | `XX` placeholder tot keldercodering vaststaat |

---

# 5556 — CV-installaties

<details open>
<summary><strong>A</strong></summary>

## Aa

```text
Aa-VL-00-5556
Aa-VL-01-5556
Aa-VL-02-5556
Aa-VL-03-5556
Aa-VL-04-5556
```

## Ab

```text
Ab-VL-XX-5556
```

## Ac

```text
Ac-VL-00-5556
Ac-VL-01-5556
Ac-VL-02-5556
Ac-VL-03-5556
Ac-VL-04-5556
Ac-VL-05-5556
Ac-VL-06-5556
```

## Ad

```text
Ad-VL-00-5556
Ad-VL-01-5556
Ad-VL-02-5556
Ad-VL-03-5556
Ad-VL-04-5556
Ad-VL-05-5556
Ad-VL-06-5556
```

</details>

<details>
<summary><strong>B</strong></summary>

## Ba

```text
Ba-VL-XX-5556
```

## Bb

```text
Bb-VL-XX-5556
```

## Bc

```text
Bc-VL-XX-5556
```

## Bd

```text
Bd-VL-XX-5556
```

</details>

<details>
<summary><strong>C</strong></summary>

## Ca

```text
Ca-VL-00-5556
Ca-VL-01-5556
Ca-VL-02-5556
Ca-VL-03-5556
Ca-VL-04-5556
Ca-VL-05-5556
Ca-VL-06-5556
```

## Cb

```text
Cb-VL-00-5556
Cb-VL-01-5556
Cb-VL-02-5556
Cb-VL-03-5556
```

## Cc

```text
Cc-VL-XX-5556
```

## Cd

```text
Cd-VL-XX-5556
```

</details>

<details>
<summary><strong>D</strong></summary>

## Da

```text
Da-VL-XX-5556
```

## Db

```text
Db-VL-XX-5556
```

</details>

<details>
<summary><strong>Kelder</strong></summary>

```text
Kelder-VL-XX-5556
```

</details>

---

# 5700 — Luchtinstallaties

<details open>
<summary><strong>A</strong></summary>

## Aa

```text
Aa-VL-00-5700
Aa-VL-01-5700
Aa-VL-02-5700
Aa-VL-03-5700
Aa-VL-04-5700
```

## Ab

```text
Ab-VL-XX-5700
```

## Ac

```text
Ac-VL-00-5700
Ac-VL-01-5700
Ac-VL-02-5700
Ac-VL-03-5700
Ac-VL-04-5700
Ac-VL-05-5700
Ac-VL-06-5700
```

## Ad

```text
Ad-VL-00-5700
Ad-VL-01-5700
Ad-VL-02-5700
Ad-VL-03-5700
Ad-VL-04-5700
Ad-VL-05-5700
Ad-VL-06-5700
```

</details>

<details>
<summary><strong>B</strong></summary>

## Ba

```text
Ba-VL-XX-5700
```

## Bb

```text
Bb-VL-XX-5700
```

## Bc

```text
Bc-VL-XX-5700
```

## Bd

```text
Bd-VL-XX-5700
```

</details>

<details>
<summary><strong>C</strong></summary>

## Ca

```text
Ca-VL-00-5700
Ca-VL-01-5700
Ca-VL-02-5700
Ca-VL-03-5700
Ca-VL-04-5700
Ca-VL-05-5700
Ca-VL-06-5700
```

## Cb

```text
Cb-VL-00-5700
Cb-VL-01-5700
Cb-VL-02-5700
Cb-VL-03-5700
```

## Cc

```text
Cc-VL-XX-5700
```

## Cd

```text
Cd-VL-XX-5700
```

</details>

<details>
<summary><strong>D</strong></summary>

## Da

```text
Da-VL-XX-5700
```

## Db

```text
Db-VL-XX-5700
```

</details>

<details>
<summary><strong>Kelder</strong></summary>

```text
Kelder-VL-XX-5700
```

</details>

---

## Open punten

- Verdiepingen voor Ab.
- Verdiepingen voor Ba, Bb, Bc en Bd.
- Verdiepingen voor Cc en Cd.
- Verdiepingen voor Da en Db.
- Definitieve keldercodering: `Kelder-VL-XX-*` is voorlopig.
- Bevestigen of `D` zelf ook als zelfstandig werkpakket nodig is naast `Da` en `Db`.
- Bevestigen of verdieping `00` altijd begane grond betekent.
