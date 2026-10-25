---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un lettore per leggere le informazioni del progetto dal database Primavera"
type: docs
weight: 200
url: /it/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Rappresenta un lettore per leggere le informazioni del progetto dal database Primavera
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Inizializza una nuova istanza della classe [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Carica il progetto con l'identificatore univoco specificato. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Inizializza una nuova istanza della classe [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Impostazioni che specificano come connettersi al DB di Primavera. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Carica il progetto con l'identificatore univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectUid | int | Identificatore unico del progetto da caricare. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
