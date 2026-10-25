---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Speichern von Projektdaten im MPP‑Format."
type: docs
weight: 149
url: /de/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Speichern von Projektdaten im MPP‑Format.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Initialisiert eine neue Instanz der Klasse [MPPSaveOptions](../../com.aspose/tasks/mppsaveoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getClearVba()](#getClearVba--) | Gibt einen Wert zurück, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen. |
| [getProtectionPassword()](#getProtectionPassword--) | Gibt ein Passwort zurück, das zum Schutz der resultierenden MPP-Datei verwendet wird. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Gibt einen Wert zurück, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen. |
| [getWriteFilters()](#getWriteFilters--) | Gibt einen Wert zurück, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
| [getWriteGroups()](#getWriteGroups--) | Gibt einen Wert zurück, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
| [getWriteVba()](#getWriteVba--) | Gibt einen Wert zurück, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen. |
| [getWriteViewData()](#getWriteViewData--) | Gibt einen Wert zurück, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Legt einen Wert fest, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Legt ein Passwort fest, das zum Schutz der resultierenden MPP-Datei verwendet wird. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Legt einen Wert fest, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Legt einen Wert fest, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Legt einen Wert fest, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Legt einen Wert fest, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Legt einen Wert fest, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [MPPSaveOptions](../../com.aspose/tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Gibt einen Wert zurück, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Ruft ein Passwort ab, das zum Schutz einer resultierenden MPP-Datei verwendet wird. Derzeit wird es für MS Project 2010 und neuere Formate unterstützt.

--------------------

Ein Nullwert zeigt an, dass die Projektdatei nicht geschützt ist.

**Returns:**
java.lang.String – ein Passwort, das zum Schutz einer resultierenden MPP-Datei verwendet wird.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Gibt einen Wert zurück, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen.

--------------------

MS Project erstellt für jede Aufgabe eine leere Ressourcenzuweisung. Setzen Sie dieses Flag auf true, um sie beim Speichern zu entfernen.

**Returns:**
boolean – ein Wert, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Gibt einen Wert zurück, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Filterdaten umfassen die Sammlungen Project.TaskFilters und Project.ResourceFilters.

--------------------

Derzeit unterstützt für MSP 2010 oder neuere Formate.

**Returns:**
boolean – ein Wert, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Gibt einen Wert zurück, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Gruppendaten umfassen die Sammlungen Project.TaskGroups und Project.ResourceGroups.

**Returns:**
boolean – ein Wert, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Ruft einen Wert ab, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen. Derzeit wird das Schreiben von VbaModule.SourceCode unterstützt.

**Returns:**
boolean – ein Wert, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Gibt einen Wert zurück, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Ansichtsdaten umfassen die Sammlungen Project.Views, Filters und Tables.

**Returns:**
boolean – ein Wert, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Legt einen Wert fest, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob vorhandene VBA-Makrodaten beim Speichern eines Projekts im MPP-Format entfernt werden sollen. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Setzt ein Passwort, das zum Schutz einer resultierenden MPP-Datei verwendet wird. Derzeit wird es für MS Project 2010 und neuere Formate unterstützt.

--------------------

Ein Nullwert zeigt an, dass die Projektdatei nicht geschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Passwort, das zum Schutz einer resultierenden MPP-Datei verwendet wird. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Legt einen Wert fest, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen.

--------------------

MS Project erstellt für jede Aufgabe eine leere Ressourcenzuweisung. Setzen Sie dieses Flag auf true, um sie beim Speichern zu entfernen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ungültige Ressourcenzuweisungen beim Speichern in MPP entfernt werden sollen. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Legt einen Wert fest, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Filterdaten umfassen die Sammlungen Project.TaskFilters und Project.ResourceFilters.

--------------------

Derzeit unterstützt für MSP 2010 oder neuere Formate.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Legt einen Wert fest, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Gruppendaten umfassen die Sammlungen Project.TaskGroups und Project.ResourceGroups.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Gruppendaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Setzt einen Wert, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen. Derzeit wird das Schreiben von VbaModule.SourceCode unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob vorhandene VBA-Makrodaten in der MPP-Datei aktualisiert werden sollen. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Legt einen Wert fest, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen.

--------------------

Ansichtsdaten umfassen die Sammlungen Project.Views, Filters und Tables.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Ansichtsdaten beim Speichern eines Projekts im MPP-Format geschrieben werden sollen. |

