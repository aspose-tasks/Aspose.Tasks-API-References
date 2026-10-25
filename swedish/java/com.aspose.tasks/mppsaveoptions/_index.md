---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektdata sparas till MPP."
type: docs
weight: 149
url: /sv/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Tillåter att ange ytterligare alternativ när projektdata sparas till MPP.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Initierar en ny instans av klassen [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getClearVba()](#getClearVba--) | Hämtar ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas i MPP-format. |
| [getProtectionPassword()](#getProtectionPassword--) | Hämtar ett lösenord som används för att skydda den resulterande MPP-filen. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Hämtar ett värde som indikerar om ogiltiga resursallokeringar ska tas bort vid sparning till MPP. |
| [getWriteFilters()](#getWriteFilters--) | Hämtar ett värde som indikerar om filterdata ska skrivas när ett projekt sparas i MPP-format. |
| [getWriteGroups()](#getWriteGroups--) | Hämtar ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas i MPP-format. |
| [getWriteVba()](#getWriteVba--) | Hämtar ett värde som indikerar om befintlig VBA-makrodatan ska uppdateras i MPP-filen. |
| [getWriteViewData()](#getWriteViewData--) | Hämtar ett värde som indikerar om vydata ska skrivas när ett projekt sparas i MPP-format. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Ställer in ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas i MPP-format. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Ställer in ett lösenord som används för att skydda den resulterande MPP-filen. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Ställer in ett värde som indikerar om ogiltiga resursallokeringar ska tas bort vid sparning till MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Ställer in ett värde som indikerar om filterdata ska skrivas när ett projekt sparas i MPP-format. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Ställer in ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas i MPP-format. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Ställer in ett värde som indikerar om befintlig VBA-makrodatan ska uppdateras i MPP-filen. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Ställer in ett värde som indikerar om vydata ska skrivas när ett projekt sparas i MPP-format. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initierar en ny instans av klassen [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Hämtar ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas i MPP-format.

**Returns:**
boolean - ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas i MPP-format.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Hämtar ett lösenord som används för att skydda den resulterande MPP-filen. Stöds för närvarande för MS Project 2010 och nyare format.

--------------------

Nullvärde indikerar att projektfilen inte är skyddad.

**Returns:**
java.lang.String - ett lösenord som används för att skydda den resulterande MPP-filen.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Hämtar ett värde som indikerar om ogiltiga resursallokeringar ska tas bort vid sparning till MPP.

--------------------

MS Project skapar en tom resursallokering för varje uppgift. Ställ in denna flagga till true för att ta bort dem vid sparning.

**Returns:**
boolean - ett värde som indikerar om ogiltiga resursallokeringar ska tas bort vid sparning till MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Hämtar ett värde som indikerar om filterdata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Filterdata inkluderar samlingarna Project.TaskFilters och Project.ResourceFilters.

--------------------

Stöds för närvarande för MSP 2010 eller nyare format.

**Returns:**
boolean - ett värde som indikerar om filterdata ska skrivas när ett projekt sparas till MPP-format.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Hämtar ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Gruppdata inkluderar samlingarna Project.TaskGroups och Project.ResourceGroups.

**Returns:**
boolean - ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas till MPP-format.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Hämtar ett värde som indikerar om befintliga VBA-makrodatan i MPP-filen ska uppdateras. För närvarande stöds skrivning av VbaModule.SourceCode.

**Returns:**
boolean - ett värde som indikerar om befintliga VBA-makrodatan i MPP-filen ska uppdateras.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Hämtar ett värde som indikerar om vydata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Visningsdata inkluderar samlingarna Project.Views, Filters och Tables.

**Returns:**
boolean - ett värde som indikerar om visningsdata ska skrivas när ett projekt sparas till MPP-format.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Ställer in ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om befintliga VBA-makrodatan ska tas bort när ett projekt sparas till MPP-format. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Anger ett lösenord som används för att skydda den resulterande MPP-filen. Stöds för närvarande för MS Project 2010 och nyare format.

--------------------

Nullvärde indikerar att projektfilen inte är skyddad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett lösenord som används för att skydda den resulterande MPP-filen. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Ställer in ett värde som indikerar om ogiltiga resursallokeringar ska tas bort vid sparning till MPP.

--------------------

MS Project skapar en tom resursallokering för varje uppgift. Ställ in denna flagga till true för att ta bort dem vid sparning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om ogiltiga resursallokeringar ska tas bort när man sparar till MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Ställer in ett värde som indikerar om filterdata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Filterdata inkluderar samlingarna Project.TaskFilters och Project.ResourceFilters.

--------------------

Stöds för närvarande för MSP 2010 eller nyare format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om filterdata ska skrivas när ett projekt sparas till MPP-format. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Ställer in ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Gruppdata inkluderar samlingarna Project.TaskGroups och Project.ResourceGroups.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om gruppdata ska skrivas när ett projekt sparas till MPP-format. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Anger ett värde som indikerar om befintliga VBA-makrodatan i MPP-filen ska uppdateras. För närvarande stöds skrivning av VbaModule.SourceCode.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om befintliga VBA-makrodatan i MPP-filen ska uppdateras. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Ställer in ett värde som indikerar om vydata ska skrivas när ett projekt sparas i MPP-format.

--------------------

Visningsdata inkluderar samlingarna Project.Views, Filters och Tables.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om visningsdata ska skrivas när ett projekt sparas till MPP-format. |

