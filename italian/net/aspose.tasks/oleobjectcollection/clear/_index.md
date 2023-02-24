---
title: OleObjectCollection.Clear
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: OleObjectCollection metodo. Cancella la collezione. Per mantenere queste modifiche project.Save dovrebbe essere chiamato con new MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /it/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Cancella la collezione. Per mantenere queste modifiche project.Save dovrebbe essere chiamato con new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Esempi

Come cancellare gli oggetti OLE e mantenere queste modifiche.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Guarda anche

* class [OleObjectCollection](../)
* spazio dei nomi [Aspose.Tasks](../../oleobjectcollection/)
* assemblea [Aspose.Tasks](../../../)


