---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks für .NET-API-Referenz
description: OleObjectCollection methode. Löscht die Sammlung. Um diese Änderungen beizubehalten sollte project.Save mit new aufgerufen werden MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /de/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Löscht die Sammlung. Um diese Änderungen beizubehalten, sollte project.Save mit new aufgerufen werden MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Beispiele

So löschen Sie OLE-Objekte und behalten diese Änderungen bei.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Siehe auch

* class [OleObjectCollection](../)
* namensraum [Aspose.Tasks](../../oleobjectcollection/)
* Montage [Aspose.Tasks](../../../)


