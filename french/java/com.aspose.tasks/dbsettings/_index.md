---
title: "DbSettings"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier les paramètres pour lire depuis la base de données du projet."
type: docs
weight: 75
url: /fr/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Permet de spécifier les paramètres pour lire depuis la base de données du projet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Obtient la chaîne de connexion. |
| [getDriverClassName()](#getDriverClassName--) | Renvoie un nom de classe de pilote JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Définit la chaîne de connexion. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Définit un nom de classe de pilote JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Obtient la chaîne de connexion.

**Returns:**
java.lang.String - la chaîne de connexion.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Renvoie un nom de classe de pilote JDBC. Le nom de classe du pilote par défaut est "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - chaîne de classe du pilote.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Définit la chaîne de connexion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la chaîne de connexion. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Définit un nom de classe de pilote JDBC. Le nom de classe du pilote par défaut est "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un nom de classe de pilote JDBC. |

