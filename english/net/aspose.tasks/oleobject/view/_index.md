---
title: OleObject.View
second_title: Aspose.Tasks for .NET API Reference
description: OleObject property. Gets or sets the instance of the View class the inserted object belongs to
type: docs
weight: 120
url: /net/aspose.tasks/oleobject/view/
---
## OleObject.View property

Gets or sets the instance of the `View` class the inserted object belongs to.

```csharp
public View View { get; set; }
```

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

* class [View](../../view/)
* class [OleObject](../)
* namespace [Aspose.Tasks](../../oleobject/)
* assembly [Aspose.Tasks](../../../)


