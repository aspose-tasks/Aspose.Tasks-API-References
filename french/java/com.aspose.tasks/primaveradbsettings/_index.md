---
title: "PrimaveraDbSettings"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de définir les options nécessaires pour lire les données du projet depuis la base de données Primavera."
type: docs
weight: 201
url: /fr/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

Permet de définir les options nécessaires pour lire les données du projet depuis la base de données Primavera.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | Initialise une nouvelle instance de la classe [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getProjectId()](#getProjectId--) | Obtient l'identifiant du projet à lire. |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


Initialise une nouvelle instance de la classe [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| connectionString | java.lang.String | la chaîne de connexion spécifiée. |
| projectId | int | l'identifiant spécifié d'un projet à lire. |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


Obtient l'identifiant du projet à lire.

**Returns:**
int - identifiant du projet à lire.
