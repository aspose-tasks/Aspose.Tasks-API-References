---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projekt sparas till Primavera XER-format."
type: docs
weight: 208
url: /sv/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Tillåter att ange ytterligare alternativ när projekt sparas till Primavera XER-format.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Initialiserar en ny instans av klassen [PrimaveraSaveOptions](../../com.aspose/tasks/primaverasaveoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Hämtar ökningen som används vid omnumrering av aktivitets‑ID:n. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Hämtar prefixet som används vid omnumrering av aktivitets‑ID:n. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Hämtar suffixet som används vid omnumrering av aktivitets‑ID:n. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Hämtar ett värde som indikerar om aktivitets‑ID:n behöver omnummeras. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Hämtar ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Ställer in ökningen som används vid omnumrering av aktivitets‑ID:n. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Ställer in prefixet som används vid omnumrering av aktivitets‑ID:n. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Ställer in suffixet som används vid omnumrering av aktivitets‑ID:n. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Ställer in ett värde som indikerar om aktivitets‑ID:n behöver omnummeras. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Ställer in ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Initialiserar en ny instans av klassen [PrimaveraSaveOptions](../../com.aspose/tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Hämtar ökningen som används vid omnumrering av aktivitets‑ID:n.

**Returns:**
int - ökningen som används vid omnumrering av aktivitets‑ID:n.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Hämtar prefixet som används vid omnumrering av aktivitets‑ID:n.

**Returns:**
java.lang.String - prefixet som används vid omnumrering av aktivitets‑ID:n.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Hämtar suffixet som används vid omnumrering av aktivitets‑ID:n.

**Returns:**
int - suffixet som används vid omnumrering av aktivitets‑ID:n.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Hämtar ett värde som indikerar om aktivitets‑ID:n behöver omnummeras.

**Returns:**
boolean - ett värde som indikerar om aktivitets‑ID:n behöver omnummeras.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Hämtar ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export.

Primavera-programvaran stödjer inte tilldelningar av resurser till sammanfattningsuppgifter (WBS). Därför kan export av sådana tilldelningar resultera i en ogiltig fil enligt Primaveras modell. Om true hoppas tilldelningar till sammanfattningsuppgifter över vid export. Om false (standardvärdet) kastas ett undantag om en tilldelning till en sammanfattningsuppgift påträffas under export.

**Returns:**
boolean - ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Ställer in ökningen som används vid omnumrering av aktivitets‑ID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ökningen som används vid omnumrering av aktivitets‑ID:n. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Ställer in prefixet som används vid omnumrering av aktivitets‑ID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | prefixet som används vid omnumrering av aktivitets‑ID:n. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Ställer in suffixet som används vid omnumrering av aktivitets‑ID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | suffixet som används vid omnumrering av aktivitets‑ID:n. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Ställer in ett värde som indikerar om aktivitets‑ID:n behöver omnummeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om aktivitets‑ID:n behöver omnummeras. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Ställer in ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export.

Primavera-programvaran stödjer inte tilldelningar av resurser till sammanfattningsuppgifter (WBS). Därför kan export av sådana tilldelningar resultera i en ogiltig fil enligt Primaveras modell. Om true hoppas tilldelningar till sammanfattningsuppgifter över vid export. Om false (standardvärdet) kastas ett undantag om en tilldelning till en sammanfattningsuppgift påträffas under export.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export. |

