---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks for .NET API Reference
description: OleObjectCollection method. Clears the collection. In order to persist these changes project.Save should be called with new MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Clears the collection. In order to persist these changes project.Save should be called with new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Examples

How to clear OLE objects and persist these changes.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Shows how to remove OLE objects from the specified project.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### See Also

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


