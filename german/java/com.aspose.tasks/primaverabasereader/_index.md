---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Baselleser dar, der zum Lesen von Projekt‑UIDs aus mehreren Primavera‑XER‑ oder XML‑Dateien verwendet werden kann."
type: docs
weight: 196
url: /de/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Stellt einen Baselleser dar, der zum Lesen von Projekt‑UIDs aus mehreren Primavera‑XER‑ oder XML‑Dateien verwendet werden kann.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Gibt eine Liste der Kurzinfo-Objekte des Projekts zurück. |
| [getProjectUids()](#getProjectUids--) | Gibt eine Liste der eindeutigen Kennungen der Projekte zurück. |
| [loadProject(int projectUid)](#loadProject-int-) | Lädt das Projekt mit der angegebenen eindeutigen Kennung. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Gibt eine Liste der Kurzinfo-Objekte des Projekts zurück.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - eine Liste der kurzen Informationsobjekte des Projekts
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Gibt eine Liste der eindeutigen Kennungen der Projekte zurück.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Liste der eindeutigen Kennungen der Projekte.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Lädt das Projekt mit der angegebenen eindeutigen Kennung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectUid | int | Eindeutige Kennung des zu ladenden Projekts. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
