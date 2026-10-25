---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het opslaan van een project in het Primavera XER-formaat."
type: docs
weight: 208
url: /nl/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Staat toe extra opties op te geven bij het opslaan van een project in het Primavera XER-formaat.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Initialiseert een nieuw exemplaar van de [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Haalt de increment op die wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Haalt het voorvoegsel op dat wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Haalt het achtervoegsel op dat wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Haalt een waarde op die aangeeft of activiteit‑ID's moeten worden hernummerd. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Haalt een waarde op die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Stelt de increment in die wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Stelt het voorvoegsel in dat wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Stelt het achtervoegsel in dat wordt gebruikt bij het hernummeren van activiteit‑ID's. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Stelt een waarde in die aangeeft of activiteit-ID's moeten worden genummerd. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Stelt een waarde in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Initialiseert een nieuw exemplaar van de [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) klasse.

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Haalt de increment op die wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Returns:**
int - de increment die wordt gebruikt bij het hernummeren van activiteit-ID's.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Haalt het voorvoegsel op dat wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Returns:**
java.lang.String - het voorvoegsel dat wordt gebruikt bij het hernummeren van activiteit-ID's.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Haalt het achtervoegsel op dat wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Returns:**
int - het achtervoegsel dat wordt gebruikt bij het hernummeren van activiteit-ID's.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Haalt een waarde op die aangeeft of activiteit‑ID's moeten worden hernummerd.

**Returns:**
boolean - een waarde die aangeeft of activiteit-ID's moeten worden genummerd.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Haalt een waarde op die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export.

Primavera-software ondersteunt geen toewijzingen van resources aan samenvattingstaken (WBS). Daarom kan het exporteren van dergelijke toewijzingen resulteren in een ongeldig bestand volgens het model van Primavera. Als true, worden toewijzingen aan samenvattingstaken overgeslagen tijdens export. Als false (de standaardwaarde), wordt er een uitzondering gegooid als een toewijzing aan een samenvattingstaak tijdens export wordt aangetroffen.

**Returns:**
boolean - een waarde die aangeeft of toewijzingen van resources aan samenvattingstaken moeten worden overgeslagen tijdens export.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Stelt de increment in die wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de increment die wordt gebruikt bij het hernummeren van activiteit-ID's. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Stelt het voorvoegsel in dat wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het voorvoegsel dat wordt gebruikt bij het hernummeren van activiteit-ID's. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Stelt het achtervoegsel in dat wordt gebruikt bij het hernummeren van activiteit‑ID's.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het achtervoegsel dat wordt gebruikt bij het hernummeren van activiteit-ID's. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Stelt een waarde in die aangeeft of activiteit-ID's moeten worden genummerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of activiteit-ID's moeten worden genummerd. |

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

