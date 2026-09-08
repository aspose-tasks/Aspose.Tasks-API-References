---
title: "Project.OleObjects"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene una colección que contiene las instancias de la clase OleObject que están vinculadas o incrustadas en este archivo de proyecto. Disponible solo para el formato de archivo mpp. Esta colección es de solo lectura, excepto para la operación Clear."
type: docs
weight: 700
url: /es/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Obtiene una colección que contiene las instancias de la clase [`OleObject`](../../oleobject/) que están vinculadas o incrustadas en este archivo de proyecto. Disponible solo para el formato de archivo mpp. Esta colección es de solo lectura, excepto para la operación 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Ejemplos

Muestra cómo extraer objetos OLE incrustados.

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Ver también

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


