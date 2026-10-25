---
title: "OleObject.Linked"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OleObject eigenschap. Haalt een waarde op die aangeeft of het projectbestand alleen een koppeling bevat naar de werkelijke gegevens die op de linkbron zijn opgeslagen"
type: docs
weight: 90
url: /nl/net/aspose.tasks/oleobject/linked/
---
## OleObject.Linked property

Haalt een waarde op die aangeeft of het projectbestand alleen een koppeling bevat naar de daadwerkelijke gegevens die bij de koppelingsbron zijn opgeslagen.

```csharp
public bool Linked { get; }
```

## Voorbeelden

Toont hoe informatie over OLE-objecten kan worden gelezen.

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

### Zie ook

* class [OleObject](../)
* namespace [Aspose.Tasks](../../oleobject/)
* assembly [Aspose.Tasks](../../../)


