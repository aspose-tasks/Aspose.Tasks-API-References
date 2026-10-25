---
title: "MspDbSettings"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données MS Project Server."
type: docs
weight: 161
url: /fr/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données MS Project Server.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Initialise une nouvelle instance de la classe [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Obtient le guid du projet à lire. |
| [getSchema()](#getSchema--) | Obtient le schéma du serveur MS Project. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Définit le schéma du serveur MS Project. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Initialise une nouvelle instance de la classe [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| connectionString | java.lang.String | la chaîne de connexion spécifiée. |
| projectGuid | java.util.UUID | le guid spécifié d'un projet à lire. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Obtient le guid du projet à lire.

**Returns:**
java.util.UUID - le guid du projet à lire.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Obtient le schéma du serveur MS Project. La valeur par défaut est "pub".

**Returns:**
java.lang.String - le schéma du serveur MS Project.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Définit le schéma du serveur MS Project. La valeur par défaut est "pub".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le schéma du serveur MS Project. |

