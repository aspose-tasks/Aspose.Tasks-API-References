---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het opslaan van projectgegevens naar MPP."
type: docs
weight: 149
url: /nl/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Staat toe extra opties op te geven bij het opslaan van projectgegevens naar MPP.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Initialiseert een nieuw exemplaar van de [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getClearVba()](#getClearVba--) | Haalt een waarde op die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project in MPP‑formaat. |
| [getProtectionPassword()](#getProtectionPassword--) | Haalt een wachtwoord op dat wordt gebruikt om het resulterende MPP‑bestand te beveiligen. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Haalt een waarde op die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP. |
| [getWriteFilters()](#getWriteFilters--) | Haalt een waarde op die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat. |
| [getWriteGroups()](#getWriteGroups--) | Haalt een waarde op die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat. |
| [getWriteVba()](#getWriteVba--) | Haalt een waarde op die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt. |
| [getWriteViewData()](#getWriteViewData--) | Haalt een waarde op die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-indeling. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Stelt een waarde in die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project naar MPP-indeling. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Stelt een wachtwoord in dat wordt gebruikt om het resulterende MPP-bestand te beveiligen. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Stelt een waarde in die aangeeft of ongeldige resource-toewijzingen moeten worden verwijderd bij het opslaan naar MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Stelt een waarde in die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Stelt een waarde in die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Stelt een waarde in die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Stelt een waarde in die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-indeling. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initialiseert een nieuw exemplaar van de [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) klasse.

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Haalt een waarde op die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project in MPP‑formaat.

**Returns:**
boolean - een waarde die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project naar MPP-indeling.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Haalt een wachtwoord op dat wordt gebruikt om het resulterende MPP-bestand te beveiligen. Momenteel wordt dit ondersteund voor MS Project 2010 en nieuwere formaten.

--------------------

Een null-waarde geeft aan dat het projectbestand niet beveiligd is.

**Returns:**
java.lang.String - een wachtwoord dat wordt gebruikt om het resulterende MPP-bestand te beveiligen.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Haalt een waarde op die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP.

--------------------

MS Project maakt voor elke taak een lege resource-toewijzing aan. Stel deze vlag in op true om ze bij het opslaan te verwijderen.

**Returns:**
boolean - een waarde die aangeeft of ongeldige resource-toewijzingen moeten worden verwijderd bij het opslaan naar MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Haalt een waarde op die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.

--------------------

Filtergegevens omvatten de collecties Project.TaskFilters en Project.ResourceFilters.

--------------------

Momenteel ondersteund voor MSP 2010 of nieuwere formaten.

**Returns:**
boolean - een waarde die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Haalt een waarde op die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.

--------------------

Groepsgegevens omvatten de collecties Project.TaskGroups en Project.ResourceGroups.

**Returns:**
boolean - een waarde die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Haalt een waarde op die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt. Momenteel wordt het schrijven van VbaModule.SourceCode ondersteund.

**Returns:**
boolean - een waarde die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Haalt een waarde op die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-indeling.

--------------------

Weergavegegevens omvatten de collecties Project.Views, Filters en Tables.

**Returns:**
boolean - een waarde die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-indeling.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Stelt een waarde in die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project naar MPP-indeling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project in MPP-indeling. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Stelt een wachtwoord in dat wordt gebruikt om een resulterend MPP-bestand te beveiligen. Momenteel wordt dit ondersteund voor MS Project 2010 en nieuwere indelingen.

--------------------

Een null-waarde geeft aan dat het projectbestand niet beveiligd is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een wachtwoord dat wordt gebruikt om een resulterend MPP-bestand te beveiligen. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Stelt een waarde in die aangeeft of ongeldige resource-toewijzingen moeten worden verwijderd bij het opslaan naar MPP.

--------------------

MS Project maakt voor elke taak een lege resource-toewijzing aan. Stel deze vlag in op true om ze bij het opslaan te verwijderen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of ongeldige resource-toewijzingen moeten worden verwijderd bij het opslaan naar MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Stelt een waarde in die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.

--------------------

Filtergegevens omvatten de collecties Project.TaskFilters en Project.ResourceFilters.

--------------------

Momenteel ondersteund voor MSP 2010 of nieuwere formaten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project in MPP-indeling. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Stelt een waarde in die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP voor het formaat.

--------------------

Groepsgegevens omvatten de collecties Project.TaskGroups en Project.ResourceGroups.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project in MPP-indeling. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Stelt een waarde in die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt. Momenteel wordt het schrijven van VbaModule.SourceCode ondersteund.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of bestaande VBA-macrogegevens in het MPP-bestand moeten worden bijgewerkt. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Stelt een waarde in die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-indeling.

--------------------

Weergavegegevens omvatten de collecties Project.Views, Filters en Tables.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project in MPP-indeling. |

