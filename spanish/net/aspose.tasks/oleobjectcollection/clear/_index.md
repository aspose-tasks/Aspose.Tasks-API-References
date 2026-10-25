---
title: "OleObjectCollection.Clear"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método OleObjectCollection. Borra la colección. Para persistir estos cambios, project.Save debe llamarse con new MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /es/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Limpia la colección. Para conservar estos cambios, se debe llamar a project.Save con new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Ejemplos

Cómo borrar objetos OLE y persistir estos cambios.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Muestra cómo eliminar objetos OLE del proyecto especificado.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Ver también

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


