---
title: OleObjectCollection.Clear
second_title: Referencia de Aspose.Tasks para la API de .NET
description: OleObjectCollection método. Borra la colección. Para que estos cambios persistan se debe llamar a project.Save con las nuevas MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /es/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Borra la colección. Para que estos cambios persistan, se debe llamar a project.Save con las nuevas MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Ejemplos

Cómo borrar objetos OLE y conservar estos cambios.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Ver también

* class [OleObjectCollection](../)
* espacio de nombres [Aspose.Tasks](../../oleobjectcollection/)
* asamblea [Aspose.Tasks](../../../)


