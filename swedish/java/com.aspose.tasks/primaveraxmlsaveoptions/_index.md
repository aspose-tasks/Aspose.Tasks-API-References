---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projekt sparas till Primavera xml-format."
type: docs
weight: 212
url: /sv/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Tillåter att ange ytterligare alternativ när projekt sparas till Primavera xml-format.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Initierar en ny instans av klassen [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Hämtar ett värde som indikerar om en rotuppgift ska sparas eller inte. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Hämtar ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Ställer in ett värde som indikerar om en rotuppgift ska sparas eller inte. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Ställer in ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Initierar en ny instans av klassen [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Hämtar ett värde som indikerar om en rotuppgift ska sparas eller inte.

**Returns:**
boolean - ett värde som indikerar om en rotuppgift ska sparas eller inte.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Hämtar ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export.

Primavera-programvaran stödjer inte tilldelningar av resurser till sammanfattningsuppgifter (WBS). Därför kan export av sådana tilldelningar resultera i en ogiltig fil enligt Primaveras modell. Om true hoppas tilldelningar till sammanfattningsuppgifter över vid export. Om false (standardvärdet) kastas ett undantag om en tilldelning till en sammanfattningsuppgift påträffas under export.

**Returns:**
boolean - ett värde som indikerar om tilldelningar av resurser till sammanfattningsuppgifter ska hoppas över vid export.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Ställer in ett värde som indikerar om en rotuppgift ska sparas eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om en rotuppgift ska sparas eller inte. |

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

