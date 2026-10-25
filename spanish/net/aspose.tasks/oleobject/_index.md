---
title: "Clase OleObject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OleObject. Representa un objeto OLE que puede insertarse en la vista de diagrama de Gantt de un archivo MPP"
type: docs
weight: 1120
url: /es/net/aspose.tasks/oleobject/
---
## OleObject class

Representa un objeto OLE que puede insertarse en la vista Gantt Chart de un archivo MPP.

```csharp
public class OleObject
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OleObject](oleobject/)() | Inicializa una nueva instancia de la clase `OleObject`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Obtiene o establece el nombre de la aplicación con la que abrir el objeto incrustado. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Obtiene o establece los datos del archivo incrustado; null si no se incrustaron datos. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Obtiene o establece una bandera que indica si el objeto OLE debe mostrarse como un ícono o como su imagen habitual. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Obtiene o establece el formato de archivo del objeto incrustado. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Obtiene o establece la ruta completa del objeto insertado. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Obtiene o establece el id del objeto. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Obtiene o establece la etiqueta del objeto insertado. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Obtiene un valor que indica si el archivo del proyecto contiene solo un enlace a los datos reales almacenados en la fuente del enlace. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Obtiene o establece el nombre de la instancia del objeto OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Obtiene o establece la ruta al archivo temporal del objeto insertado. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Obtiene o establece la instancia de la clase [`View`](./view/) a la que pertenece el objeto insertado. |

## Ejemplos

Muestra cómo leer información sobre objetos OLE.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


