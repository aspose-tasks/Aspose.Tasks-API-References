---
title: Class OleObject
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OleObject class. Represents an OLE object which can be inserter into Gantt Chart View of an MPP file
type: docs
weight: 1100
url: /net/aspose.tasks/oleobject/
---
## OleObject class

Represents an OLE object which can be inserter into Gantt Chart View of an MPP file.

```csharp
public class OleObject
```

## Constructors

| Name | Description |
| --- | --- |
| [OleObject](oleobject/)() | Initializes a new instance of the `OleObject` class. |

## Properties

| Name | Description |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Gets or sets the application name to open the embedded object with. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Gets or sets the embedded file's data; null if no data was embedded. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Gets or sets a flag indicating that OLE object should be shown either as an icon or as its regular picture. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Gets or sets the file format of the embedded object. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Gets or sets the full path of the inserted object. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Gets or sets the object id. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Gets or sets the label of the inserted object. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Gets a value indicating whether the project file contains only a link to the actual data stored at the link source. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Gets or sets the name of the instance of the OLE object. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Gets or sets the path to the temporary file of the inserted object. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Gets or sets the instance of the [`View`](./view/) class the inserted object belongs to. |

## Examples

Shows how to read info about OLE objects.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


