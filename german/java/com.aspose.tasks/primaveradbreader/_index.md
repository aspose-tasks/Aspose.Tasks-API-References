---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Leser dar, um Projektinformationen aus der Primavera‑Datenbank zu lesen."
type: docs
weight: 200
url: /de/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Stellt einen Leser dar, um Projektinformationen aus der Primavera‑Datenbank zu lesen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Initialisiert eine neue Instanz der [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Lädt das Projekt mit der angegebenen eindeutigen Kennung. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Initialisiert eine neue Instanz der [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Einstellungen, die festlegen, wie eine Verbindung zur Primavera-DB hergestellt wird. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
