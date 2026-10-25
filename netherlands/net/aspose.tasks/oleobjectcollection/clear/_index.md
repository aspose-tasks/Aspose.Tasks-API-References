---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OleObjectCollection-methode. Leegt de collectie. Om deze wijzigingen te behouden moet project.Save worden aangeroepen met nieuwe MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /nl/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Leegt de collectie. Om deze wijzigingen te behouden moet project.Save worden aangeroepen met new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Voorbeelden

Hoe OLE-objecten te wissen en deze wijzigingen te behouden.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Toont hoe OLE-objecten uit het opgegeven project te verwijderen.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Zie ook

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


