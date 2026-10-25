---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt kurze Informationen zu einem Projekt dar, das aus dem Primavera-Format geladen wurde."
type: docs
weight: 204
url: /de/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Stellt kurze Informationen zu einem Projekt dar, das aus dem Primavera-Format geladen wurde.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | Ruft das Export‑Flag des Projekts ab. |
| [getName()](#getName--) | Ruft den Namen des Projekts ab. |
| [getShortName()](#getShortName--) | Ruft den Kurznamen des Projekts (Projekt‑ID) ab. |
| [getUid()](#getUid--) | Ruft die UID des Projekts ab. |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


Ruft das Export‑Flag des Projekts ab. Wenn ein Projekt in Primavera für den Export ausgewählt wird, ist sein ExportFlag true. Einige Projekte, die nicht ausdrücklich für den Export ausgewählt wurden, können aufgrund ihrer Beziehung zum exportierten Projekt in eine XER‑Datei exportiert werden.

**Returns:**
boolean - Export‑Flag des Projekts.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Namen des Projekts ab.

**Returns:**
java.lang.String - Name des Projekts.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Ruft den Kurznamen des Projekts (Projekt‑ID) ab.

**Returns:**
java.lang.String - Kurzname des Projekts (Projekt‑ID).
### getUid() {#getUid--}
```
public final int getUid()
```


Ruft die UID des Projekts ab.

**Returns:**
int - UID des Projekts.
