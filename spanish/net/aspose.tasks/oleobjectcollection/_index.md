---
title: "Clase OleObjectCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OleObjectCollection. Representa una colección que contiene las instancias de la clase OleObject"
type: docs
weight: 1130
url: /es/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Representa una colección que contiene las instancias de la clase [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Limpia la colección. Para conservar estos cambios, se debe llamar a project.Save con new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Convierte la instancia de la clase `OleObjectCollection` en una lista que contiene las instancias de la clase [`OleObject`](../oleobject/). |

## Ejemplos

Muestra cómo trabajar con una colección de objetos OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// mediante acceso por índice
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// o enumeración, se puede iterar sobre objetos OLE
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Ver también

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


