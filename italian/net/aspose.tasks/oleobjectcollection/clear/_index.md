---
title: "OleObjectCollection.Clear"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo OleObjectCollection. Cancella la collezione. Per persistere queste modifiche, project.Save dovrebbe essere chiamato con new MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /it/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Cancella la raccolta. Per rendere persistenti queste modifiche, dovrebbe essere chiamato project.Save con new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Esempi

Come cancellare gli oggetti OLE e persistere queste modifiche.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Mostra come rimuovere gli oggetti OLE dal progetto specificato.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Vedi anche

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


