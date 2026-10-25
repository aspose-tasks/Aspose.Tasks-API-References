---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un lettore di base che può essere utilizzato per leggere gli UID del progetto da file Primavera XER o XML multi-progetto."
type: docs
weight: 196
url: /it/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Rappresenta un lettore di base che può essere utilizzato per leggere gli UID del progetto da file Primavera XER o XML multi-progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Restituisce un elenco degli oggetti di informazioni brevi del progetto. |
| [getProjectUids()](#getProjectUids--) | Restituisce un elenco degli identificatori unici dei progetti. |
| [loadProject(int projectUid)](#loadProject-int-) | Carica il progetto con l'identificatore univoco specificato. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Restituisce un elenco degli oggetti di informazioni brevi del progetto.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - un elenco degli oggetti di informazioni brevi del progetto
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Restituisce un elenco degli identificatori unici dei progetti.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Elenco degli identificatori unici dei progetti.
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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
