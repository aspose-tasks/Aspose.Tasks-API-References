---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar kort information om ett projekt som laddats från Primavera-format."
type: docs
weight: 204
url: /sv/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Representerar kort information om ett projekt som laddats från Primavera-format.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | Hämtar projektets exportflagga. |
| [getName()](#getName--) | Hämtar projektets namn. |
| [getShortName()](#getShortName--) | Hämtar projektets korta namn (Projekt-ID). |
| [getUid()](#getUid--) | Hämtar projektets Uid. |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


Hämtar projektets exportflagga. När ett projekt väljs för export i Primavera är dess ExportFlag sann. Vissa projekt som inte uttryckligen valts för export kan exporteras till en XER-fil på grund av deras relation till det exporterade projektet.

**Returns:**
boolean - projektets exportflagga.
### getName() {#getName--}
```
public final String getName()
```


Hämtar projektets namn.

**Returns:**
java.lang.String - projektets namn.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Hämtar projektets korta namn (Projekt-ID).

**Returns:**
java.lang.String - projektets korta namn (Projekt-ID).
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar projektets Uid.

**Returns:**
int - projektets Uid.
