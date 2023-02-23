---
title: OleObjectCollection.Clear
second_title: Справочник по Aspose.Tasks для .NET API
description: OleObjectCollection метод. Очищает коллекцию. Чтобы сохранить эти изменения project.Save следует вызывать с помощью new MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /ru/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Очищает коллекцию. Чтобы сохранить эти изменения, project.Save следует вызывать с помощью new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Примеры

Как очистить объекты OLE и сохранить эти изменения.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Смотрите также

* class [OleObjectCollection](../)
* пространство имен [Aspose.Tasks](../../oleobjectcollection/)
* сборка [Aspose.Tasks](../../../)


