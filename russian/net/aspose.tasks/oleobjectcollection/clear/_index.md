---
title: "OleObjectCollection.Clear"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод OleObjectCollection. Очищает коллекцию. Чтобы сохранить эти изменения, следует вызвать project.Save с новыми MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /ru/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Очищает коллекцию. Чтобы сохранить эти изменения, следует вызвать project.Save с новыми MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Примеры

Как очистить OLE‑объекты и сохранить эти изменения.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Показывает, как удалить OLE‑объекты из указанного проекта.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### См. также

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


