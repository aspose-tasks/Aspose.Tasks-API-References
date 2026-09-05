---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database MS Project Server."
type: docs
weight: 161
url: /it/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database MS Project Server.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Inizializza una nuova istanza della classe [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Ottiene il guid del progetto da leggere. |
| [getSchema()](#getSchema--) | Ottiene lo schema di MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Imposta lo schema di MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Inizializza una nuova istanza della classe [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connectionString | java.lang.String | la stringa di connessione specificata. |
| projectGuid | java.util.UUID | il guid specificato di un progetto da leggere. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Ottiene il guid del progetto da leggere.

**Returns:**
java.util.UUID - il guid del progetto da leggere.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Ottiene lo schema di MS Project Server. Il valore predefinito è "pub".

**Returns:**
java.lang.String - lo schema di MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Imposta lo schema di MS Project Server. Il valore predefinito è "pub".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | lo schema di MS Project Server. |

