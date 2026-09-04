---
title: "PrimaveraDbReader"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un lecteur pour lire les informations du projet depuis la base de données Primavera."
type: docs
weight: 200
url: /fr/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Représente un lecteur pour lire les informations du projet depuis la base de données Primavera.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Initialise une nouvelle instance de la classe [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Charge le projet avec l'identifiant unique spécifié. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Initialise une nouvelle instance de la classe [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Paramètres qui spécifient comment se connecter à la base de données Primavera. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Charge le projet avec l'identifiant unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectUid | int | Identifiant unique du projet à charger. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
