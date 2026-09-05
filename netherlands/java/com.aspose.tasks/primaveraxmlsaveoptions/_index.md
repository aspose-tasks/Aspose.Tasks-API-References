---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het opslaan van een project in het Primavera xml-formaat."
type: docs
weight: 212
url: /nl/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Staat toe extra opties op te geven bij het opslaan van een project in het Primavera xml-formaat.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Initialiseert een nieuw exemplaar van de [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Haalt een waarde op die aangeeft of een hoofdtaak moet worden opgeslagen of niet. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Haalt een waarde op die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Stelt een waarde in die aangeeft of een hoofdtaak moet worden opgeslagen of niet. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Stelt een waarde in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Initialiseert een nieuw exemplaar van de [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) klasse.

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Haalt een waarde op die aangeeft of een hoofdtaak moet worden opgeslagen of niet.

**Returns:**
boolean - een waarde die aangeeft of een hoofdtaak moet worden opgeslagen of niet.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Haalt een waarde op die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export.

Primavera-software ondersteunt geen toewijzingen van resources aan samenvattingstaken (WBS). Daarom kan het exporteren van dergelijke toewijzingen resulteren in een ongeldig bestand volgens het model van Primavera. Als true, worden toewijzingen aan samenvattingstaken overgeslagen tijdens export. Als false (de standaardwaarde), wordt er een uitzondering gegooid als een toewijzing aan een samenvattingstaak tijdens export wordt aangetroffen.

**Returns:**
boolean - een waarde die aangeeft of toewijzingen van resources aan samenvattingstaken moeten worden overgeslagen tijdens export.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Stelt een waarde in die aangeeft of een hoofdtaak moet worden opgeslagen of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een hoofdtaak moet worden opgeslagen of niet. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Stelt een waarde in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export.

Primavera-software ondersteunt geen toewijzingen van resources aan samenvattingstaken (WBS). Daarom kan het exporteren van dergelijke toewijzingen resulteren in een ongeldig bestand volgens het model van Primavera. Als true, worden toewijzingen aan samenvattingstaken overgeslagen tijdens export. Als false (de standaardwaarde), wordt er een uitzondering gegooid als een toewijzing aan een samenvattingstaak tijdens export wordt aangetroffen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of toewijzingen van resources aan samenvattingstaken moeten worden overgeslagen tijdens export. |

